# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repo Is

This is the source for the [NASA PDS Software Portal](https://nasa-pds.github.io) — a Sphinx-generated static site that documents PDS software builds, processes, and team information. The repo doubles as the GitHub Pages host: the root of `main` contains the pre-built HTML output, while `docs/source/` contains the RST/Markdown source.

## Build Commands

```bash
# Install dependencies (use a virtualenv)
pip install -r requirements.txt

# Build and deploy HTML to the repo root (used by CI and for local preview)
cd docs && make github

# Build HTML locally without copying to root
cd docs && make html
# Output goes to docs/build/html/
```

The `make github` target runs `make clean html` then copies `docs/build/html/` up to the repo root — this is what CI commits to `main` as the live site.

## Architecture

**Two-layer structure:**

1. **`docs/source/`** — Sphinx source (RST + Markdown). Edit here.
2. **Repo root** — Pre-built HTML committed by CI (`pdsen-ci` bot). Do not edit HTML files directly; they are regenerated on every build.

**Key source directories:**

- `docs/source/releases/` — Per-build software release catalogs. Each build has its own subdirectory (e.g., `16/`, `17/`). The `index.rst` in each is a large RST table of all PDS tools for that build, and `rdd.rst` is an auto-generated Requirements & Delivery Document.
- `docs/source/collaborate/` — Contribution guides, developer resources, OSS policy.
- `docs/source/support/` — Contact info, discipline node support pages.
- `docs/source/teams/` — PDS team descriptions (PDSEN operations, SWG, PMC).
- `docs/source/conf.py` — Sphinx config. Current release is `B16`; update `release` and `version` here when cutting a new build.
- `docs/source/index.rst` — Site root TOC; controls which toctrees appear in navigation.

**CI workflows (`.github/workflows/`):**

- `build.yml` — Triggered on pushes to non-`main` branches that touch `docs/source/**`; builds and commits HTML back to that branch. Skips if actor is `pdsen-ci` to prevent loops.
- `rdd-gen.yml` — Runs weekly (Friday midnight); uses `pds-issues` CLI to generate `rdd.rst` for the current in-development build (matrix variable `build-number`), then rebuilds the site.

## Adding a New Build Release

1. Create `docs/source/releases/<N>/` with `index.rst` (software catalog table) and optionally `rdd.rst`.
2. Add it to `docs/source/releases/releases.rst` under "Past Releases" (or "Upcoming").
3. Update `docs/source/index.rst` if the "Current Release" pointer should change.
4. Update `release` and `version` in `docs/source/conf.py`.
5. Update the `build-number` matrix in `.github/workflows/rdd-gen.yml`.

## RDD Generation

The `pds-issues` CLI (from `lasso.issues`) generates RST release notes from closed GitHub issues tagged with a build label:

```bash
pds-issues --token <GITHUB_TOKEN> --format rst --issue_state closed --build B<N> --group-by-component
```

Output is `pdsen_issues.rst`; move it to `docs/source/releases/<N>/rdd.rst`.
