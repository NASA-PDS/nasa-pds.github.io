# PDS Continuous Integration / Continuous Deployment

---

## Purpose

To describe a consistent approach to developing CI/CD processes for PDS software products.

---

## Stable Releases

CI/CD for will differ between stable releases versus unstable releases (e.g. SNAPSHOT, -dev releases).

Here are the steps we want to accomplish during our stable release CI/CD process:

* Identify repo (Java or Python)
* Unit Test
* Integration Test
* Generate CHANGELOG (1)
* Generate REQUIREMENTS (1)
* Push updates to repo
* Tag Release in Github
* Build software
* Publish software (push to PyPi, Maven Central, Github Release Assets - Java only)
* Generate and package Documentation
* Push Documentation
    * To Github Pages
    * To Github Release Assets
* Ping pdsen-corral for updates (1)
    


### Github Actions Example

TBD link to template action or repo for this

---

## Unstable Releases

CI/CD for in-development software updates (e.g. Java SNAPSHOTS, Python -dev)

* Identify repo (Java or Python)
* Unit Test
* Integration Test
* Generate CHANGELOG (1)
* Generate REQUIREMENTS (1)
* Push updates to repo
* Build software
* Publish unstable release to Github Releases
* Publish to public artifact repos
    * Python - push to PyPi Test
    * Java - push to Maven Central SNAPSHOTS repo, upload package to Github assets
* Generate and package Documentation
* Push Documentation to Github Release Assets ONLY
* Ping pdsen-corral for updates (1)


(1) steps which could be wrapped into a single github action.

