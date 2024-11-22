==========================================
Release Description Document (Build B15.1)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B15.1`_

The following sections can be found in this document:

.. toctree::
   :glob:
   :maxdepth: 3

   rdd.rst


PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

No PDS4 Standards Updates

Software Changes
================
For each software repository, the changes are listed in 2 categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B15.1`_).

The 'Other Updates' occurs during the build cycle without being planned or attached to a theme. They are organized by
types (bug, enhancements, requirements, tasks). Any updates that require a de-scope of planned tasks are reviewed by the
PDS Software Working Group.

The deliveries are validated by the development team and go through an additional Integration & Test process, as
applicable, as indicated by the ```Testing Status``` column in the tables below. There are 3 possible statuses for
testing:

- |:blue_circle:| Skip Testing - Testing is not needed for this ticket. These are determined at the discretion of the
  team based upon the technical or operational nature of the closed task.
- |:yellow_circle:| Testing Needed
- |:green_circle:| Testing Complete - Initial testing complete, and test cases/results documented.

--------

Devops
------
*Parent repo for PDS DevOps activities*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/devops#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/devops>`_
     - `Issue Tracking <https://github.com/NASA-PDS/devops/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/devops/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/devops/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/devops/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`devops#69`_ Phase 2: Develop CI/CD for NPM/React projects
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================================+=================+===========================+
| `devops#78`_ Image vulnerability scanning updates have broken the Validate docker build | |:blue_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------+-----------------+---------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================================================================+===================+===========================+
| `devops#76`_ As a developer, I want to ensure image dependencies are secure                                                                       | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `devops#77`_ As a developer and tester, I want my test case to be automatically defined from the github ticket without manual editing, copy/paste | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Ds-view
-------
*Data Set View application (pds.nasa.gov/ds-view)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/ds-view#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/ds-view>`_
     - `Issue Tracking <https://github.com/NASA-PDS/ds-view/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/ds-view/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/ds-view/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/ds-view/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                        | I&T Status        | Priority / Bug Severity   |
+==============================================================================+===================+===========================+
| `ds-view#37`_ As a user, I want a landing page for Airborne context objects  | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------+-------------------+---------------------------+
| `ds-view#39`_ As a user, I want a landing page for Telescope context objects | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------+-------------------+---------------------------+
| `ds-view#38`_ As a user, I want a landing page for Facility context objects  | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Harvest
-------
*Standalone Harvest client application providing the functionality for capturing and indexing product metadata into the PDS Registry system (https://github.com/nasa-pds/registry).*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/harvest>`_
     - `Issue Tracking <https://github.com/NASA-PDS/harvest/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/harvest/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/harvest/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/harvest/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================+===================+===========================+
| `harvest#208`_ Read time out errors occurring with big data uploads                               | |:blue_circle:|   | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#206`_ Issues identified with uncaught throttling errors                                  | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#186`_ New records harvested in the registry don't have the expected Node value           | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#190`_ I want to update the OpenSearch schema whatever the number of fields to be updated | |:yellow_circle:| | s.critical                |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#197`_ Unknown date format used that could not be parsed by Harvest                       | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================================================================================+===================+===========================+
| `harvest#187`_ As a user, I want to include my organization name in the harvest metadata (`ops:Harvest_Info.ops:node_name`) | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#199`_ As a user, I want harvest to exit with non 0 code when the arguments are not parsable                        | |:yellow_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================================================+=================+===========================+
| `harvest#207`_ Update harvest to support batches with data volumes larger than AOSS allowable limit | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Nucleus
-------
*Nucleus is a software platform used to create workflows for the Planetary Data (PDS).*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/nucleus>`_
     - `Github Repo <https://github.com/NASA-PDS/nucleus>`_
     - `Issue Tracking <https://github.com/NASA-PDS/nucleus/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/nucleus/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/nucleus/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/nucleus/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`nucleus#130`_ Update Product-Level DAG with Upgraded Harvest
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+----------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                            | I&T Status      | Priority / Bug Severity   |
+==================================================================================+=================+===========================+
| `nucleus#121`_ Integrate the latest version 4.0.1 of harvest in Nucleus workflow | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Operations
----------
*Tickets for the PDSEN Operations Team*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/operations#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/operations>`_
     - `Issue Tracking <https://github.com/NASA-PDS/operations/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/operations/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/operations/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/operations/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                      | I&T Status        | Priority / Bug Severity   |
+============================================================+===================+===========================+
| `operations#551`_ [ldd-request] Create new LDD "dragonfly" | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------+-------------------+---------------------------+

--------

Pds4-information-model
----------------------
*The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-information-model/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-information-model>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-information-model/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds4-information-model/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-information-model/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-information-model/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================+===================+===========================+
| `pds4-information-model#822`_ Tests fail when there are multiple tests with multiple schemas/schematrons | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#834`_ emrsp namespaces are configured to be produced as https:                   | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#846`_ Download links broken for lddtool for online documentation                 | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================================================+=================+===========================+
| `pds4-information-model#825`_ Add `Product_Native` test case for #795 back to test suite | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Peppi
-----
*Planetary Data Explorere: Python (PEPPi) library (pds.peppi) to access Planetary Data from the Planetary Data System (formerly known as updart)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/peppi>`_
     - `Github Repo <https://github.com/NASA-PDS/peppi>`_
     - `Issue Tracking <https://github.com/NASA-PDS/peppi/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/peppi/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/peppi/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/peppi/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================+===================+===========================+
| `peppi#35`_ As a user, I want to filter on a specific processing level                | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `peppi#33`_ As a user, I want to search for collection products only                  | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `peppi#34`_ As a user, I want to search for bundle products only                      | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `peppi#32`_ As a user, I want to search for observational products only               | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `peppi#30`_ As a user, I want to search for products based upon a investigation LID   | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `peppi#31`_ As a user, I want to search for products based upon a instrument LID      | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `peppi#47`_ As a user, I want to see an online reference documentation of the library | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Planetary-data-cloud
--------------------
*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetary-data-cloud#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetary-data-cloud>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetary-data-cloud/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/planetary-data-cloud/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetary-data-cloud/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetary-data-cloud/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`planetary-data-cloud#80`_ Develop PDC Tenant Roles
+++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================================================================================================+===================+===========================+
| `planetary-data-cloud#75`_ As a user, I want a warm backup of my archive data to be available in the event of corruption of of primary archive data | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Portal-tasks
------------
*PDS Portal tasks repo used to track update requests for the website. Actual code and website are managed in separate private repo*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://pds.nasa.gov>`_
     - `Github Repo <https://github.com/NASA-PDS/portal-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal-tasks/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/portal-tasks/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal-tasks/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================================================================================+===================+===========================+
| `portal-tasks#102`_ tool registry search result count is incorrect                                                          | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#107`_ Missing PDS4_IMG_1100.xsd                                                                               | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#104`_ Tool Registry search does not work past initial query                                                   | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#103`_ `Browse and search` link broken on https://pds.nasa.gov/datastandards/dictionaries/index-missions.shtml | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#106`_ Missing PDS4_MSN_SURFACE_1A10.xsd                                                                       | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Portal-wp
---------
*New PDS Website driven by the PDS Web Modernization Working Group*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/portal-wp#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/portal-wp>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal-wp/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/portal-wp/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal-wp/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal-wp/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                          | I&T Status        | Priority / Bug Severity   |
+================================================================================================+===================+===========================+
| `portal-wp#72`_ Search results are linking to an empty page (`investigations/identifier/data`) | |:yellow_circle:| | s.critical                |
+------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                              | I&T Status        | Priority / Bug Severity   |
+====================================================================================================================+===================+===========================+
| `portal-wp#87`_ As a user, I want collection descriptions to default to `pds:Citation_Information.pds:description` | |:yellow_circle:| | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                            | I&T Status      | Priority / Bug Severity   |
+==================================================================+=================+===========================+
| `portal-wp#107`_ Test instructions for running WST Drupal Site   | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------+-----------------+---------------------------+
| `portal-wp#97`_ Add State to Homepage for what has been selected | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------+-----------------+---------------------------+

--------

Registry
--------
*PDS Registry provides service and software application necessary for tracking, searching, auditing, locating, and maintaining artifacts within the system. These artifacts can range from data files and label files, schemas, dictionary definitions for objects and elements, services, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================+===================+===========================+
| `registry#331`_ GEO index does not work, appears to be corrupted | |:yellow_circle:| | s.critical                |
+------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-common
---------------
*Library utilized by tools that manage and load data into the PDS Registry, including Harvest, Registry Manager, and Supplementer*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-common>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-common/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-common/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-common/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-common/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================+===================+===========================+
| `registry-common#83`_ As a Nucleus system, I want to be able to invoke harvest and registry-mgr from within the AWS VPC | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-legacy-solr
--------------------
*Legacy Registry Software components leveraging Apache Solr. Includes Legacy Harvest Tool, Registry Manager, PDS3 Catalog Tool, and Search Core library. These components provide the capabilities for loading PDS3 and PDS4 data into the Legacy Solr Registry, driving the PDS keyword search.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-legacy-solr#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-legacy-solr>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-legacy-solr/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-legacy-solr/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-legacy-solr/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-legacy-solr/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================+===================+===========================+
| `registry-legacy-solr#163`_ Cassini ISS Users Guide returns "No Document Information found in the registry" msg | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#147`_ `page_type` not working for context products                                        | |:blue_circle:|   | s.critical                |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-mgr
------------
*Standalone Registry Manager application responsible for managing the PDS Registry (https://github.com/NASA-PDS/registry) schemas and indexes.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-mgr>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-mgr/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-mgr/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-mgr/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-mgr/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================+===================+===========================+
| `registry-mgr#104`_ Update inline help to match latest features | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------+-------------------+---------------------------+

--------

Search-ui-legacy
----------------
*Legacy Keyword Search UI querying the Legacy Registry through Apache Solr.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://pds.nasa.gov/datasearch/keyword-search/>`_
     - `Github Repo <https://github.com/NASA-PDS/search-ui-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/search-ui-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/search-ui-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/search-ui-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/search-ui-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                          | I&T Status      | Priority / Bug Severity   |
+================================================================+=================+===========================+
| `search-ui-legacy#40`_ `Too many open files` error for servlet | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------+-----------------+---------------------------+

--------

System-i-n-t
------------
*Repo for PDS EN System I&T scripts and issue tracking*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/system-i-n-t#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/system-i-n-t>`_
     - `Issue Tracking <https://github.com/NASA-PDS/system-i-n-t/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/system-i-n-t/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/system-i-n-t/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/system-i-n-t/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`system-i-n-t#54`_ B15.0 System Integration & Test
++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`system-i-n-t#55`_ B15.0 Test Readiness Review (TRR)
++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

--------

Validate
--------
*Validates PDS4 product labels, data and PDS3 Volumes*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/validate/>`_
     - `Github Repo <https://github.com/NASA-PDS/validate>`_
     - `Issue Tracking <https://github.com/NASA-PDS/validate/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/validate/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/validate/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/validate/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================================================+===================+===========================+
| `validate#1028`_ validate incorrectly disallows Encoded_Native/encoding_standard_id = 'SEED 2.4'                 | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1066`_ Telescopes missing from registry context products config                                        | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#979`_ OutOfMemoryError when NASA validate v3.5.2 is executed through a library for a batch of products | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1008`_ The PDF verification / VeraPDF component of Validate seems to error on Windows paths            | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================================================================================================+===================+===========================+
| `validate#992`_ As a user, I want to validate that there is exactly one digit to the left of the decimal point for the specifier `e` or `E` | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Web-modernization
-----------------
*PDS.nasa.gov Web Modernization repo for managing the overall design process and user testing for modernizing the PDS web experience.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/web-modernization#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/web-modernization>`_
     - `Issue Tracking <https://github.com/NASA-PDS/web-modernization/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/web-modernization/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/web-modernization/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/web-modernization/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`web-modernization#239`_ Final Prep for MVP
+++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Liens
=====

+---------+---------+-------------+
| Issue   | Title   | Rationale   |
+=========+=========+=============+
+---------+---------+-------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B15.1)`_

Installation and Operation
==========================
PDS Engineering Node Software have 3 different venues/purposes for execution: Standalone, Discipline Node Deployment or
Engineering Node-only Deployment
For the Installation and Operation manual see the `users manuals` in the software summary sections below:

- `PDS Standalone`_

- `PDS Discipline Nodes`_

- `PDS Engineering Node Only`_

Reference documents
===================
This section details the controlling and applicable documents referenced for this release. The controlling documents are
as follows:

- PDS Level 1, 2 and 3 Requirements, April 20, 2017.

- PDS4 Project Plan, July 17, 2013.

- PDS4 System Architecture Specification, Version 1.3, September 1, 2013.

- PDS4 Operations Concept, Version 1.0, September 1, 2013.

- PDS Harvest Tool Software Requirements and Design Document (SRD/SDD), Version 1.2, September 1, 2013.

- PDS Preparation Tools Software Requirements and Design Document (SRD/SDD), Version 0.3, September 1, 2013.

- PDS Registry Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.

- PDS Report Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.

- PDS Search Service Software Requirements and Design Document (SRD/SDD), Version 1.0, September 1, 2013.

- PDS Search Scenarios, Version 1.0, September 1, 2013.

- PDS Search Protocol, Version 1.2, March 21, 2014.

- PDAP Search Protocol, Version 1.0, March 21, 2014.

- PDS Security Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.

- `PDS Deep Archive Software Requirements and Design Document (SRD/SDD)`_

- `PDS DOI Service Requirements and Design Document (SRD/SDD)`_

.. _plan B15.1: https://nasa-pds.github.io/releases/15.1/plan.html
.. _devops#69: https://github.com/NASA-PDS/devops/issues/69
.. _devops#78: https://github.com/NASA-PDS/devops/issues/78
.. _devops#76: https://github.com/NASA-PDS/devops/issues/76
.. _devops#77: https://github.com/NASA-PDS/devops/issues/77
.. _ds-view#37: https://github.com/NASA-PDS/ds-view/issues/37
.. _ds-view#39: https://github.com/NASA-PDS/ds-view/issues/39
.. _ds-view#38: https://github.com/NASA-PDS/ds-view/issues/38
.. _harvest#208: https://github.com/NASA-PDS/harvest/issues/208
.. _harvest#206: https://github.com/NASA-PDS/harvest/issues/206
.. _harvest#186: https://github.com/NASA-PDS/harvest/issues/186
.. _harvest#190: https://github.com/NASA-PDS/harvest/issues/190
.. _harvest#197: https://github.com/NASA-PDS/harvest/issues/197
.. _harvest#187: https://github.com/NASA-PDS/harvest/issues/187
.. _harvest#199: https://github.com/NASA-PDS/harvest/issues/199
.. _harvest#207: https://github.com/NASA-PDS/harvest/issues/207
.. _nucleus#130: https://github.com/NASA-PDS/nucleus/issues/130
.. _nucleus#121: https://github.com/NASA-PDS/nucleus/issues/121
.. _operations#551: https://github.com/NASA-PDS/operations/issues/551
.. _pds4-information-model#822: https://github.com/NASA-PDS/pds4-information-model/issues/822
.. _pds4-information-model#834: https://github.com/NASA-PDS/pds4-information-model/issues/834
.. _pds4-information-model#846: https://github.com/NASA-PDS/pds4-information-model/issues/846
.. _pds4-information-model#825: https://github.com/NASA-PDS/pds4-information-model/issues/825
.. _peppi#35: https://github.com/NASA-PDS/peppi/issues/35
.. _peppi#33: https://github.com/NASA-PDS/peppi/issues/33
.. _peppi#34: https://github.com/NASA-PDS/peppi/issues/34
.. _peppi#32: https://github.com/NASA-PDS/peppi/issues/32
.. _peppi#30: https://github.com/NASA-PDS/peppi/issues/30
.. _peppi#31: https://github.com/NASA-PDS/peppi/issues/31
.. _peppi#47: https://github.com/NASA-PDS/peppi/issues/47
.. _planetary-data-cloud#80: https://github.com/NASA-PDS/planetary-data-cloud/issues/80
.. _planetary-data-cloud#75: https://github.com/NASA-PDS/planetary-data-cloud/issues/75
.. _portal-tasks#102: https://github.com/NASA-PDS/portal-tasks/issues/102
.. _portal-tasks#107: https://github.com/NASA-PDS/portal-tasks/issues/107
.. _portal-tasks#104: https://github.com/NASA-PDS/portal-tasks/issues/104
.. _portal-tasks#103: https://github.com/NASA-PDS/portal-tasks/issues/103
.. _portal-tasks#106: https://github.com/NASA-PDS/portal-tasks/issues/106
.. _portal-wp#72: https://github.com/NASA-PDS/portal-wp/issues/72
.. _portal-wp#87: https://github.com/NASA-PDS/portal-wp/issues/87
.. _portal-wp#107: https://github.com/NASA-PDS/portal-wp/issues/107
.. _portal-wp#97: https://github.com/NASA-PDS/portal-wp/issues/97
.. _registry#331: https://github.com/NASA-PDS/registry/issues/331
.. _registry-common#83: https://github.com/NASA-PDS/registry-common/issues/83
.. _registry-legacy-solr#163: https://github.com/NASA-PDS/registry-legacy-solr/issues/163
.. _registry-legacy-solr#147: https://github.com/NASA-PDS/registry-legacy-solr/issues/147
.. _registry-mgr#104: https://github.com/NASA-PDS/registry-mgr/issues/104
.. _search-ui-legacy#40: https://github.com/NASA-PDS/search-ui-legacy/issues/40
.. _system-i-n-t#54: https://github.com/NASA-PDS/system-i-n-t/issues/54
.. _system-i-n-t#55: https://github.com/NASA-PDS/system-i-n-t/issues/55
.. _validate#1028: https://github.com/NASA-PDS/validate/issues/1028
.. _validate#1066: https://github.com/NASA-PDS/validate/issues/1066
.. _validate#979: https://github.com/NASA-PDS/validate/issues/979
.. _validate#1008: https://github.com/NASA-PDS/validate/issues/1008
.. _validate#992: https://github.com/NASA-PDS/validate/issues/992
.. _web-modernization#239: https://github.com/NASA-PDS/web-modernization/issues/239
.. _Software Release Summary (B15.1): https://nasa-pds.github.io/releases/15.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md