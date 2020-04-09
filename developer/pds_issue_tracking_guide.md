
# PDS Issue Tracking

* [Overview](#Overview)
* [Getting Started with Zenhub](#getting-started-with-zenhub)
* [Issue Creation Best Practices](#issue-creation-best-practices)
* [Help with Zenhub](#help-with-zenhub)
* [References](#references)

---

## Overview
The Planetary Data System has several issue tracking and project management mechanisms that serve different purposes:

| System | Applicable Nodes / Projects | Description | Access |
| ------ | --------------------------- | ----------- | ------ |
| [PDS JIRA](https://pds-jira.jpl.nasa.gov/secure/Dashboard.jspa) | PDS4 Standards Change Control Board | This JIRA is used specifically for tracking PDS4 Information Model Software Change Requests (SCRs) and their approval through the Change Control Board. Once and SCR is approved, the implementation will be tracked in the [PDS4 Information Model repo](https://github.com/NASA-PDS-Incubator/pds4-information-model/issues) | Access is restricted to PDS personnel, or [upon request](mailto:pds-operator@jpl.nasa.gov) |
| Github.com Issues | All open sourced PDS projects | Issues are created in their appropriate [NASA-PDS and NASA-PDS-Incubator repositories](https://nasa-pds.github.io/) | Public access |
| [Zenhub PDSEN Workspace](https://app.zenhub.com/workspaces/pdsen-workspace-5c87e859b7a0872dd10b87c5/board?repos=186914179,225741245,247182582,179379537,192617533,211189958,245216997,236086558,236099103,253108483,200280392,251664703,170207812,193572640,198717028,193800615,225956031,84491609,199739690,198517222,193560281) | All open sources PDS projects managed by PDS Engineering Node | [Zenhub](#Zenhub) is utilized for sprint planning, management, and reporting by integrating all PDS projects into one visual workspace | Access [available upon request](mailto:pds-operator@jpl.nasa.gov) |
| JPL Github Enterprise | PDS Engineering Internal Projects | Github Issues / Zenhub Internal EN software and operations projects and issue tracking ([Development](https://zenhub.jpl.nasa.gov/app/workspaces/pdsen-dev-internal-5d5ff11ab8761871eb7ed692/board?repos=23220), [Operations](https://zenhub.jpl.nasa.gov/app/workspaces/pds-ops-5e444561fe7e060b0e514b07/board?repos=31090,31009,31007))| Access restricted to JPL personnel only |

## Getting Started with Zenhub
Go to the applicable board to view / create / update new tickets:
    * [PDS EN Github.com Development](https://app.zenhub.com/workspaces/pdsen-workspace-5c87e859b7a0872dd10b87c5/board?repos=186914179,225741245,247182582,179379537,192617533,211189958,245216997,236086558,236099103,253108483,200280392,251664703,170207812,193572640,198717028,193800615,225956031,84491609,199739690,198517222,193560281)
    * [PDS EN JPL Internal Development](https://zenhub.jpl.nasa.gov/app/workspaces/pdsen-dev-internal-5d5ff11ab8761871eb7ed692/board?repos=27663,28856,29312,28901,25759,24033,23921,28407,23450,23220,23446,28406,23894,28296)
    * [PDS EN JPL Internal Operations](https://zenhub.jpl.nasa.gov/app/workspaces/pds-ops-5e444561fe7e060b0e514b07/board?repos=31090,31009,31007)

Alternatively, you can install the Zenhub Chrome/Firefox extension to view Zenhub within Github:
* [Zenhub for Github.com](https://www.zenhub.com/extension)
* [Zenhub for JPL Github Enterprise](https://zenhub.jpl.nasa.gov/)


## Issue Creation Best Practices

The PDS has uses the article ["Naming Guide For Task, Bug, and User Story Titles"](https://stratejos.ai/blog/naming-task-bug-user-story-titles/) for issue best practices.

*Here are some high-priority best practices we really want to try to follow:*

* In general, for tasks, bugs, and new features, at minimum, **start the title with a verb** (e.g. Ingest some data from somewhere or Update this page with some change)
* **Title** should be able to tell someone what was fixed or completed
    * We plan on using these issue titles for generating changelogs and report automatically
* Use [autolinked references](https://help.github.com/en/enterprise/2.18/user/github/writing-on-github/autolinked-references-and-urls#issues-and-pull-requests) wherever possible for traceability
    * Using references is a *HUGE* benefit in streamlining productivity, project management, provenance, and requirements/test traceability.


## Help with Zenhub
We use Zenhub to visualize all our tickets across Github.com repositories.

* [How to use Zenhub](https://help.zenhub.com/support/solutions/articles/43000010778-what-is-zenhub-an-intro-to-zenhub-in-github)
* [Zenhub Support](https://help.zenhub.com/support/home)

## References
* https://gist.github.com/robertpainsi/b632364184e70900af4ab688decf6f53
* https://help.github.com/en/enterprise/2.18/user/github/writing-on-github/autolinked-references-and-urls#issues-and-pull-requests
