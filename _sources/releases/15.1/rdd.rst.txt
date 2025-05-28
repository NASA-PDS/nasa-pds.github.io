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

+-------------------------------+----------------------------------------------------------------------------------------------------+
| Ref                           | Title                                                                                              |
+===============================+====================================================================================================+
| `pds4-information-model#891`_ | CCB-43: Repair Incorrectly Formed Enumerated Value for Units_of_Gmass                              |
+-------------------------------+----------------------------------------------------------------------------------------------------+
| `pds4-information-model#907`_ | CCB-54: Allow comment for DD_Class                                                                 |
+-------------------------------+----------------------------------------------------------------------------------------------------+
| `pds4-information-model#910`_ | CCB-55: Funding_Ackowledgement class enhancement (funding_source and funding_acknowledgement_text) |
+-------------------------------+----------------------------------------------------------------------------------------------------+
| `pds4-information-model#912`_ | CCB-13 Ensure file_name and directory_path_name adhere to SR                                       |
+-------------------------------+----------------------------------------------------------------------------------------------------+

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
`data-upload-manager#151`_ Improve DUM Deployment Automation, Data Replication, and Monitoring
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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

+-------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================================================================+=================+===========================+
| `deep-archive#202`_ pds-deep-registry-archive produces incomplete SIPs for data recently uploaded to the Registry | |:blue_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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

+---------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                                             | I&T Status       | Priority / Bug Severity   |
+===================================================================================================================================================+==================+===========================+
| `devops#77`_ As a developer and tester, I want my test case to be automatically defined from the github ticket without manual editing, copy/paste | |:green_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

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

+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================+===================+===========================+
| `ds-view#14`_ Memory leak in Solr connections leading to Tomcat crash                 | |:blue_circle:|   | s.high                    |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `ds-view#43`_ `viewProfile.jsp` not grabbing latest metadata when data set is updated | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `ds-view#40`_ Products with multiple resources are not appearing on landing pages     | |:green_circle:|  | s.high                    |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `ds-view#45`_ `ds-view` is unexpectedly replacing `=` with `:` in resource URLs       | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                        | I&T Status       | Priority / Bug Severity   |
+==============================================================================+==================+===========================+
| `ds-view#39`_ As a user, I want a landing page for Telescope context objects | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------+------------------+---------------------------+
| `ds-view#38`_ As a user, I want a landing page for Facility context objects  | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================+=================+===========================+
| `ds-view#42`_ Update to improve ordering based upon indexed order | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------+-----------------+---------------------------+

--------

Edwg
----
*PDS Editorial Working Group Working Area*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/EdWG#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/EdWG>`_
     - `Issue Tracking <https://github.com/NASA-PDS/EdWG/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/EdWG/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/EdWG/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/EdWG/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`EdWG#38`_ Context Updates Phase 1: Investigations
++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`EdWG#41`_ Context Updates Phase 1: Instrument Hosts
++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`EdWG#44`_ Context Updates Phase 1: Instruments
+++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------+-------------------+---------------------------+
| Issue                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================+===================+===========================+
| `EdWG#55`_ Context product missing from Working directory | |:blue_circle:|   | s.high                    |
+-----------------------------------------------------------+-------------------+---------------------------+
| `EdWG#57`_ Modification_Detail out of order               | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------+-------------------+---------------------------+

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
`harvest#209`_ Harvest Performance Improvements to Support Big Data Use Cases
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================================================+===================+===========================+
| `harvest#204`_ OpenSearch mapping conflict issue when trying to change a type (`[illegal_argument_exception]`)   | |:yellow_circle:| | s.critical                |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#231`_ harvest stops after [ERROR] (HarvestCli.java:runCommand:98) Object builders can only be used once | |:green_circle:|  | s.critical                |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#229`_ harvest it fails to load org.slf4j.impl.StaticLoggerBinder                                        | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#186`_ New records harvested in the registry don't have the expected Node value                          | |:green_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#208`_ Read time out errors occurring with big data uploads                                              | |:blue_circle:|   | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#190`_ I want to update the OpenSearch schema whatever the number of fields to be updated                | |:blue_circle:|   | s.critical                |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#206`_ Issues identified with uncaught throttling errors                                                 | |:blue_circle:|   | s.high                    |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#222`_ Issue with ALT LDD date format error                                                              | |:blue_circle:|   | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#213`_ harvest by default overwrites all products                                                        | |:green_circle:|  | s.critical                |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#197`_ Unknown date format used that could not be parsed by Harvest                                      | |:green_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                       | I&T Status       | Priority / Bug Severity   |
+=============================================================================================================================+==================+===========================+
| `harvest#199`_ As a user, I want harvest to exit with non 0 code when the arguments are not parsable                        | |:green_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `harvest#187`_ As a user, I want to include my organization name in the harvest metadata (`ops:Harvest_Info.ops:node_name`) | |:green_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================================================+=================+===========================+
| `harvest#223`_ Quiet Harvest noisy logs for Invalid cookie header                                   | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `harvest#203`_ Add the date time in the log messages                                                | |:blue_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `harvest#227`_ Disable graceful handling of missing schema configs with `keyword` data type         | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `harvest#205`_ Optimize LDD downloads also on errors                                                | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `harvest#207`_ Update harvest to support batches with data volumes larger than AOSS allowable limit | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
Requirements
++++++++++++

+--------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                              | I&T Status      | Priority / Bug Severity   |
+====================================================================+=================+===========================+
| `mi-label#84`_ As a user, I want to provide metadata in JSON files | |:blue_circle:| | p.should-have             |
+--------------------------------------------------------------------+-----------------+---------------------------+

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
`nucleus#123`_ Web based Cognito authentication for Nucleus Airflow UI
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`nucleus#130`_ Update Product-Level DAG with Upgraded Harvest
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`nucleus#131`_ Update Architecture and Implement Separate EFS Per Node Baseline DAG
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================================================+===================+===========================+
| `nucleus#143`_ Nucleus workflow validation task failed to find compressed data files that are not .fits files | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================+===================+===========================+
| `nucleus#46`_ As a data provider, I want to deliver cloud-native data to Nucleus      | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+
| `nucleus#141`_ As a user, I want to process a backlog of data present in an S3 bucket | |:green_circle:|  | p.must-have               |
+---------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`operations#562`_ Complete Testing of Upgrade for all EC2 Operating Systems
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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
`pds4-information-model#833`_ B15.1 Information Model SCR Implementation and LDDTool Updates
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#862`_ B15.1 SCR Freeze
++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#863`_ B15.1 Information Model Delivery to I&T
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#864`_ B15.1 Standards Documents Updates
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================+===================+===========================+
| `pds4-information-model#852`_ Issue trying to generate schemas 1E00 and 1D00                                    | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#857`_ Exit codes no longer working as expected                                          | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#859`_ `-V` flag does not work when attempting to generate core IM                       | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#834`_ emrsp namespaces are configured to be produced as https:                          | |:blue_circle:|   | s.high                    |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#848`_ lddtool -v creates/overwrites output directory and files                          | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#846`_ Download links broken for lddtool for online documentation                        | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#723`_ lddtool json export seems to export the whole IM, not just the current dictionary | |:blue_circle:|   | unknown                   |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#867`_ LDDTool does not propertly generate the All LDD Data Dictionary                   | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#866`_ Unable to run >1 cucumber test with LDDs                                          | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#874`_ lddtool `-V` flag outputs invalid schemas for 1C00                                | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#849`_ lddtool -h returns expected information twice and then error messages             | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#822`_ Tests fail when there are multiple tests with multiple schemas/schematrons        | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#885`_ lddtool -V flag outputs invalid schemas for 1D00                                  | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                            | I&T Status       | Priority / Bug Severity   |
+==================================================================================================================================+==================+===========================+
| `pds4-information-model#907`_ CCB-54: Allow comment for DD_Class                                                                 | |:green_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#860`_ As a user, I want to generate the core PDS4 IM for a specific version of PDS4                      | |:green_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#910`_ CCB-55: Funding_Ackowledgement class enhancement (funding_source and funding_acknowledgement_text) | |:green_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#891`_ CCB-43: Repair Incorrectly Formed Enumerated Value for Units_of_Gmass                              | |:green_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#912`_ CCB-13 Ensure file_name and directory_path_name adhere to SR                                       | |:green_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                      | I&T Status      | Priority / Bug Severity   |
+============================================================================================================+=================+===========================+
| `pds4-information-model#845`_ [namespace-registry] add new namespace `LCROSS`                              | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#882`_ [namespace-registry] add new namespace sln, slim, hisaki, and mmx            | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#825`_ Add `Product_Native` test case for #795 back to test suite                   | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#872`_ Archive all PDS Policy documents                                             | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#906`_ [namespace-registry] add new JAXA namespaces for BepiColombo MMO instruments | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#876`_ [namespace-registry] add new namespaces for vex, smart1, and giotto          | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#861`_ Update command-line arguments to be in line with standard best practices     | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Peppi
-----
*Planetary Data Explorer: Python (PEPPi) client library (pds.peppi) to access Planetary Data from the NASA Planetary Data System*

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
`peppi#52`_ PEPPi Refactoring and Documentation to support 2-3 User Support Demos
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`peppi#53`_ Prep for AGU Training Workshop
++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                   | I&T Status       | Priority / Bug Severity   |
+=========================================================================================================+==================+===========================+
| `peppi#30`_ As a user, I want to search for products based upon a investigation LID                     | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#64`_ As a user, I want to limit the number of fields returned                                    | |:green_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#32`_ As a user, I want to search for observational products only                                 | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#31`_ As a user, I want to search for products based upon a instrument LID                        | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#34`_ As a user, I want to search for bundle products only                                        | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#60`_ As a user, I want to transform binary tables (.dat) in CSVs for all members of a collection | |:green_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#47`_ As a user, I want to see an online reference documentation of the library                   | |:green_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#57`_ As a user, I want my query response as a Pandas DataFrame                                   | |:green_circle:| | p.could-have              |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#63`_ As a developer, I want to install pds.peppi in a conda environment                          | |:green_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#74`_ As a user, I want to find products with a target given as a string                          | |:green_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#35`_ As a user, I want to filter on a specific processing level                                  | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#61`_ As a user, I want to read all tables within a collection into a pandas DataFrame            | |:green_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `peppi#33`_ As a user, I want to search for collection products only                                    | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------+------------------+---------------------------+

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
`planetary-data-cloud#74`_ [SBN CATCH Migration] Support Development of Initial Migration Plan and Architecture
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                         | I&T Status        | Level       | Priority / Bug Severity   |
+===============================================================================================================================================================+===================+=============+===========================+
| `planetary-data-cloud#121`_ Phase 1: PDS-EN to provide codeql scan for SBN to incorporate.  Review any questions at next SBN cloud migration tagup (11/22/24) | |:yellow_circle:| | enhancement | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `planetary-data-cloud#122`_ Phase 1: PDS-EN to provide terraform templates for SBN to capture the current status of CATCH.                                    | |:yellow_circle:| | enhancement | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `planetary-data-cloud#123`_ Phase 1: PDS-EN to provide cloud endpoint for SBN to integrate the endpoint into SBN Survey Image Service.                        | |:blue_circle:|   | enhancement | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`planetary-data-cloud#80`_ Develop PDC Tenant Roles
+++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#112`_ Refine Data Backup, Disaster Recovery and Configuration Management Plans
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#119`_ Document Test Venue Strategies and Level of Service
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#124`_ Review SMD Cost Model, Develop Additional Requirements, and Refine FY25 Cost Model
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#126`_ ATLAS MVP: Big Data Migration Trade Study
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#129`_ B15.1 Bi-annual Cloud Resource Housekeeping
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                           | I&T Status       | Priority / Bug Severity   |
+=================================================================================================================================+==================+===========================+
| `planetary-data-cloud#125`_ CSS ODR bucket no longer accessible to the public                                                   | |:green_circle:| | s.critical                |
+---------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `planetary-data-cloud#143`_ ODR bucket is missing the initial CSS data that was loaded by SBN-PSI prior to the existence of ODR | |:blue_circle:|  | s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================================================================================================+=================+===========================+
| `planetary-data-cloud#75`_ As a user, I want a warm backup of my archive data to be available in the event of corruption of of primary archive data | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `planetary-data-cloud#131`_ As a cloud user, I want to create a new S3 bucket in Dev venue                                                          | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                  | I&T Status      | Priority / Bug Severity   |
+========================================================================================+=================+===========================+
| `planetary-data-cloud#128`_ Setup Budgets and Reporting for all accounts               | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------------------------------+-----------------+---------------------------+
| `planetary-data-cloud#140`_ Review data backups and remove data that we no longer need | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`portal-tasks#108`_ Create 2025 Data Release Calendar
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================================================================================+===================+===========================+
| `portal-tasks#109`_ Tool Registry doesn't work for text searches                                                            | |:blue_circle:|   | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#107`_ Missing PDS4_IMG_1100.xsd                                                                               | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#103`_ `Browse and search` link broken on https://pds.nasa.gov/datastandards/dictionaries/index-missions.shtml | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#102`_ tool registry search result count is incorrect                                                          | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#104`_ Tool Registry search does not work past initial query                                                   | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#105`_ Missing PDS4_LCROSS_1E00_1100.JSON                                                                      | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `portal-tasks#106`_ Missing PDS4_MSN_SURFACE_1A10.xsd                                                                       | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                               | I&T Status       | Priority / Bug Severity   |
+=====================================================================================================+==================+===========================+
| `portal-tasks#117`_ Invalid dates in LDD JSON files causing read errors in Harvest                  | |:green_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `portal-tasks#115`_ Remove phonebook from portal                                                    | |:blue_circle:|  | unknown                   |
+-----------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `portal-tasks#116`_ Update PDS Data Dictionaries page to include links to the WebHelp documentation | |:blue_circle:|  | unknown                   |
+-----------------------------------------------------------------------------------------------------+------------------+---------------------------+

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

+------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                          | I&T Status       | Priority / Bug Severity   |
+================================================================================================+==================+===========================+
| `portal-wp#147`_ Data Sets are linking to viewCollection pages, not the resLocation            | |:green_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `portal-wp#139`_ Page Type value in search results does not match actual page_type field value | |:blue_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `portal-wp#72`_ Search results are linking to an empty page (`investigations/identifier/data`) | |:green_circle:| | s.critical                |
+------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `portal-wp#145`_ Search strings containing a slash "/" character fail                          | |:green_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------+------------------+---------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                              | I&T Status       | Priority / Bug Severity   |
+====================================================================================================================+==================+===========================+
| `portal-wp#119`_ As a user, I want to select 1 or more filters to facet search results                             | |:blue_circle:|  | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `portal-wp#87`_ As a user, I want collection descriptions to default to `pds:Citation_Information.pds:description` | |:green_circle:| | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                        | I&T Status      | Priority / Bug Severity   |
+==============================================================================+=================+===========================+
| `portal-wp#107`_ Test instructions for running WST Drupal Site               | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------+-----------------+---------------------------+
| `portal-wp#97`_ Add State to Homepage for what has been selected             | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------------+-----------------+---------------------------+
| `portal-wp#129`_ Update facets and search results to enable sorting by title | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------+-----------------+---------------------------+

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
`registry#338`_ Re-index All Registries For All Fields to be Searchable
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry#345`_ B15.1 Registry Maintenance: High Priority Enhancements / Bug Fixes / Tasks
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry#346`_ Formalize and Scrub all Registry Documentation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry#348`_ Update Registry AOSS Auth Layer To Enable Read-only Access to All Registries
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                     | I&T Status       | Priority / Bug Severity   |
+===========================================================================================+==================+===========================+
| `registry#340`_ Getting "blocked by: maximum OCU capacity reached" errors when harvesting | |:blue_circle:|  | s.critical                |
+-------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#329`_ AOSS 500/502 responses repeatedly observed under heavy load               | |:blue_circle:|  | s.high                    |
+-------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#365`_ Update terraform to use port 443 not port 80                              | |:green_circle:| | s.critical                |
+-------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#351`_ Data products duplicated across en-registry and other node registries     | |:green_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#331`_ GEO index does not work, appears to be corrupted                          | |:blue_circle:|  | s.critical                |
+-------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#369`_ Registry return authorization error for ATM node                          | |:green_circle:| | s.critical                |
+-------------------------------------------------------------------------------------------+------------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                              | I&T Status       | Priority / Bug Severity   |
+====================================================================================+==================+===========================+
| `registry#350`_ As a user, I want to have read-only access to all registry indexes | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                              | I&T Status        | Priority / Bug Severity   |
+====================================================================================+===================+===========================+
| `registry#352`_ Recreate PDS EN Registry from scratch and load only necessary data | |:blue_circle:|   | p.must-have               |
+------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry#361`_ Document the refresh rate of OpenSearch                            | |:yellow_circle:| | p.should-have             |
+------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`registry-api#285`_ Design and Implement Faceting
+++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry-api#549`_ Implement additional formats from previous version of API (pds4+xml, pds4+json)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry-api#559`_ B15.1 API Maintenance: Must-have / Should-have Enhancements and Bug Fixes
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================+===================+===========================+
| `registry-api#548`_ Responses do not return correct metadata when `fields` parameter is specified | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#616`_ Registry API returning >1 version of data                                     | |:green_circle:|  | s.critical                |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#634`_ Fix broken branch testing                                                     | |:blue_circle:|   | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                      | I&T Status        | Priority / Bug Severity   |
+============================================================================================================================================================+===================+===========================+
| `registry-api#575`_ As application support, I want to see in the server side logs the full query being sent to OpenSearch                                  | |:yellow_circle:| | p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#450`_ As a user, I want to receive a JSON response that contains the PDS4 label metadata in JSON format (application/vnd.nasa.pds.pds4+json) | |:green_circle:|  | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#440`_ As a user, I want to receive a XML response that contains the PDS4 label metadata in XML format (application/vnd.nasa.pds.pds4+xml)    | |:green_circle:|  | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#283`_ As a client developer, I want to facet on 1 or more fields in the registry                                                             | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================================================================+=================+===========================+
| `registry-common#83`_ As a Nucleus system, I want to be able to invoke harvest and registry-mgr from within the AWS VPC | |:blue_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------+-----------------+---------------------------+
| Issue                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================+=================+===========================+
| `registry-common#118`_ Cleanup potential resource leaks | |:blue_circle:| | unknown                   |
+---------------------------------------------------------+-----------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================================+===================+===========================+
| `registry-legacy-solr#154`_ viewDocument.jsp has no links for SEARCH/ACCESS DATA                                  | |:green_circle:|  | s.high                    |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#184`_ NullPointerException being thrown and catalog-solr is not completing execution        | |:green_circle:|  | s.critical                |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#163`_ Cassini ISS Users Guide returns "No Document Information found in the registry" msg   | |:green_circle:|  | s.high                    |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#176`_ SIP_Deep_Archive products showing up in search results                                | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#174`_ Harvest ignoring secondary members of collections managed by EN                       | |:yellow_circle:| | unknown                   |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#204`_ Bug introduced when supporting product external and missing resource_refs             | |:blue_circle:|   | s.high                    |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#172`_ Possible memory leak related to use of Solr library per `Direct buffer memory` errors | |:blue_circle:|   | s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#156`_ viewDataset.jsp shows no links for Search/Access Data                                 | |:green_circle:|  | s.high                    |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-legacy-solr#147`_ `page_type` not working for context products                                          | |:blue_circle:|   | s.critical                |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                   | I&T Status       | Priority / Bug Severity   |
+=========================================================================================================================+==================+===========================+
| `registry-legacy-solr#179`_ As a user, I want to provide a data input path via command-line                             | |:green_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry-legacy-solr#93`_ As a user, I want to provide search/access links using the hsk.cat files within the data set | |:green_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                       | I&T Status      | Priority / Bug Severity   |
+=============================================================================================+=================+===========================+
| `registry-legacy-solr#158`_ Add single-value title and context name field to enable sorting | |:blue_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------+-----------------+---------------------------+

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

+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                  | I&T Status        | Priority / Bug Severity   |
+========================================================================================================================+===================+===========================+
| `registry-mgr#122`_ `[ERROR] Need to fill this out when have a return value` when trying to execute `list-dd` command  | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-mgr#121`_ `Missing required property 'FieldValue.<variant value>'` error when running with `list-dd` command | |:green_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-mgr#104`_ Update inline help to match latest features                                                        | |:green_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-mgr#124`_ Getting null message in log with option packageId                                                  | |:yellow_circle:| | s.low                     |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-mgr#131`_ registry-manager does not process _all_ collections in a bundle                                    | |:green_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-mgr#111`_ registry-mgr return ERROR null                                                                     | |:blue_circle:|   | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-mgr#109`_ archive status does not change for all bundle members                                              | |:green_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                                      | I&T Status       | Priority / Bug Severity   |
+============================================================================================================================================+==================+===========================+
| `registry-mgr#113`_ As a user, I want to change the archive status for a collection and it's associated products given a collection lidvid | |:green_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry-mgr#112`_ As a user, I want to update a bundle and associated collections' and products' archive status given a bundle lidvid    | |:green_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------+-----------------+---------------------------+
| Issue                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================+=================+===========================+
| `registry-mgr#117`_ Quiet SLF4J log message from end user | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------+-----------------+---------------------------+

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
`registry-sweepers#147`_ Deploy Registry Sweeper Task using EventBridge in Prod
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-----------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================+=================+===========================+
| `registry-sweepers#156`_ Finalize deployment of sweeper in production | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------+-----------------+---------------------------+

--------

S3-browser-cloudfront
---------------------
*Web view for files in S3 buckets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/s3-browser-cloudfront#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/s3-browser-cloudfront>`_
     - `Issue Tracking <https://github.com/NASA-PDS/s3-browser-cloudfront/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/s3-browser-cloudfront/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/s3-browser-cloudfront/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/s3-browser-cloudfront/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`s3-browser-cloudfront#29`_ Deploy S3 Browser to Test and Prod
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                | I&T Status       | Priority / Bug Severity   |
+======================================================================+==================+===========================+
| `s3-browser-cloudfront#131`_ Resolve broken icon links in file pages | |:green_circle:| | s.medium                  |
+----------------------------------------------------------------------+------------------+---------------------------+

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
`software-issues-repo#110`_ B15.1 Code Freeze
+++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#111`_ B15.1 Prep for I&T
++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#115`_ B15.1 Bi-Annual Triage Static Code Analysis Scan Results
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#116`_ 2025 Annual Contingency Plan Review and Test
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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

`system-i-n-t#60`_ B15.1 Test Readiness Review (TRR)
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
`validate#1011`_ B15.1 High Priority Bug Fixes and Missing Standards Implementations
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#1053`_ Update `validate-refs` per new Registry Architecture
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================================================+===================+===========================+
| `validate#1118`_ JPEG validation does not allow JPEG files with trailers                                         | |:green_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1058`_ validate cucumber testing is not exercising all tests as it should be                           | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1135`_ Min/Max value check does not handle ASCII_Time_* Strings                                        | |:green_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1130`_ Min/Max value check does not handle ASCII_Numeric_Base16 values                                 | |:green_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1100`_ validate's PDS4 Bundle Level Validation Results are wrong if filenames end in XML               | |:green_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1066`_ Telescopes missing from registry context products config                                        | |:green_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1183`_ validate-refs appears to be validating many more products than the input LIDVID                 | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1105`_ Validate does not work for multiple executions with LDDs in the same Java run                   | |:blue_circle:|   | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1008`_ The PDF verification / VeraPDF component of Validate seems to error on Windows paths            | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1090`_ Validate run with --skip-product-validation reports product success in log                      | |:green_circle:|  | s.low                     |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1158`_ Context object name check does not match against latest version of context object               | |:green_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1157`_ Fix failing integration tests                                                                   | |:blue_circle:|   | unknown                   |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1019`_ Configuration file documenation does not match actual config file options                       | |:blue_circle:|   | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1210`_ JP2 as encoding standard id still throws and error                                              | |:blue_circle:|   | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1028`_ validate incorrectly disallows Encoded_Native/encoding_standard_id = 'SEED 2.4'                 | |:green_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#979`_ OutOfMemoryError when NASA validate v3.5.2 is executed through a library for a batch of products | |:blue_circle:|   | s.medium                  |
+------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                                       | I&T Status       | Priority / Bug Severity   |
+=============================================================================================================================================+==================+===========================+
| `validate#992`_ As a user, I want to validate that there is exactly one digit to the left of the decimal point for the specifier `e` or `E` | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#1104`_ As a user, I want to support the JP2 as an acceptable file extension per the PDS4 standards                                | |:green_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================================================+===================+===========================+
| `validate#1085`_ Improve error handling for Registry connection issues                                        | |:blue_circle:|   | unknown                   |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1102`_ Reformat cucumber feature files to be more succinct                                          | |:blue_circle:|   | unknown                   |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1129`_ Add new `encoding_standard_id` values for `Encoded_Byte_Stream` quality check                | |:green_circle:|  | p.must-have               |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#621`_ Upgrade validate-refs to work with new AOSS registry                                          | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1147`_ Deprecate `validate.checkInbetweenFields` and add `validate.strictFieldChecks` as synonymous | |:blue_circle:|   | unknown                   |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

`web-modernization#246`_ Refine Designs and Implement Improved Faceting
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`web-modernization#248`_ Refine UI Implementation Based Upon Must-Have User Feedback on Beta
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`web-modernization#251`_ Finalize Investigation Deep Dive Content Pages
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-----------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================================+=================+===========================+
| `web-modernization#241`_ Specify Image Requirements for the Various Landing Pages | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------------------+-----------------+---------------------------+

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
.. _pds4-information-model#891: https://github.com/NASA-PDS/pds4-information-model/issues/891
.. _pds4-information-model#907: https://github.com/NASA-PDS/pds4-information-model/issues/907
.. _pds4-information-model#910: https://github.com/NASA-PDS/pds4-information-model/issues/910
.. _pds4-information-model#912: https://github.com/NASA-PDS/pds4-information-model/issues/912
.. _data-upload-manager#151: https://github.com/NASA-PDS/data-upload-manager/issues/151
.. _deep-archive#202: https://github.com/NASA-PDS/deep-archive/issues/202
.. _devops#69: https://github.com/NASA-PDS/devops/issues/69
.. _devops#78: https://github.com/NASA-PDS/devops/issues/78
.. _devops#77: https://github.com/NASA-PDS/devops/issues/77
.. _ds-view#14: https://github.com/NASA-PDS/ds-view/issues/14
.. _ds-view#43: https://github.com/NASA-PDS/ds-view/issues/43
.. _ds-view#40: https://github.com/NASA-PDS/ds-view/issues/40
.. _ds-view#45: https://github.com/NASA-PDS/ds-view/issues/45
.. _ds-view#39: https://github.com/NASA-PDS/ds-view/issues/39
.. _ds-view#38: https://github.com/NASA-PDS/ds-view/issues/38
.. _ds-view#42: https://github.com/NASA-PDS/ds-view/issues/42
.. _EdWG#38: https://github.com/NASA-PDS/EdWG/issues/38
.. _EdWG#41: https://github.com/NASA-PDS/EdWG/issues/41
.. _EdWG#44: https://github.com/NASA-PDS/EdWG/issues/44
.. _EdWG#55: https://github.com/NASA-PDS/EdWG/issues/55
.. _EdWG#57: https://github.com/NASA-PDS/EdWG/issues/57
.. _harvest#209: https://github.com/NASA-PDS/harvest/issues/209
.. _harvest#204: https://github.com/NASA-PDS/harvest/issues/204
.. _harvest#231: https://github.com/NASA-PDS/harvest/issues/231
.. _harvest#229: https://github.com/NASA-PDS/harvest/issues/229
.. _harvest#186: https://github.com/NASA-PDS/harvest/issues/186
.. _harvest#208: https://github.com/NASA-PDS/harvest/issues/208
.. _harvest#190: https://github.com/NASA-PDS/harvest/issues/190
.. _harvest#206: https://github.com/NASA-PDS/harvest/issues/206
.. _harvest#222: https://github.com/NASA-PDS/harvest/issues/222
.. _harvest#213: https://github.com/NASA-PDS/harvest/issues/213
.. _harvest#197: https://github.com/NASA-PDS/harvest/issues/197
.. _harvest#199: https://github.com/NASA-PDS/harvest/issues/199
.. _harvest#187: https://github.com/NASA-PDS/harvest/issues/187
.. _harvest#223: https://github.com/NASA-PDS/harvest/issues/223
.. _harvest#203: https://github.com/NASA-PDS/harvest/issues/203
.. _harvest#227: https://github.com/NASA-PDS/harvest/issues/227
.. _harvest#205: https://github.com/NASA-PDS/harvest/issues/205
.. _harvest#207: https://github.com/NASA-PDS/harvest/issues/207
.. _mi-label#84: https://github.com/NASA-PDS/mi-label/issues/84
.. _nucleus#123: https://github.com/NASA-PDS/nucleus/issues/123
.. _nucleus#130: https://github.com/NASA-PDS/nucleus/issues/130
.. _nucleus#131: https://github.com/NASA-PDS/nucleus/issues/131
.. _nucleus#143: https://github.com/NASA-PDS/nucleus/issues/143
.. _nucleus#46: https://github.com/NASA-PDS/nucleus/issues/46
.. _nucleus#141: https://github.com/NASA-PDS/nucleus/issues/141
.. _nucleus#121: https://github.com/NASA-PDS/nucleus/issues/121
.. _operations#562: https://github.com/NASA-PDS/operations/issues/562
.. _pds4-information-model#833: https://github.com/NASA-PDS/pds4-information-model/issues/833
.. _pds4-information-model#862: https://github.com/NASA-PDS/pds4-information-model/issues/862
.. _pds4-information-model#863: https://github.com/NASA-PDS/pds4-information-model/issues/863
.. _pds4-information-model#864: https://github.com/NASA-PDS/pds4-information-model/issues/864
.. _pds4-information-model#852: https://github.com/NASA-PDS/pds4-information-model/issues/852
.. _pds4-information-model#857: https://github.com/NASA-PDS/pds4-information-model/issues/857
.. _pds4-information-model#859: https://github.com/NASA-PDS/pds4-information-model/issues/859
.. _pds4-information-model#834: https://github.com/NASA-PDS/pds4-information-model/issues/834
.. _pds4-information-model#848: https://github.com/NASA-PDS/pds4-information-model/issues/848
.. _pds4-information-model#846: https://github.com/NASA-PDS/pds4-information-model/issues/846
.. _pds4-information-model#723: https://github.com/NASA-PDS/pds4-information-model/issues/723
.. _pds4-information-model#867: https://github.com/NASA-PDS/pds4-information-model/issues/867
.. _pds4-information-model#866: https://github.com/NASA-PDS/pds4-information-model/issues/866
.. _pds4-information-model#874: https://github.com/NASA-PDS/pds4-information-model/issues/874
.. _pds4-information-model#849: https://github.com/NASA-PDS/pds4-information-model/issues/849
.. _pds4-information-model#822: https://github.com/NASA-PDS/pds4-information-model/issues/822
.. _pds4-information-model#885: https://github.com/NASA-PDS/pds4-information-model/issues/885
.. _pds4-information-model#907: https://github.com/NASA-PDS/pds4-information-model/issues/907
.. _pds4-information-model#860: https://github.com/NASA-PDS/pds4-information-model/issues/860
.. _pds4-information-model#910: https://github.com/NASA-PDS/pds4-information-model/issues/910
.. _pds4-information-model#891: https://github.com/NASA-PDS/pds4-information-model/issues/891
.. _pds4-information-model#912: https://github.com/NASA-PDS/pds4-information-model/issues/912
.. _pds4-information-model#845: https://github.com/NASA-PDS/pds4-information-model/issues/845
.. _pds4-information-model#882: https://github.com/NASA-PDS/pds4-information-model/issues/882
.. _pds4-information-model#825: https://github.com/NASA-PDS/pds4-information-model/issues/825
.. _pds4-information-model#872: https://github.com/NASA-PDS/pds4-information-model/issues/872
.. _pds4-information-model#906: https://github.com/NASA-PDS/pds4-information-model/issues/906
.. _pds4-information-model#876: https://github.com/NASA-PDS/pds4-information-model/issues/876
.. _pds4-information-model#861: https://github.com/NASA-PDS/pds4-information-model/issues/861
.. _peppi#52: https://github.com/NASA-PDS/peppi/issues/52
.. _peppi#53: https://github.com/NASA-PDS/peppi/issues/53
.. _peppi#30: https://github.com/NASA-PDS/peppi/issues/30
.. _peppi#64: https://github.com/NASA-PDS/peppi/issues/64
.. _peppi#32: https://github.com/NASA-PDS/peppi/issues/32
.. _peppi#31: https://github.com/NASA-PDS/peppi/issues/31
.. _peppi#34: https://github.com/NASA-PDS/peppi/issues/34
.. _peppi#60: https://github.com/NASA-PDS/peppi/issues/60
.. _peppi#47: https://github.com/NASA-PDS/peppi/issues/47
.. _peppi#57: https://github.com/NASA-PDS/peppi/issues/57
.. _peppi#63: https://github.com/NASA-PDS/peppi/issues/63
.. _peppi#74: https://github.com/NASA-PDS/peppi/issues/74
.. _peppi#35: https://github.com/NASA-PDS/peppi/issues/35
.. _peppi#61: https://github.com/NASA-PDS/peppi/issues/61
.. _peppi#33: https://github.com/NASA-PDS/peppi/issues/33
.. _planetary-data-cloud#74: https://github.com/NASA-PDS/planetary-data-cloud/issues/74
.. _planetary-data-cloud#121: https://github.com/NASA-PDS/planetary-data-cloud/issues/121
.. _planetary-data-cloud#122: https://github.com/NASA-PDS/planetary-data-cloud/issues/122
.. _planetary-data-cloud#123: https://github.com/NASA-PDS/planetary-data-cloud/issues/123
.. _planetary-data-cloud#80: https://github.com/NASA-PDS/planetary-data-cloud/issues/80
.. _planetary-data-cloud#112: https://github.com/NASA-PDS/planetary-data-cloud/issues/112
.. _planetary-data-cloud#119: https://github.com/NASA-PDS/planetary-data-cloud/issues/119
.. _planetary-data-cloud#124: https://github.com/NASA-PDS/planetary-data-cloud/issues/124
.. _planetary-data-cloud#126: https://github.com/NASA-PDS/planetary-data-cloud/issues/126
.. _planetary-data-cloud#129: https://github.com/NASA-PDS/planetary-data-cloud/issues/129
.. _planetary-data-cloud#125: https://github.com/NASA-PDS/planetary-data-cloud/issues/125
.. _planetary-data-cloud#143: https://github.com/NASA-PDS/planetary-data-cloud/issues/143
.. _planetary-data-cloud#75: https://github.com/NASA-PDS/planetary-data-cloud/issues/75
.. _planetary-data-cloud#131: https://github.com/NASA-PDS/planetary-data-cloud/issues/131
.. _planetary-data-cloud#128: https://github.com/NASA-PDS/planetary-data-cloud/issues/128
.. _planetary-data-cloud#140: https://github.com/NASA-PDS/planetary-data-cloud/issues/140
.. _portal-tasks#108: https://github.com/NASA-PDS/portal-tasks/issues/108
.. _portal-tasks#109: https://github.com/NASA-PDS/portal-tasks/issues/109
.. _portal-tasks#107: https://github.com/NASA-PDS/portal-tasks/issues/107
.. _portal-tasks#103: https://github.com/NASA-PDS/portal-tasks/issues/103
.. _portal-tasks#102: https://github.com/NASA-PDS/portal-tasks/issues/102
.. _portal-tasks#104: https://github.com/NASA-PDS/portal-tasks/issues/104
.. _portal-tasks#105: https://github.com/NASA-PDS/portal-tasks/issues/105
.. _portal-tasks#106: https://github.com/NASA-PDS/portal-tasks/issues/106
.. _portal-tasks#117: https://github.com/NASA-PDS/portal-tasks/issues/117
.. _portal-tasks#115: https://github.com/NASA-PDS/portal-tasks/issues/115
.. _portal-tasks#116: https://github.com/NASA-PDS/portal-tasks/issues/116
.. _portal-wp#147: https://github.com/NASA-PDS/portal-wp/issues/147
.. _portal-wp#139: https://github.com/NASA-PDS/portal-wp/issues/139
.. _portal-wp#72: https://github.com/NASA-PDS/portal-wp/issues/72
.. _portal-wp#145: https://github.com/NASA-PDS/portal-wp/issues/145
.. _portal-wp#119: https://github.com/NASA-PDS/portal-wp/issues/119
.. _portal-wp#87: https://github.com/NASA-PDS/portal-wp/issues/87
.. _portal-wp#107: https://github.com/NASA-PDS/portal-wp/issues/107
.. _portal-wp#97: https://github.com/NASA-PDS/portal-wp/issues/97
.. _portal-wp#129: https://github.com/NASA-PDS/portal-wp/issues/129
.. _registry#338: https://github.com/NASA-PDS/registry/issues/338
.. _registry#345: https://github.com/NASA-PDS/registry/issues/345
.. _registry#346: https://github.com/NASA-PDS/registry/issues/346
.. _registry#348: https://github.com/NASA-PDS/registry/issues/348
.. _registry#340: https://github.com/NASA-PDS/registry/issues/340
.. _registry#329: https://github.com/NASA-PDS/registry/issues/329
.. _registry#365: https://github.com/NASA-PDS/registry/issues/365
.. _registry#351: https://github.com/NASA-PDS/registry/issues/351
.. _registry#331: https://github.com/NASA-PDS/registry/issues/331
.. _registry#369: https://github.com/NASA-PDS/registry/issues/369
.. _registry#350: https://github.com/NASA-PDS/registry/issues/350
.. _registry#352: https://github.com/NASA-PDS/registry/issues/352
.. _registry#361: https://github.com/NASA-PDS/registry/issues/361
.. _registry-api#285: https://github.com/NASA-PDS/registry-api/issues/285
.. _registry-api#549: https://github.com/NASA-PDS/registry-api/issues/549
.. _registry-api#559: https://github.com/NASA-PDS/registry-api/issues/559
.. _registry-api#548: https://github.com/NASA-PDS/registry-api/issues/548
.. _registry-api#616: https://github.com/NASA-PDS/registry-api/issues/616
.. _registry-api#634: https://github.com/NASA-PDS/registry-api/issues/634
.. _registry-api#575: https://github.com/NASA-PDS/registry-api/issues/575
.. _registry-api#450: https://github.com/NASA-PDS/registry-api/issues/450
.. _registry-api#440: https://github.com/NASA-PDS/registry-api/issues/440
.. _registry-api#283: https://github.com/NASA-PDS/registry-api/issues/283
.. _registry-common#83: https://github.com/NASA-PDS/registry-common/issues/83
.. _registry-common#118: https://github.com/NASA-PDS/registry-common/issues/118
.. _registry-legacy-solr#154: https://github.com/NASA-PDS/registry-legacy-solr/issues/154
.. _registry-legacy-solr#184: https://github.com/NASA-PDS/registry-legacy-solr/issues/184
.. _registry-legacy-solr#163: https://github.com/NASA-PDS/registry-legacy-solr/issues/163
.. _registry-legacy-solr#176: https://github.com/NASA-PDS/registry-legacy-solr/issues/176
.. _registry-legacy-solr#174: https://github.com/NASA-PDS/registry-legacy-solr/issues/174
.. _registry-legacy-solr#204: https://github.com/NASA-PDS/registry-legacy-solr/issues/204
.. _registry-legacy-solr#172: https://github.com/NASA-PDS/registry-legacy-solr/issues/172
.. _registry-legacy-solr#156: https://github.com/NASA-PDS/registry-legacy-solr/issues/156
.. _registry-legacy-solr#147: https://github.com/NASA-PDS/registry-legacy-solr/issues/147
.. _registry-legacy-solr#179: https://github.com/NASA-PDS/registry-legacy-solr/issues/179
.. _registry-legacy-solr#93: https://github.com/NASA-PDS/registry-legacy-solr/issues/93
.. _registry-legacy-solr#158: https://github.com/NASA-PDS/registry-legacy-solr/issues/158
.. _registry-mgr#122: https://github.com/NASA-PDS/registry-mgr/issues/122
.. _registry-mgr#121: https://github.com/NASA-PDS/registry-mgr/issues/121
.. _registry-mgr#104: https://github.com/NASA-PDS/registry-mgr/issues/104
.. _registry-mgr#124: https://github.com/NASA-PDS/registry-mgr/issues/124
.. _registry-mgr#131: https://github.com/NASA-PDS/registry-mgr/issues/131
.. _registry-mgr#111: https://github.com/NASA-PDS/registry-mgr/issues/111
.. _registry-mgr#109: https://github.com/NASA-PDS/registry-mgr/issues/109
.. _registry-mgr#113: https://github.com/NASA-PDS/registry-mgr/issues/113
.. _registry-mgr#112: https://github.com/NASA-PDS/registry-mgr/issues/112
.. _registry-mgr#117: https://github.com/NASA-PDS/registry-mgr/issues/117
.. _registry-sweepers#147: https://github.com/NASA-PDS/registry-sweepers/issues/147
.. _registry-sweepers#156: https://github.com/NASA-PDS/registry-sweepers/issues/156
.. _s3-browser-cloudfront#29: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/29
.. _s3-browser-cloudfront#131: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/131
.. _search-ui-legacy#40: https://github.com/NASA-PDS/search-ui-legacy/issues/40
.. _software-issues-repo#110: https://github.com/NASA-PDS/software-issues-repo/issues/110
.. _software-issues-repo#111: https://github.com/NASA-PDS/software-issues-repo/issues/111
.. _software-issues-repo#115: https://github.com/NASA-PDS/software-issues-repo/issues/115
.. _software-issues-repo#116: https://github.com/NASA-PDS/software-issues-repo/issues/116
.. _system-i-n-t#54: https://github.com/NASA-PDS/system-i-n-t/issues/54
.. _system-i-n-t#55: https://github.com/NASA-PDS/system-i-n-t/issues/55
.. _system-i-n-t#60: https://github.com/NASA-PDS/system-i-n-t/issues/60
.. _validate#1011: https://github.com/NASA-PDS/validate/issues/1011
.. _validate#1053: https://github.com/NASA-PDS/validate/issues/1053
.. _validate#1118: https://github.com/NASA-PDS/validate/issues/1118
.. _validate#1058: https://github.com/NASA-PDS/validate/issues/1058
.. _validate#1135: https://github.com/NASA-PDS/validate/issues/1135
.. _validate#1130: https://github.com/NASA-PDS/validate/issues/1130
.. _validate#1100: https://github.com/NASA-PDS/validate/issues/1100
.. _validate#1066: https://github.com/NASA-PDS/validate/issues/1066
.. _validate#1183: https://github.com/NASA-PDS/validate/issues/1183
.. _validate#1105: https://github.com/NASA-PDS/validate/issues/1105
.. _validate#1008: https://github.com/NASA-PDS/validate/issues/1008
.. _validate#1090: https://github.com/NASA-PDS/validate/issues/1090
.. _validate#1158: https://github.com/NASA-PDS/validate/issues/1158
.. _validate#1157: https://github.com/NASA-PDS/validate/issues/1157
.. _validate#1019: https://github.com/NASA-PDS/validate/issues/1019
.. _validate#1210: https://github.com/NASA-PDS/validate/issues/1210
.. _validate#1028: https://github.com/NASA-PDS/validate/issues/1028
.. _validate#979: https://github.com/NASA-PDS/validate/issues/979
.. _validate#992: https://github.com/NASA-PDS/validate/issues/992
.. _validate#1104: https://github.com/NASA-PDS/validate/issues/1104
.. _validate#1085: https://github.com/NASA-PDS/validate/issues/1085
.. _validate#1102: https://github.com/NASA-PDS/validate/issues/1102
.. _validate#1129: https://github.com/NASA-PDS/validate/issues/1129
.. _validate#621: https://github.com/NASA-PDS/validate/issues/621
.. _validate#1147: https://github.com/NASA-PDS/validate/issues/1147
.. _web-modernization#239: https://github.com/NASA-PDS/web-modernization/issues/239
.. _web-modernization#246: https://github.com/NASA-PDS/web-modernization/issues/246
.. _web-modernization#248: https://github.com/NASA-PDS/web-modernization/issues/248
.. _web-modernization#251: https://github.com/NASA-PDS/web-modernization/issues/251
.. _web-modernization#241: https://github.com/NASA-PDS/web-modernization/issues/241
.. _Software Release Summary (B15.1): https://nasa-pds.github.io/releases/15.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md