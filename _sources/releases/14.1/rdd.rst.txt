==========================================
Release Description Document (Build B14.1)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B14.1`_

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
PDS Software Working Group (see `Plan B14.1`_).

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

Data-upload-manager
-------------------
*Data Upload Manager (DUM) component for managing the interface for data uploads to the Planetary Data Cloud from Data Providers and PDS Nodes.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/data-upload-manager>`_
     - `Github Repo <https://github.com/NASA-PDS/data-upload-manager>`_
     - `Issue Tracking <https://github.com/NASA-PDS/data-upload-manager/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/data-upload-manager/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/data-upload-manager/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/data-upload-manager/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`data-upload-manager#4`_ Develop Cost Model
+++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`data-upload-manager#13`_ CSS MVP: Deploy to MCP and Test Uploads to Nucleus
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`data-upload-manager#29`_ Develop Directory Write Locking Mechanism
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`data-upload-manager#51`_ Add User-Defined Object Metadata
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                          | I&T Status        | Level       | Priority / Bug Severity   |
+================================================================================================================================================+===================+=============+===========================+
| `data-upload-manager#50`_ As a user, I want to include a MD5 checksum in the the user-defined object metadata being sent in the upload payload | |:yellow_circle:| | requirement | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


--------

Deep-archive
------------
*PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/deep-archive/>`_
     - `Github Repo <https://github.com/NASA-PDS/deep-archive>`_
     - `Issue Tracking <https://github.com/NASA-PDS/deep-archive/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/deep-archive/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/deep-archive/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/deep-archive/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                     | I&T Status       | Priority / Bug Severity   |
+===========================================================================================================+==================+===========================+
| `deep-archive#158`_ Transfer manifest mismatch between `pds-deep-archive` and `pds-deep-registry-archive` | |:green_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `deep-archive#155`_ pds-deep-registry-archive produces invalid SIPs/AIPs                                  | |:green_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `deep-archive#151`_ Installation instructions don't work on Windows 11                                    | |:green_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                  | I&T Status      | Priority / Bug Severity   |
+========================================================================================================================+=================+===========================+
| `deep-archive#159`_ Upgrade deep-archive to comply with latest search API changes (API v1.4.0 / pds-api-client v1.5.0) | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`devops#37`_ Automatically deploy an up to date I&T platform where all software can be tested (Part 2)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`devops#67`_ Develop baseline CI/CD for React Projects
++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

--------

Doi-ui
------
*The web interface for the PDS DOI Service providing the ability management PDS archive DOIs. See the DOI Service for more details on the available capabilities. https://nasa-pds.github.io/doi-service/*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/doi-ui/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/doi-ui/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/doi-ui/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                | I&T Status       | Priority / Bug Severity   |
+======================================================================================================================+==================+===========================+
| `doi-ui#215`_ When the cognito token is expired, the UI fails and returns a misleading/badly formatted error message | |:green_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

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
Bugs
++++

+-----------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                 | I&T Status       | Priority / Bug Severity   |
+=======================================================================+==================+===========================+
| `ds-view#12`_ v2.14.2 does not work for resource links                | |:green_circle:| | s.high                    |
+-----------------------------------------------------------------------+------------------+---------------------------+
| `ds-view#14`_ Memory leak in Solr connections leading to Tomcat crash | |:blue_circle:|  | s.critical                |
+-----------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                   | I&T Status       | Priority / Bug Severity   |
+=========================================================================================+==================+===========================+
| `ds-view#8`_ Upgrade to latest Solr 9.3.x                                               | |:blue_circle:|  | unknown                   |
+-----------------------------------------------------------------------------------------+------------------+---------------------------+
| `ds-view#3`_ Upgrade Dataset View and dependencies to support Harvest/Registry upgrades | |:green_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------+------------------+---------------------------+

--------

Feedback-widget
---------------
*Javascript widget for user feedback*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/feedback-widget#pds-feedback-widget>`_
     - `Github Repo <https://github.com/NASA-PDS/feedback-widget>`_
     - `Issue Tracking <https://github.com/NASA-PDS/feedback-widget/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/feedback-widget/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/feedback-widget/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/feedback-widget/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                        | I&T Status        | Priority / Bug Severity   |
+==============================================================+===================+===========================+
| `feedback-widget#18`_ Feedback says (CORS) error but submits | |:yellow_circle:| | s.medium                  |
+--------------------------------------------------------------+-------------------+---------------------------+

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
`harvest#129`_ Add Support for LBLX File Extension
++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                              | I&T Status        | Level       | Priority / Bug Severity   |
+====================================================================================================+===================+=============+===========================+
| `harvest#130`_ As a user, I want to ingest data products with labels having `.lblx` file extension | |:yellow_circle:| | requirement | p.must-have               |
+----------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================+===================+===========================+
| `harvest#134`_ `Too many requests` error to OpenSearch                           | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#141`_ A bundle that previously loaded throws an error on reload attempt | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Lasso-issues
------------
*Utilities for wrapping GitHub API for creating specific data structures and reports from GitHub issues*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/lasso-issues#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/lasso-issues>`_
     - `Issue Tracking <https://github.com/NASA-PDS/lasso-issues/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/lasso-issues/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/lasso-issues/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/lasso-issues/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                  | I&T Status        | Priority / Bug Severity   |
+========================================================================================================================+===================+===========================+
| `lasso-issues#11`_ add-version-label-to-open-bugs fails when launched multiple times as sometime done through the CICD | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `lasso-issues#7`_ Unable to generate RDD when upgrading rstcloth 0.5.0                                                 | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Ldd-gen-action
--------------
*Do a "roundup" of a local data dictionary, a/k/a PDS-style continuous integration for local data dictionary*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/ldd-gen-action#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/ldd-gen-action>`_
     - `Issue Tracking <https://github.com/NASA-PDS/ldd-gen-action/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/ldd-gen-action/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/ldd-gen-action/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/ldd-gen-action/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================+===================+===========================+
| `ldd-gen-action#7`_ Submodules execution does not support nested dependencies | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Ldd-manager
-----------
*tools and software needed for managing PDS4 Sub-Models (formerly known as Data Dictionaries)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/ldd-manager#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/ldd-manager>`_
     - `Issue Tracking <https://github.com/NASA-PDS/ldd-manager/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/ldd-manager/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/ldd-manager/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/ldd-manager/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================+===================+===========================+
| `ldd-manager#2`_ Generate does not fail fast when the ingest ldd file is missing | |:green_circle:|  | s.low                     |
+----------------------------------------------------------------------------------+-------------------+---------------------------+
| `ldd-manager#7`_ LDD Manager fails when there are nested dependencies            | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Mi-label
--------
*Metadata Injector for PDS Labels (MILabel) provides a command-line interface for generating PDS4 Labels using a user provided PDS4 XML template and input (source) data products.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/mi-label/>`_
     - `Github Repo <https://github.com/NASA-PDS/mi-label>`_
     - `Issue Tracking <https://github.com/NASA-PDS/mi-label/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/mi-label/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/mi-label/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/mi-label/releases>`_ 


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
| `mi-label#64`_ Executing `pds-generate` does not output anything | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------+-------------------+---------------------------+
| `mi-label#46`_ Jackson-databind vulnerability identified         | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------+-------------------+---------------------------+

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
`nucleus#17`_ CSS MVP: Deploy Baseline Nucleus for Catalina Sky Survey in Development Environment
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`nucleus#66`_ MCP Pilot: Pilot Nucleus Deployment for CSS and MESSENGER MDIS Data
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`nucleus#62`_ Develop Support For Off-Nominal Data Loads
++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------+-----------------+---------------------------+
| Issue                                         | I&T Status      | Priority / Bug Severity   |
+===============================================+=================+===========================+
| `nucleus#76`_ Nucleus documentation is broken | |:blue_circle:| | s.medium                  |
+-----------------------------------------------+-----------------+---------------------------+

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
`operations#379`_ Phase 2: Wordpress migration for pds-engineering website
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`operations#459`_ B14.0 dLDD Build and I&T
++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`operations#455`_ B14.0 EN Deployment & Release
+++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

--------

Pds-api
-------
*PDS web APIs specifications and user's manual*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds-api/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`pds-api#274`_ Initialize a Wrapper API Client
++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

--------

Pds-api-client
--------------
*Python library and API for accessing the online PDS Search API. This repository however only contains the utilities used to generate, test, document and demo the actual pds.api-client package. The library itself is only released on pypi (https://pypi.org/project/pds.api-client/) but not here on github*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-api-client/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api-client>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api-client/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds-api-client/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api-client/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api-client/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================+===================+===========================+
| `pds-api-client#29`_ product_properties_list() returns None | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------+-------------------+---------------------------+

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
`pds4-information-model#700`_ Document Nuances for Reusability of Generic LDD Classes/Attributes
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#703`_ B14.1 Information Model SCR Implementation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#704`_ B14.1 Information Model Delivery to I&T
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#705`_ B14.1 Standards Documents Updates
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#713`_ B14.1 SCR Freeze
++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================================================+===================+===========================+
| `pds4-information-model#738`_ LDDTool is not creating valid URL for KPLO                                                  | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#761`_ Documentation broken with latest upgrade for maven site plugin                              | |:blue_circle:|   | s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#471`_ PDS4 IM repo fails with openjdk 17+                                                         | |:yellow_circle:| | s.low                     |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#744`_ LDDTool producing invalid XSD for Voyager LDD                                               | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#733`_ LDDTool is throwing ERROR SetMasterAttrXMLBaseDataTypeFromDataType - Data Type is missing - | |:yellow_circle:| | s.critical                |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#763`_ Version flag no longer works on Windows                                                     | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#746`_ JDK17 issue re-introduced bug per #733                                                      | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#754`_ webpage links are not working                                                               | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#750`_ Unable to build maven site after JDK17 upgrade                                              | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                  | I&T Status        | Priority / Bug Severity   |
+========================================================================+===================+===========================+
| `pds4-information-model#709`_ Add KARI as a new agency `urn:kari:kpds` | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================================+===================+===========================+
| `pds4-information-model#716`_ [namespace-registry]update namespace URL for KPDS                       | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#734`_ Add LDDTool Execution Smoke Test to Branch Testing and Unstable testing | |:blue_circle:|   | p.should-have             |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`planetary-data-cloud#35`_ MCP Pilot: Deploy Registry
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#61`_ Design and Implement Initial Archive Browser Beta
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#69`_ Design and Implement Minor Planet Center (MPC) Cloud Backup Solution
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#71`_ CSS MVP: Identify Requirements and Complete CSS AWS Open Data Registry Onboarding
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                           | I&T Status        | Level       | Priority / Bug Severity   |
+=================================================================================================================================+===================+=============+===========================+
| `planetary-data-cloud#90`_ As a user, I want to know how the CSS archive is organized and how users can find the data they need | |:yellow_circle:| | requirement | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `planetary-data-cloud#91`_ As a user, I want to know how to use CSS data on AWS                                                 | |:yellow_circle:| | requirement | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`planetary-data-cloud#76`_ Design and Implement Warm Storage Data Backup Solution
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#77`_ B14.1 Bi-Annual Cost Model Review
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#79`_ Phase 1 Migration of Existing Production JPL AWS Infra to MCP
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================================================================+=================+===========================+
| `planetary-data-cloud#72`_ Update cost model to provide more accurate representation of existing Registry deployments | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Planetary-data-engine
---------------------
*Free-text search capability for planetary data, services, tools, and information*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetary-data-engine#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetary-data-engine>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetary-data-engine/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/planetary-data-engine/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetary-data-engine/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetary-data-engine/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`planetary-data-engine#5`_ Complete Sinequa Useability Analysis
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-engine#7`_ Develop Query Test Suite and Success Criteria
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

--------

Portal-wp-tasks
---------------
*PDS Web Design System*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds>`_
     - `Github Repo <https://github.com/NASA-PDS/portal-wp-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal-wp-tasks/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/portal-wp-tasks/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal-wp-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal-wp-tasks/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`portal-wp-tasks#44`_ Develop Initial Headless Wordpress Docker Deployment
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`portal-wp-tasks#49`_ Implement Header
++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`portal-wp-tasks#56`_ Implement Initial Investigation Landing Page Template and Associated Components
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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
`registry#155`_ Registry Multi-tenancy Design and implementation with Cognito
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry#178`_ Improved Fault Tolerance for Registry and Registry API
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry#231`_ Design Support for Alternate Data File Paths
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry#258`_ Implement Cloud Resources for OpenSearch Serverless Authentication
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------+-----------------+---------------------------+
| Issue                                              | I&T Status      | Priority / Bug Severity   |
+====================================================+=================+===========================+
| `registry#234`_ Missing NAIF from Legacy Dashboard | |:blue_circle:| | s.low                     |
+----------------------------------------------------+-----------------+---------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================================+=================+===========================+
| `registry#176`_ As a user, I want the registry to have 99.9999999% uptime | |:blue_circle:| | p.must-have               |
+---------------------------------------------------------------------------+-----------------+---------------------------+

--------

Registry-api
------------
*Web API service for the PDS Registry, providing the implementation of the PDS Search API (https://github.com/nasa-pds/pds-api) for the PDS Registry.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-api/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-api/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-api/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`registry-api#389`_ Cleanup Code Scanning Issues Identified
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------+------------------+---------+---------------------------+
| Issue                                                                            | I&T Status       | Level   | Priority / Bug Severity   |
+==================================================================================+==================+=========+===========================+
| `registry-api#387`_ Cleanup logging of keys                                      | |:green_circle:| | bug     | s.medium                  |
+----------------------------------------------------------------------------------+------------------+---------+---------------------------+
| `registry-api#388`_ Insufficient scrubbing of user input values prior to logging | |:green_circle:| | bug     | s.medium                  |
+----------------------------------------------------------------------------------+------------------+---------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                  | I&T Status        | Priority / Bug Severity   |
+========================================================================================================================+===================+===========================+
| `registry-api#404`_ Broken tests per pagination upgrade #397                                                           | |:blue_circle:|   | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#352`_ Pagination performance does not meet requirements                                                  | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#411`_ members query return 500 when members do not exist in the registry or alternate_id does not exists | |:yellow_circle:| | s.critical                |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
Bugs
++++

+------------------------------------------------+-------------------+---------------------------+
| Issue                                          | I&T Status        | Priority / Bug Severity   |
+================================================+===================+===========================+
| `registry-common#40`_ Fix code scanning alerts | |:yellow_circle:| | s.high                    |
+------------------------------------------------+-------------------+---------------------------+

--------

Registry-harvest-legacy
-----------------------
*Legacy Harvest Tool for loading PDS4 data into the Legacy Solr Registry driving the website keyword search.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-harvest-legacy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-harvest-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-harvest-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-harvest-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-harvest-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-harvest-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                | I&T Status        | Priority / Bug Severity   |
+======================================================================================================+===================+===========================+
| `registry-harvest-legacy#8`_ As a user, I want to ingest Product_External products into the Registry | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-mgr-legacy
-------------------
*Software app for managing the Legacy Solr Registry on pds.nasa.gov. This application is tightly coupled with https://github.com/NASA-PDS/registry-harvest-legacy and https://github.com/NASA-PDS/search-ui-legacy*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-mgr-legacy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-mgr-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-mgr-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-mgr-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-mgr-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-mgr-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================================================+===================+===========================+
| `registry-mgr-legacy#42`_ Hit count and pagination not working in XSLT response             | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-mgr-legacy#49`_ Faceting is not working properly for counts and overall functions | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------+------------------+---------------------------+
| Issue                                                  | I&T Status       | Priority / Bug Severity   |
+========================================================+==================+===========================+
| `registry-mgr-legacy#17`_ Upgrade to latest Solr 9.3.x | |:green_circle:| | unknown                   |
+--------------------------------------------------------+------------------+---------------------------+

--------

Registry-pds3-catalog
---------------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-pds3-catalog#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-pds3-catalog>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-pds3-catalog/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-pds3-catalog/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-pds3-catalog/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-pds3-catalog/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================================+===================+===========================+
| `registry-pds3-catalog#4`_ Upgrade Catalog Tool and dependencies to support Harvest/Registry upgrades | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-pds3-catalog#6`_ Upgrade to latest Solr 9.3.x                                               | |:green_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-sweepers
-----------------
*Scripts that run regularly on the registry database, to clean and consolidate information *

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-sweepers#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-sweepers>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-sweepers/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-sweepers/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-sweepers/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-sweepers/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================================================+===================+===========================+
| `registry-sweepers#86`_ Property values returned by the API are inconsistent, as list or single value.                | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-sweepers#111`_ Timeout bug when running legacy dashboard sync                                               | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-sweepers#109`_ When building registry-sweeper version 1.2.1, docker image 1.3.0 was published on docker hub | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================+===================+===========================+
| `registry-sweepers#92`_ Investigate/implement non-redundant provenance processing | |:yellow_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Roundup-action
--------------
*Do a "roundup", a/k/a PDS-style continuous integration and delivery*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/roundup-action#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/roundup-action>`_
     - `Issue Tracking <https://github.com/NASA-PDS/roundup-action/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/roundup-action/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/roundup-action/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/roundup-action/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                | I&T Status      | Priority / Bug Severity   |
+======================================================================================+=================+===========================+
| `roundup-action#136`_ Roundup DocsPublication step not working in maven              | |:blue_circle:| | s.high                    |
+--------------------------------------------------------------------------------------+-----------------+---------------------------+
| `roundup-action#124`_ Roundup pushes version update prior to completion of execution | |:blue_circle:| | s.medium                  |
+--------------------------------------------------------------------------------------+-----------------+---------------------------+

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

+----------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                | I&T Status        | Priority / Bug Severity   |
+======================================================================+===================+===========================+
| `search-ui-legacy#7`_ NullPointerException when `wt` is not provided | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                              | I&T Status       | Priority / Bug Severity   |
+====================================================================================================+==================+===========================+
| `search-ui-legacy#1`_ Upgrade Keyword Search and dependencies to support Harvest/Registry upgrades | |:green_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------+------------------+---------------------------+

--------

Software-issues-repo
--------------------
*Issue tracking repository as a centralized entry point for general PDS software bugs and feature requests.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/software-issues-repo#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/software-issues-repo>`_
     - `Issue Tracking <https://github.com/NASA-PDS/software-issues-repo/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/software-issues-repo/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/software-issues-repo/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/software-issues-repo/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`software-issues-repo#67`_ Switchover from PDS JIRA to Private GitHub for PDS4 SCR Management
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#80`_ Upgrade Legacy Registry Tools and Services to Fix Vulnerability
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#93`_ B14.1 Bi-Annual Triage CodeQL Static Code Analysis Scan Results
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                   | I&T Status       | Priority / Bug Severity   |
+=========================================================================================================+==================+===========================+
| `software-issues-repo#54`_ As a user, I want to ensure no passwords/secrets are committed to a PDS repo | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `software-issues-repo#49`_ As a software user, I want to see the known bugs for a component release     | |:blue_circle:|  | p.could-have              |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+

--------

Transform
---------
*Transforms PDS3 and PDS4 product labels and data into various formats.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/transform/>`_
     - `Github Repo <https://github.com/NASA-PDS/transform>`_
     - `Issue Tracking <https://github.com/NASA-PDS/transform/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/transform/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/transform/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/transform/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================================+===================+===========================+
| `transform#30`_ [SECURITY] Upgrade to log4j-core/log4j-api                          | |:green_circle:|  | s.low                     |
+-------------------------------------------------------------------------------------+-------------------+---------------------------+
| `transform#45`_ Broken download link and Windows JAVA settings in installation docs | |:green_circle:|  | s.medium                  |
+-------------------------------------------------------------------------------------+-------------------+---------------------------+
| `transform#67`_ Transform failing with `java.lang.NoClassDefFoundError` on Windows  | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------+-------------------+---------------------------+
| `transform#46`_ NoClassDefFoundError exception when transforming XML to PDS3 label  | |:green_circle:|  | s.medium                  |
+-------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`validate#695`_ Update Validate Test Suite to Support Larger Data Sets
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#833`_ Fix Performance and Content Validation Regressions
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================================+===================+===========================+
| `validate#432`_ Requirement #308 does not appear to be working for checking referential integrity from products to others in the bundle | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#761`_ Validate gives errors for 'NaN' values in IEEE754 data                                                                  | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#763`_ Validate.bat does not execute on Windows                                                                                | |:green_circle:|  | s.critical                |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#809`_ Validate fails to read files on Windows systems after Internal Reference check updates (#308)                           | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#754`_ Validate 3.3.0 erroneously reports data objects out of offset order                                                     | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#750`_ Validate-refs with manifest of file paths does not seem to read the files correctly                                     | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#739`_ Intermittent network failures attempting repeated downloads of schemas/schematrons                                      | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#781`_ Validate making incorrect assumption that first object has and object length == `file_size`                             | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#760`_ Uncaught exception thrown when only 1 of schemas/schematrons are provided via command-line                              | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#475`_ Validate crashes on invalid # of records, and spurious file left behind                                                 | |:green_circle:|  | p.wont-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#681`_ Validate incorrectly throws precision mismatch error for Table_Delimited                                                | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#698`_ Investigate and Fix code scanning alert for potential improvements                                                      | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#747`_ validate flags IEEE 754 "infinity" values as invalid                                                                    | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#427`_ validate does not work correct when path name contains a space on mac                                                   | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#723`_ Installation instructions need updates for Windows                                                                      | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#785`_ validate catches valid_maximum but not valid_minimum                                                                    | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#748`_ Buffer limit IOException thrown with validate-refs                                                                      | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#854`_ validate 3.5.0-SNAPSHOT attempts to look at all files, not just *.xml                                                   | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================================================================+===================+===========================+
| `validate#741`_ As a user, I want validate's referential integrity tool to read a manifest of files and check referential integrity                      | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#755`_ As a user, I want validate to throw an error when a file is being referenced by more than one label                                      | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#308`_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#773`_ As a user, I want validate with the registry when a file is being referenced by more than one label                                      | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Web-analytics
-------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/web-analytics#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/web-analytics>`_
     - `Issue Tracking <https://github.com/NASA-PDS/web-analytics/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/web-analytics/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/web-analytics/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/web-analytics/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================+===================+===========================+
| `web-analytics#21`_ As a user, I want year over year metrics for total egress | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------+-------------------+---------------------------+

Liens
=====

+-----------------------------------------------------------------------------------------+-----------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Issue                                                                                   | Title                                                                       | Rationale                                                                                                                                                                                                                                          |
+=========================================================================================+=============================================================================+====================================================================================================================================================================================================================================================+
| pds-swg_26_ [CR] Defer Registry/API new requirements, Add Performance Improvement Tasks | [CR] Defer Registry/API new requirements, Add Performance Improvement Tasks | Increased scope of NASA-PDS/registry#185 to use Cognito for multi-tenant OpenSearch requires developer needed for other tasks   NASA-PDS/registry-sweepers#92 was necessary in order to decrease cost and improve scalability of registry sweepers |
+-----------------------------------------------------------------------------------------+-----------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B14.1)`_

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

.. _plan B14.1: https://nasa-pds.github.io/releases/14.1/plan.html
.. _data-upload-manager#4: https://github.com/NASA-PDS/data-upload-manager/issues/4
.. _data-upload-manager#13: https://github.com/NASA-PDS/data-upload-manager/issues/13
.. _data-upload-manager#29: https://github.com/NASA-PDS/data-upload-manager/issues/29
.. _data-upload-manager#51: https://github.com/NASA-PDS/data-upload-manager/issues/51
.. _data-upload-manager#50: https://github.com/NASA-PDS/data-upload-manager/issues/50
.. _deep-archive#158: https://github.com/NASA-PDS/deep-archive/issues/158
.. _deep-archive#155: https://github.com/NASA-PDS/deep-archive/issues/155
.. _deep-archive#151: https://github.com/NASA-PDS/deep-archive/issues/151
.. _deep-archive#159: https://github.com/NASA-PDS/deep-archive/issues/159
.. _devops#37: https://github.com/NASA-PDS/devops/issues/37
.. _devops#67: https://github.com/NASA-PDS/devops/issues/67
.. _doi-ui#215: https://github.com/NASA-PDS/doi-ui/issues/215
.. _ds-view#12: https://github.com/NASA-PDS/ds-view/issues/12
.. _ds-view#14: https://github.com/NASA-PDS/ds-view/issues/14
.. _ds-view#8: https://github.com/NASA-PDS/ds-view/issues/8
.. _ds-view#3: https://github.com/NASA-PDS/ds-view/issues/3
.. _feedback-widget#18: https://github.com/NASA-PDS/feedback-widget/issues/18
.. _harvest#129: https://github.com/NASA-PDS/harvest/issues/129
.. _harvest#130: https://github.com/NASA-PDS/harvest/issues/130
.. _harvest#134: https://github.com/NASA-PDS/harvest/issues/134
.. _harvest#141: https://github.com/NASA-PDS/harvest/issues/141
.. _lasso-issues#11: https://github.com/NASA-PDS/lasso-issues/issues/11
.. _lasso-issues#7: https://github.com/NASA-PDS/lasso-issues/issues/7
.. _ldd-gen-action#7: https://github.com/NASA-PDS/ldd-gen-action/issues/7
.. _ldd-manager#2: https://github.com/NASA-PDS/ldd-manager/issues/2
.. _ldd-manager#7: https://github.com/NASA-PDS/ldd-manager/issues/7
.. _mi-label#64: https://github.com/NASA-PDS/mi-label/issues/64
.. _mi-label#46: https://github.com/NASA-PDS/mi-label/issues/46
.. _nucleus#17: https://github.com/NASA-PDS/nucleus/issues/17
.. _nucleus#66: https://github.com/NASA-PDS/nucleus/issues/66
.. _nucleus#62: https://github.com/NASA-PDS/nucleus/issues/62
.. _nucleus#76: https://github.com/NASA-PDS/nucleus/issues/76
.. _operations#379: https://github.com/NASA-PDS/operations/issues/379
.. _operations#459: https://github.com/NASA-PDS/operations/issues/459
.. _operations#455: https://github.com/NASA-PDS/operations/issues/455
.. _pds-api#274: https://github.com/NASA-PDS/pds-api/issues/274
.. _pds-api-client#29: https://github.com/NASA-PDS/pds-api-client/issues/29
.. _pds4-information-model#700: https://github.com/NASA-PDS/pds4-information-model/issues/700
.. _pds4-information-model#703: https://github.com/NASA-PDS/pds4-information-model/issues/703
.. _pds4-information-model#704: https://github.com/NASA-PDS/pds4-information-model/issues/704
.. _pds4-information-model#705: https://github.com/NASA-PDS/pds4-information-model/issues/705
.. _pds4-information-model#713: https://github.com/NASA-PDS/pds4-information-model/issues/713
.. _pds4-information-model#738: https://github.com/NASA-PDS/pds4-information-model/issues/738
.. _pds4-information-model#761: https://github.com/NASA-PDS/pds4-information-model/issues/761
.. _pds4-information-model#471: https://github.com/NASA-PDS/pds4-information-model/issues/471
.. _pds4-information-model#744: https://github.com/NASA-PDS/pds4-information-model/issues/744
.. _pds4-information-model#733: https://github.com/NASA-PDS/pds4-information-model/issues/733
.. _pds4-information-model#763: https://github.com/NASA-PDS/pds4-information-model/issues/763
.. _pds4-information-model#746: https://github.com/NASA-PDS/pds4-information-model/issues/746
.. _pds4-information-model#754: https://github.com/NASA-PDS/pds4-information-model/issues/754
.. _pds4-information-model#750: https://github.com/NASA-PDS/pds4-information-model/issues/750
.. _pds4-information-model#709: https://github.com/NASA-PDS/pds4-information-model/issues/709
.. _pds4-information-model#716: https://github.com/NASA-PDS/pds4-information-model/issues/716
.. _pds4-information-model#734: https://github.com/NASA-PDS/pds4-information-model/issues/734
.. _planetary-data-cloud#35: https://github.com/NASA-PDS/planetary-data-cloud/issues/35
.. _planetary-data-cloud#61: https://github.com/NASA-PDS/planetary-data-cloud/issues/61
.. _planetary-data-cloud#69: https://github.com/NASA-PDS/planetary-data-cloud/issues/69
.. _planetary-data-cloud#71: https://github.com/NASA-PDS/planetary-data-cloud/issues/71
.. _planetary-data-cloud#90: https://github.com/NASA-PDS/planetary-data-cloud/issues/90
.. _planetary-data-cloud#91: https://github.com/NASA-PDS/planetary-data-cloud/issues/91
.. _planetary-data-cloud#76: https://github.com/NASA-PDS/planetary-data-cloud/issues/76
.. _planetary-data-cloud#77: https://github.com/NASA-PDS/planetary-data-cloud/issues/77
.. _planetary-data-cloud#79: https://github.com/NASA-PDS/planetary-data-cloud/issues/79
.. _planetary-data-cloud#72: https://github.com/NASA-PDS/planetary-data-cloud/issues/72
.. _planetary-data-engine#5: https://github.com/NASA-PDS/planetary-data-engine/issues/5
.. _planetary-data-engine#7: https://github.com/NASA-PDS/planetary-data-engine/issues/7
.. _portal-wp-tasks#44: https://github.com/NASA-PDS/portal-wp-tasks/issues/44
.. _portal-wp-tasks#49: https://github.com/NASA-PDS/portal-wp-tasks/issues/49
.. _portal-wp-tasks#56: https://github.com/NASA-PDS/portal-wp-tasks/issues/56
.. _registry#155: https://github.com/NASA-PDS/registry/issues/155
.. _registry#178: https://github.com/NASA-PDS/registry/issues/178
.. _registry#231: https://github.com/NASA-PDS/registry/issues/231
.. _registry#258: https://github.com/NASA-PDS/registry/issues/258
.. _registry#234: https://github.com/NASA-PDS/registry/issues/234
.. _registry#176: https://github.com/NASA-PDS/registry/issues/176
.. _registry-api#389: https://github.com/NASA-PDS/registry-api/issues/389
.. _registry-api#387: https://github.com/NASA-PDS/registry-api/issues/387
.. _registry-api#388: https://github.com/NASA-PDS/registry-api/issues/388
.. _registry-api#404: https://github.com/NASA-PDS/registry-api/issues/404
.. _registry-api#352: https://github.com/NASA-PDS/registry-api/issues/352
.. _registry-api#411: https://github.com/NASA-PDS/registry-api/issues/411
.. _registry-common#40: https://github.com/NASA-PDS/registry-common/issues/40
.. _registry-harvest-legacy#8: https://github.com/NASA-PDS/registry-harvest-legacy/issues/8
.. _registry-mgr-legacy#42: https://github.com/NASA-PDS/registry-mgr-legacy/issues/42
.. _registry-mgr-legacy#49: https://github.com/NASA-PDS/registry-mgr-legacy/issues/49
.. _registry-mgr-legacy#17: https://github.com/NASA-PDS/registry-mgr-legacy/issues/17
.. _registry-pds3-catalog#4: https://github.com/NASA-PDS/registry-pds3-catalog/issues/4
.. _registry-pds3-catalog#6: https://github.com/NASA-PDS/registry-pds3-catalog/issues/6
.. _registry-sweepers#86: https://github.com/NASA-PDS/registry-sweepers/issues/86
.. _registry-sweepers#111: https://github.com/NASA-PDS/registry-sweepers/issues/111
.. _registry-sweepers#109: https://github.com/NASA-PDS/registry-sweepers/issues/109
.. _registry-sweepers#92: https://github.com/NASA-PDS/registry-sweepers/issues/92
.. _roundup-action#136: https://github.com/NASA-PDS/roundup-action/issues/136
.. _roundup-action#124: https://github.com/NASA-PDS/roundup-action/issues/124
.. _search-ui-legacy#7: https://github.com/NASA-PDS/search-ui-legacy/issues/7
.. _search-ui-legacy#1: https://github.com/NASA-PDS/search-ui-legacy/issues/1
.. _software-issues-repo#67: https://github.com/NASA-PDS/software-issues-repo/issues/67
.. _software-issues-repo#80: https://github.com/NASA-PDS/software-issues-repo/issues/80
.. _software-issues-repo#93: https://github.com/NASA-PDS/software-issues-repo/issues/93
.. _software-issues-repo#54: https://github.com/NASA-PDS/software-issues-repo/issues/54
.. _software-issues-repo#49: https://github.com/NASA-PDS/software-issues-repo/issues/49
.. _transform#30: https://github.com/NASA-PDS/transform/issues/30
.. _transform#45: https://github.com/NASA-PDS/transform/issues/45
.. _transform#67: https://github.com/NASA-PDS/transform/issues/67
.. _transform#46: https://github.com/NASA-PDS/transform/issues/46
.. _validate#695: https://github.com/NASA-PDS/validate/issues/695
.. _validate#833: https://github.com/NASA-PDS/validate/issues/833
.. _validate#432: https://github.com/NASA-PDS/validate/issues/432
.. _validate#761: https://github.com/NASA-PDS/validate/issues/761
.. _validate#763: https://github.com/NASA-PDS/validate/issues/763
.. _validate#809: https://github.com/NASA-PDS/validate/issues/809
.. _validate#754: https://github.com/NASA-PDS/validate/issues/754
.. _validate#750: https://github.com/NASA-PDS/validate/issues/750
.. _validate#739: https://github.com/NASA-PDS/validate/issues/739
.. _validate#781: https://github.com/NASA-PDS/validate/issues/781
.. _validate#760: https://github.com/NASA-PDS/validate/issues/760
.. _validate#475: https://github.com/NASA-PDS/validate/issues/475
.. _validate#681: https://github.com/NASA-PDS/validate/issues/681
.. _validate#698: https://github.com/NASA-PDS/validate/issues/698
.. _validate#747: https://github.com/NASA-PDS/validate/issues/747
.. _validate#427: https://github.com/NASA-PDS/validate/issues/427
.. _validate#723: https://github.com/NASA-PDS/validate/issues/723
.. _validate#785: https://github.com/NASA-PDS/validate/issues/785
.. _validate#748: https://github.com/NASA-PDS/validate/issues/748
.. _validate#854: https://github.com/NASA-PDS/validate/issues/854
.. _validate#741: https://github.com/NASA-PDS/validate/issues/741
.. _validate#755: https://github.com/NASA-PDS/validate/issues/755
.. _validate#308: https://github.com/NASA-PDS/validate/issues/308
.. _validate#773: https://github.com/NASA-PDS/validate/issues/773
.. _web-analytics#21: https://github.com/NASA-PDS/web-analytics/issues/21
.. _pds-swg_26: https://github.com/NASA-PDS/pds-swg/issues/26
.. _Software Release Summary (B14.1): https://nasa-pds.github.io/releases/14.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md