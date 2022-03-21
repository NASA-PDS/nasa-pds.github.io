===================================================
Release Description Document (build B12.1-SNAPSHOT)
===================================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `Plan B12.1`_

The following sections can be found in this document:

.. toctree::
   :glob: 
   :maxdepth: 3

   rdd.rst

PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

+--------------------------------+----------------------------------------------------------------------------------------------+
|Ref                             |Title                                                                                         |
+================================+==============================================================================================+
|`pds4-information-model#446`_   |CCB-344:  Add data_to_partially_processed_product to reference types for Internal_Reference   |
+--------------------------------+----------------------------------------------------------------------------------------------+
|`pds4-information-model#448`_   |CCB-343: Revise Product_Metadata_Supplemental                                                 |
+--------------------------------+----------------------------------------------------------------------------------------------+
|`pds4-information-model#450`_   |CCB-340 : <Local_Internal_Reference>.<local_identifier_reference> cardinality                 |
+--------------------------------+----------------------------------------------------------------------------------------------+
|`pds4-information-model#453`_   |CCB-335: Inventory Specification Allows Too Many Delimiters                                   |
+--------------------------------+----------------------------------------------------------------------------------------------+

Software Changes
================
The changes types are 'Bug', 'Enhancement' or 'Requirement'. For each software repository, the changes are listed in 2
categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B12.1-SNAPSHOT`_')
The 'Other Updates' occurs during the build cycle witout being planned or attached to a theme. They are organized by
types (bug, enhancements, requirements...). Any updates that require a de-scope of planned tasks are reviewed by the PDS
Software Working Group.

The deliveries are validated by the development team and go through an additional Integration & Test process, as
applicable, as indicated by a specific icon in the following tables.

--------

Cloud-tasks
-----------
*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/cloud-tasks#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/cloud-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/cloud-tasks/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/cloud-tasks/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/cloud-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/cloud-tasks/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `cloud-tasks#3`_ B12.1 pds.nasa.gov Website Lift-and-Shift Pilot Project
    
+-----------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                            |I&T   |Level   |Priority / Bug Severity   |
+=================================================================+======+========+==========================+
|`cloud-tasks#9`_ AWS testing for PDS and PDS Engineering sites   |      |task    |p.must-have               |
+-----------------------------------------------------------------+------+--------+--------------------------+


- `cloud-tasks#4`_ B12.1 pds-engineering.nasa.gov Website Lift-and-Shift Pilot Project
    
+-----------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                            |I&T   |Level   |Priority / Bug Severity   |
+=================================================================+======+========+==========================+
|`cloud-tasks#9`_ AWS testing for PDS and PDS Engineering sites   |      |task    |p.must-have               |
+-----------------------------------------------------------------+------+--------+--------------------------+


- `cloud-tasks#5`_ NAIF.nasa.gov Website Lift-and-Shift Pilot Project (this theme has not epics in this repository)

- `cloud-tasks#7`_ B12.1 Refine AWS Registry Deployment Strategy
    
+-------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                              |I&T       |Level         |Priority / Bug Severity   |
+===================================================================================================================+==========+==============+==========================+
|`cloud-tasks#1`_ As a manager, I want a cost monitoring capability for AWS deployments                             ||iandt|   |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`cloud-tasks#13`_ Registry ES version incompatible with available available AWS managed ES / OpenSearch versions   |          |bug           |s.critical                |
+-------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `cloud-tasks#8`_ Develop Roadmap and Cost Model for PDS Cloud (this theme has not epics in this repository)

- `cloud-tasks#10`_ Initialize PDS-ESDIS NGAP Pilot Project
    
+------------------------------------------+------+--------------+--------------------------+
|Issue                                     |I&T   |Level         |Priority / Bug Severity   |
+==========================================+======+==============+==========================+
|`cloud-tasks#22`_ create users for NGAP   |      |enhancement   |p.must-have               |
+------------------------------------------+------+--------------+--------------------------+


- `cloud-tasks#11`_ B12.1 Deploy Node Registries
    
+---------------------------------------------------------+------+--------+--------------------------+
|Issue                                                    |I&T   |Level   |Priority / Bug Severity   |
+=========================================================+======+========+==========================+
|`cloud-tasks#12`_ Deploy production registries           |      |task    |unknown                   |
+---------------------------------------------------------+------+--------+--------------------------+
|`cloud-tasks#14`_ Implement CCS across node registries   |      |task    |unknown                   |
+---------------------------------------------------------+------+--------+--------------------------+


- `cloud-tasks#15`_ Design and Develop Registry Upgrade Strategy (this theme has not epics in this repository)

Other Updates
~~~~~~~~~~~~~
--------

Deep-archive
------------
*PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/deep-archive/>`_
     - `Github Repo <https://github.com/NASA-PDS/deep-archive>`_
     - `Issue Tracking <https://github.com/NASA-PDS/deep-archive/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/deep-archive/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/deep-archive/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/deep-archive/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `deep-archive#115`_ Revisit PDS Deep Archive Integration with Registry
    
+-------------------------------------------------------------------------------------------------------------------------------+------+--------------+--------------------------+
|Issue                                                                                                                          |I&T   |Level         |Priority / Bug Severity   |
+===============================================================================================================================+======+==============+==========================+
|`deep-archive#107`_ Update PDS Deep "Registry" Archive and remove workaround + implement latest-only-feature per API updates   |      |enhancement   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------+------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                     |I&T       |Priority / Bug Severity   |
+==========================================================================================+==========+==========================+
|`deep-archive#124`_ Unexpected fatal error when running pds-deep-archive against bundle   ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Devops
------
*Parent repo for PDS DevOps activities*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/devops#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/devops>`_
     - `Issue Tracking <https://github.com/NASA-PDS/devops/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/devops/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/devops/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/devops/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `devops#11`_ Implement Continuous Deployment Strategy (this theme has not epics in this repository)

- `devops#13`_ Continuous improvements to Continuous Integration
    
+-----------------------------------------------------------------------------+------+--------------+--------------------------+
|Issue                                                                        |I&T   |Level         |Priority / Bug Severity   |
+=============================================================================+======+==============+==========================+
|`devops#10`_ Rollout template updates to existing repos                      |      |task          |unknown                   |
+-----------------------------------------------------------------------------+------+--------------+--------------------------+
|`devops#12`_ Remove Versioneer                                               |      |task          |unknown                   |
+-----------------------------------------------------------------------------+------+--------------+--------------------------+
|`devops#14`_ Update Stable Major Releases of PDS software with DOIs          |      |requirement   |p.must-have               |
+-----------------------------------------------------------------------------+------+--------------+--------------------------+
|`devops#15`_ Update stable releases to handle Java repos                     |      |task          |unknown                   |
+-----------------------------------------------------------------------------+------+--------------+--------------------------+
|`devops#20`_ Update documentation for creating new repo to add DOI webhook   |      |task          |unknown                   |
+-----------------------------------------------------------------------------+------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
--------

Doi-service
-----------
*Service and tools for generating DOIs for PDS bundles, collections, and data sets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/doi-service>`_
     - `Github Repo <https://github.com/NASA-PDS/doi-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/doi-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/doi-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/doi-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/doi-service/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `doi-service#203`_ Improve DOI Service Documentation
    
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                           |I&T       |Level         |Priority / Bug Severity   |
+================================================================================================================+==========+==============+==========================+
|`doi-service#201`_ As an operator, I want to know how to deploy and use the API from the Sphinx documentation   ||iandt|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`doi-service#202`_ As an operator, I want one place to go for all DOI Service / API / UI documentation          ||iandt|   |requirement   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`doi-service#256`_ Develop DOI documentation for PDS Operator                                                   ||iandt|   |task          |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `doi-service#251`_ B12.1 Enhancements to PDS DOI Metadata
    
+----------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                     |I&T       |Level         |Priority / Bug Severity   |
+==========================================================================================================+==========+==============+==========================+
|`doi-service#102`_ Add new alternateIdentifier to match SBN schema                                        |          |enhancement   |p.must-have               |
+----------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`doi-service#294`_ Update all past DOIs for consistent metadata                                           |          |enhancement   |unknown                   |
+----------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`doi-service#303`_ identifiers vs alternateIdentifiers appear disconnected from current DataCite schema   ||iandt|   |bug           |s.high                    |
+----------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `doi-service#270`_ B12.1 DOI Metadata and Update Functionality Improvements
    
+--------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                               |I&T       |Level         |Priority / Bug Severity   |
+====================================================================================================================+==========+==============+==========================+
|`doi-service#257`_ As a PDS Operator, I want to perform a bulk update of a specific field across many DOI records   ||iandt|   |requirement   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`doi-service#278`_ As a user, I want to update the LIDVID associated with a DOI                                     ||iandt|   |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `doi-service#287`_ B12.1 DOI Service Integration with Registry
    
+----------------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                                 |I&T   |Level   |Priority / Bug Severity   |
+======================================================================+======+========+==========================+
|`doi-service#312`_ Develop script to sync SBN DOIs with DOI Service   |      |task    |unknown                   |
+----------------------------------------------------------------------+------+--------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                 |I&T       |Priority / Bug Severity   |
+======================================================================================================================+==========+==========================+
|`doi-service#318`_ Corruption in local database with invalid JSON                                                     |          |s.high                    |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#259`_ Spreadsheet parser does not validate/sanitize format of expected header row                        |          |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#258`_ Spreadsheet parser does not validate parsed contents of rows                                       ||iandt|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#310`_ Test DOIs are showing up in pds-gamma DOI search now linked from operations Citing PDS Data page   ||iandt|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#291`_ Spreadsheet parsers do not handle blank rows gracefully                                            |          |s.low                     |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#305`_ --no-review argument has potential to be confused with -n (node ID) argument                       ||iandt|   |s.low                     |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#273`_ Default keywords/subjects are not always added to DOI records                                      ||iandt|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#299`_ DOI Service does not assign adequate permissions to transaction database/history                   ||iandt|   |s.low                     |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#321`_ deactivate registered cassini doi 10.17189/1517823                                                 |          |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#214`_ Remove test and other transaction log data from public pypi distro                                 |          |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                            |I&T       |Priority / Bug Severity   |
+=================================================================================================================================+==========+==========================+
|`doi-service#317`_ Add Radio Science to set of possible nodes                                                                    |          |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#279`_ As a user, I want to update the bundle/collection metadata associated with a DOI for accumulating data sets   ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                        |I&T       |Priority / Bug Severity   |
+=============================================================================================+==========+==========================+
|`doi-service#231`_ Improve upon application security for write access                        ||iandt|   |unknown                   |
+---------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#260`_ Improve spreadsheet parser error handling                                 ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#289`_ As a user, I want to obtain json label format from a list command query   ||iandt|   |unknown                   |
+---------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Doi-ui
------
*web UI for pds-doi-service*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/doi-ui/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/doi-ui/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/doi-ui/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `doi-ui#60`_ DOI Search Component (this theme has not epics in this repository)

- `doi-ui#111`_ Complete DOI UI Implementation
    
+------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                 |I&T       |Level         |Priority / Bug Severity   |
+======================================================+==========+==============+==========================+
|`doi-ui#106`_ Update DOI UI app to use NPM package    ||iandt|   |enhancement   |unknown                   |
+------------------------------------------------------+----------+--------------+--------------------------+
|`doi-ui#115`_ deploy latest doi service on pds-dev3   |          |enhancement   |unknown                   |
+------------------------------------------------------+----------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                              |I&T       |Priority / Bug Severity   |
+===================================================================================================+==========+==========================+
|`doi-ui#67`_ Issue with displaying the content of an uploaded file after multiple selections       ||iandt|   |s.high                    |
+---------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#87`_ When I try to reload a reserve which has been updated, the web page does not update   ||iandt|   |s.high                    |
+---------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#88`_ Pre-existing keyword show in a weird way in the UI                                    ||iandt|   |s.medium                  |
+---------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#117`_ Fix DOI Search And DOI UI Integration Bugs                                           ||iandt|   |s.critical                |
+---------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                                                  |I&T   |Priority / Bug Severity   |
+=======================================================================================================================+======+==========================+
|`doi-ui#63`_ As an administrator, I want to deploy the ui from a release and be able to change the back-end API urls   |      |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------+------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                         |I&T       |Priority / Bug Severity   |
+==============================================================================================+==========+==========================+
|`doi-ui#68`_ Improve Search UI behavior to only show results when search button is selected   ||iandt|   |p.should-have             |
+----------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#102`_ Have a single entry for the backend API url configuration                       ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Feedback-widget
---------------
*Javascript widget for user feedback*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/feedback-widget#pds-feedback-widget>`_
     - `Github Repo <https://github.com/NASA-PDS/feedback-widget>`_
     - `Issue Tracking <https://github.com/NASA-PDS/feedback-widget/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/feedback-widget/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/feedback-widget/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/feedback-widget/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                |I&T       |Priority / Bug Severity   |
+=====================================================================================+==========+==========================+
|`feedback-widget#16`_ widget not working on pds.nasa.gov or pds-gamma.jpl.nasa.gov   |          |s.medium                  |
+-------------------------------------------------------------------------------------+----------+--------------------------+
|`feedback-widget#17`_ Feedback does not let submissions through for SBN              ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------+----------+--------------------------+

--------

Harvest
-------
*Provides software provides functionality for capturing and indexing product metadata in PDS Registry. A sub-component of the PDS Registry App (https://github.com/NASA-PDS/pds-registry-app)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app>`_
     - `Github Repo <https://github.com/NASA-PDS/harvest>`_
     - `Issue Tracking <https://github.com/NASA-PDS/harvest/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/harvest/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/harvest/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/harvest/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================+==========+==========================+
|`harvest#75`_ harvest stops rather than skips a file with bad permissions   ||iandt|   |s.high                    |
+----------------------------------------------------------------------------+----------+--------------------------+
|`harvest#78`_ Error ingesting an XML boolean with values of 0/1             ||iandt|   |s.high                    |
+----------------------------------------------------------------------------+----------+--------------------------+
|`harvest#70`_ Harvest fails on `yyyyZ` date time                            ||iandt|   |s.high                    |
+----------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------+------+--------------------------+
|Issue                                                  |I&T   |Priority / Bug Severity   |
+=======================================================+======+==========================+
|`harvest#64`_ Add release datetime to version output   |      |p.must-have               |
+-------------------------------------------------------+------+--------------------------+

--------

Mi-label
--------
*Metadata Injector for PDS Labels (MILabel) provides a command-line interface for generating PDS4 Labels using a user provided PDS4 XML template and input (source) data products.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/mi-label/>`_
     - `Github Repo <https://github.com/NASA-PDS/mi-label>`_
     - `Issue Tracking <https://github.com/NASA-PDS/mi-label/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/mi-label/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/mi-label/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/mi-label/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------+----------+--------------------------+
|Issue                                                          |I&T       |Priority / Bug Severity   |
+===============================================================+==========+==========================+
|`mi-label#21`_ Product-Tools parsing mode cannot parse units   ||iandt|   |s.medium                  |
+---------------------------------------------------------------+----------+--------------------------+

--------

Pds-api
-------
*PDS API Application with client and server integrated into one package*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `pds-api#111`_ B12.1 Response Format Improvements (this theme has not epics in this repository)

- `pds-api#114`_ Improve PDS API Development Workflow and Versioning
    
+----------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                       |I&T       |Level         |Priority / Bug Severity   |
+============================================================================+==========+==============+==========================+
|`pds-api#122`_ analysis of current workflow, ideas for improvment           |          |task          |unknown                   |
+----------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#123`_ create a super registry+api repository                       |          |task          |unknown                   |
+----------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#139`_ As a user, I want to see API stable release specifications   ||iandt|   |requirement   |p.must-have               |
+----------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#140`_ Merge unnecessary individual repository                      |          |enhancement   |unknown                   |
+----------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#142`_ flesh out the registry repository                            ||iandt|   |enhancement   |unknown                   |
+----------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#150`_ Update the swagger web tool from the specification           |          |task          |unknown                   |
+----------------------------------------------------------------------------+----------+--------------+--------------------------+


- `pds-api#117`_ [pds-api] B12.1 API Response Improvements
    
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                         |I&T       |Level         |Priority / Bug Severity   |
+==============================================================================================================================+==========+==============+==========================+
|`pds-api#66`_ As an API user, I want to get an XML response                                                                   ||iandt|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#125`_ As a user, I want to get the metadata in a pds4+xml response                                                   ||iandt|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#127`_ As a user, I want to clearly see which formats are accepted by the API when a 406 error is raised              ||iandt|   |requirement   |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#151`_ Update fields parameter definition to note that it does not apply to pds4+json and pds4+xml response formats   |          |task          |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#152`_ As a user, I want the API response media types to be compliant with RFC 6838                                   ||iandt|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#153`_ As a user, I want to receive error messages when an invalid request is submitted to the API                    ||iandt|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#154`_ Refactor `meta` section of pds4+json and pds4+xml to use ops namespace                                         ||iandt|   |enhancement   |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `pds-api#129`_ Prep for API v1.0 Release
    
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                           |I&T       |Level         |Priority / Bug Severity   |
+================================================================================================================+==========+==============+==========================+
|`pds-api#133`_ clarify what `keyword` parameter is for                                                          ||iandt|   |enhancement   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#136`_ Revise the pds-api README so that it gives a perspective on non search api (e.g. doi) from pds   ||iandt|   |enhancement   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#137`_ As a user, I want to have a detailed description of the API q parameter syntax                   ||iandt|   |enhancement   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#156`_ Disable automated github pages deployment with v1.0                                              |          |task          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                             |I&T       |Priority / Bug Severity   |
+==================================================================================================+==========+==========================+
|`pds-api#155`_ `products/{identifier}` missing properties object in application/json response     ||iandt|   |s.high                    |
+--------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#164`_ version number invalid according to PEP validation in CI                           |          |s.critical                |
+--------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#124`_ Changes to API per last tagged release not in SwaggerHub                           |          |s.critical                |
+--------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#121`_ Deployed API + Registry does not contain product metadata for pds4+json response   ||iandt|   |s.high                    |
+--------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                      |I&T       |Priority / Bug Severity   |
+===========================================================================================================================+==========+==========================+
|`pds-api#120`_ As an API user, I want a CSV response format option                                                         ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#106`_ As a API manager, I want to restrict access to registered products that should not be publicly accessible   ||iandt|   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#74`_ As an API user, I want to specify whether I get the latest or all versions of a product                      ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#134`_ As an API user, I want to get a key-value-pair JSON response                                                ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#72`_ As an API user, I want to search by a temporal range as an ISO-8601 time interval.                           ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#65`_ As an API user, I want to get only the fields I explicitly requested                                         ||iandt|   |p.could-have              |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================================================================+==========+==========================+
|`pds-api#112`_ As an API client user, I want to consistently and robustly start local servers for development and testing   |          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#145`_ Remove the x-total-count header from the API specification                                                   ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#108`_ Update API endpoints to use `identifier` instead of `lidvid`                                                 ||iandt|   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#110`_ Extend application/pds4+json support to all endpoints                                                        ||iandt|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Pds-api-client
--------------
*PDS API Client*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-api-client/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api-client>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api-client/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api-client/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api-client/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api-client/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                           |I&T       |Priority / Bug Severity   |
+================================================================================================+==========+==========================+
|`pds-api-client#17`_ Import failure for pds.api_client.CollectionsApi using PIP package 0.8.0   ||iandt|   |s.critical                |
+------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api-client#19`_ The demo provided on pds-api-client quickstart gives a 500 error           ||iandt|   |s.high                    |
+------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api-client#18`_ Links to client API details are broken on GitHub site                      ||iandt|   |s.high                    |
+------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Pds-registry-app
----------------
*Registry application enabling a PDS node to register all its data products for long term preservation and sharing with the rest of the PDS system. This repo builds, packages, and documents all the services and tools related to the ingestion and access of the data.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-registry-app>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-registry-app/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-registry-app/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-registry-app/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-registry-app/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `pds-registry-app#26`_ Manage duplicate products (this theme has not epics in this repository)

- `pds-registry-app#184`_ B12.1 Registry Tools Performance Improvements
    
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                                 |I&T       |Level         |Priority / Bug Severity   |
+======================================================================================================================================+==========+==============+==========================+
|`pds-registry-app#179`_ As a user, I want the registry app components to be able to ingest data sets containing 1+ million products   ||iandt|   |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-registry-app#200`_ As a user, I want big data ingestion tools packaged and dockerized together                                   ||iandt|   |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-registry-app#217`_ Clearly define best practices configuration for harvest/registry-mgr                                          |          |task          |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-registry-app#218`_ Document big data harvest / registry manager / crawler installation and operation                             |          |task          |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `pds-registry-app#190`_ Provide Initial Support for Restricted Access vs. Public Data
    
+----------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                                               |I&T       |Level         |Priority / Bug Severity   |
+====================================================================================================================================================+==========+==============+==========================+
|`pds-registry-app#201`_ As a user, I want to be able to ingest a set of files specified in a file listing                                           ||iandt|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-registry-app#223`_ As a user, I want to change the archive status for a collection and it's associated products                                ||iandt|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-registry-app#224`_ As a user, I want to switch a bundle and it's associated collections and products from a protected status to operational.   ||iandt|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-registry-app#228`_ Develop design documentation for staging vs production data for review with SWG                                             |          |task          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `pds-registry-app#194`_ Populate EN Registry (this theme has not epics in this repository)

- `pds-registry-app#199`_ Dockerize Registry Components for Dev and Ops Deployments
    
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                                 |I&T       |Level         |Priority / Bug Severity   |
+======================================================================================================================================+==========+==============+==========================+
|`pds-registry-app#187`_ As a developer, I want to be able to access the registry related docker images from https://hub.docker.com/   ||iandt|   |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-registry-app#208`_ As a developer I want to start the registry with a single command                                             ||iandt|   |task          |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `pds-registry-app#219`_ Re-imagine Registry Handling of Product Versioning (this theme has not epics in this
repository)

- `pds-registry-app#226`_ Upgrade Registry App to OpenSearch
    
+------------------------------------------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                                                           |I&T   |Level   |Priority / Bug Severity   |
+================================================================================================+======+========+==========================+
|`pds-registry-app#250`_ test registry docker compose with opensearch instead of elasticsearch   |      |task    |unknown                   |
+------------------------------------------------------------------------------------------------+------+--------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                         |I&T       |Priority / Bug Severity   |
+==============================================================================================================+==========+==========================+
|`pds-registry-app#220`_ harvest flags as mandatory a config elements the docs describe as optional            ||iandt|   |s.low                     |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#177`_ stable continuous integration don't generate the packages tar.gz and .zip properly.   |          |s.medium                  |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#231`_ the snapshot releases are not created for big-data-harvest-client                     |          |s.critical                |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#205`_ Harvest network I/O errors can cause corrupted JSON                                   ||iandt|   |s.high                    |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#238`_ pom.xml on main is broken                                                             |          |s.high                    |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                        |I&T       |Priority / Bug Severity   |
+=============================================================================================================+==========+==========================+
|`pds-registry-app#241`_ Simplify the readme and procedure to start the registry with docker-compose          |          |p.should-have             |
+-------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#186`_ As a developer, I want to deploy the registry with a single docker-compose command   ||iandt|   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                   |I&T       |Priority / Bug Severity   |
+========================================================================================================================+==========+==========================+
|`pds-registry-app#237`_ Rename bigdata repositories                                                                     |          |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#257`_ Simple wrappers to call the pds-batch-loader and pds-service-loader docker compose services     ||iandt|   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#230`_ As a developer, I want to update and run the integration tests from the 'registry' repository   |          |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#90`_ Develop cost model and reporting for Registry deployments                                        |          |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#260`_ Make CICD work on registry-api repository                                                       |          |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-registry-app#245`_ Update the README of the harvest service repositories                                           |          |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Pds-report-service
------------------
*PDS Report and Metrics Service with ELK stack*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-report-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-report-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-report-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-report-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-report-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-report-service/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+--------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                 |I&T   |Priority / Bug Severity   |
+======================================================================================+======+==========================+
|`pds-report-service#9`_ Expand number years included in OREx and New Horizons tasks   |      |unknown                   |
+--------------------------------------------------------------------------------------+------+--------------------------+

--------

Pds-wds-react
-------------
*PDS Web Design System - React Implementation*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds-react>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-wds-react>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-wds-react/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-wds-react/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-wds-react/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-wds-react/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `pds-wds-react#13`_ B12.1 Enhancements to DOI Search Component
    
+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                 |I&T       |Level         |Priority / Bug Severity   |
+======================================================================================================================+==========+==============+==========================+
|`pds-wds-react#5`_ Some findable product do not have links in the search results                                      ||iandt|   |bug           |s.high                    |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-wds-react#9`_ As a developer, I want to update the DOISearch component backend url in an attribute               ||iandt|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-wds-react#10`_ DOI Search updates per testing                                                                    ||iandt|   |task          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-wds-react#12`_ As a DOI Search user, I want to be able to find a parent data set DOI from a product identifier   ||iandt|   |requirement   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                     |I&T   |Priority / Bug Severity   |
+==========================================================================+======+==========================+
|`pds-wds-react#26`_ Fix Material UI Overriding Client App's Styling       |      |s.critical                |
+--------------------------------------------------------------------------+------+--------------------------+
|`pds-wds-react#28`_ Hovering Over Status Value Will Crash A Client App    |      |s.critical                |
+--------------------------------------------------------------------------+------+--------------------------+
|`pds-wds-react#27`_ Hovering Over Status Value Will Crash A Client App    |      |s.critical                |
+--------------------------------------------------------------------------+------+--------------------------+
|`pds-wds-react#29`_ Fix Search Not Running On First Call For Client App   |      |s.critical                |
+--------------------------------------------------------------------------+------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                                          |I&T       |Priority / Bug Severity   |
+===============================================================================================================================================+==========+==========================+
|`pds-wds-react#14`_ As a PDS.nasa.gov user, I want to search for the DOI for a PDS4 data product from a public facing website (pds.nasa.gov)   ||iandt|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                             |I&T       |Priority / Bug Severity   |
+==================================================================================+==========+==========================+
|`pds-wds-react#22`_ Update DOI Service per user feedback                          |          |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+
|`pds-wds-react#17`_ Combine NPM Package And Embeddable JS Script Toolchains       ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+
|`pds-wds-react#19`_ Create javascript library for website integration             ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+
|`pds-wds-react#4`_ Add Search DOI Component                                       ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+
|`pds-wds-react#8`_ Create a NPM package                                           ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+
|`pds-wds-react#15`_ Improve Search UI Behavior For DOI Search Widget              ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+
|`pds-wds-react#30`_ Update NPM Package Documentation                              ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+
|`pds-wds-react#18`_ Create PDS React Component Library Process For NPM Packages   ||iandt|   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------------------+

--------

Pds-web-mgmt
------------
*PDS Web Management and Unification Team*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-web-mgmt#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-web-mgmt>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-web-mgmt/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-web-mgmt/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-web-mgmt/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-web-mgmt/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `pds-web-mgmt#1`_ Initial Assessment of Today’s Web Management Landscape (this theme has not epics in this repository)

- `pds-web-mgmt#2`_ Preliminary Design of Migration (this theme has not epics in this repository)

- `pds-web-mgmt#3`_ Initial High-level Implementation Plan (this theme has not epics in this repository)

--------

Pds.nasa.gov-ux
---------------
*PDS.nasa.gov User Experience Task Issue and Prototype repository*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS.nasa.gov-UX#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS.nasa.gov-UX>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `PDS.nasa.gov-UX#77`_ Initial Information Architecture (this theme has not epics in this repository)

- `PDS.nasa.gov-UX#78`_ Initial Design Validation and Usability Testing (this theme has not epics in this repository)

- `PDS.nasa.gov-UX#100`_ B12.1 Continuation of User Persona and User Story Development
    
+---------------------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                                      |I&T   |Level   |Priority / Bug Severity   |
+===========================================================================+======+========+==========================+
|`PDS.nasa.gov-UX#99`_ Document initial User Stories using WMWG feedback    |      |task    |unknown                   |
+---------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#103`_ Iterate on WMWG feedback                            |      |task    |unknown                   |
+---------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#107`_ Tag user stories to modules and templates           |      |task    |unknown                   |
+---------------------------------------------------------------------------+------+--------+--------------------------+


- `PDS.nasa.gov-UX#101`_ Deploy new Citing PDS Data Web Pages (this theme has not epics in this repository)

- `PDS.nasa.gov-UX#109`_ Develop Initial User Journey Designs
    
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                                                      |I&T   |Level   |Priority / Bug Severity   |
+===========================================================================================+======+========+==========================+
|`PDS.nasa.gov-UX#115`_ Develop Module List                                                 |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#116`_ Develop Template List                                               |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#117`_ Prioritize Module List                                              |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#118`_ Prioritize Template List                                            |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#119`_ Define User Journeys                                                |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#120`_ Identify Key User Journeys                                          |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#121`_ Develop Low-fidelity User Journey Designs                           |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#128`_  Brainstorm additional modules based upon remaining user journeys   |      |task    |unknown                   |
+-------------------------------------------------------------------------------------------+------+--------+--------------------------+


- `PDS.nasa.gov-UX#110`_ Define Initial Content Strategy
    
+-----------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                            |I&T   |Level   |Priority / Bug Severity   |
+=================================================================+======+========+==========================+
|`PDS.nasa.gov-UX#122`_ Define Navigation Strategy                |      |task    |unknown                   |
+-----------------------------------------------------------------+------+--------+--------------------------+
|`PDS.nasa.gov-UX#123`_ Define Homepage / Landing Page Strategy   |      |task    |unknown                   |
+-----------------------------------------------------------------+------+--------+--------------------------+


- `PDS.nasa.gov-UX#111`_ Define Current Information Architecture
    
+-------------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                              |I&T   |Level   |Priority / Bug Severity   |
+===================================================================+======+========+==========================+
|`PDS.nasa.gov-UX#127`_ Finalize current information architecture   |      |task    |unknown                   |
+-------------------------------------------------------------------+------+--------+--------------------------+


--------

Pds4-information-model
----------------------
*The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-information-model/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-information-model>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-information-model/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds4-information-model/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-information-model/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-information-model/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `pds4-information-model#306`_ Refactoring of IMTool
    
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                      |I&T       |Level         |Priority / Bug Severity   |
+===========================================================================================================================+==========+==============+==========================+
|`pds4-information-model#239`_ Refactor Class information from config to Data Dictionary Protege ontology                   |          |enhancement   |unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds4-information-model#281`_ Tag ops classes/attributes in IM so they are easily identifiable by users                    ||iandt|   |enhancement   |unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds4-information-model#428`_ IMTool Refactoring - Phase 2 - Move deprecated values to Protege ontology file               ||iandt|   |enhancement   |unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds4-information-model#440`_ remaining code cleanup / refactoring                                                         |          |enhancement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds4-information-model#444`_ XML Schema files generated by LDDTool should not write the source file names in the header   ||iandt|   |enhancement   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `pds4-information-model#356`_ Kick-off PDS4 Information Model in GraphDB (this theme has not epics in this repository)

- `pds4-information-model#401`_ B12.1 LDDTool Improvements
    
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                      |I&T       |Level         |Priority / Bug Severity   |
+===========================================================================================================================+==========+==============+==========================+
|`pds4-information-model#269`_ The PDS4 IM Specification Document is not consistent in the ordering of Permissible Values   ||iandt|   |bug           |s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds4-information-model#341`_ As a user, I want to specify an IngestLDD using a relative path                              ||iandt|   |requirement   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `pds4-information-model#410`_ B12.1 LDDTool / PDS4 IM Documentation Updates (this theme has not epics in this
repository)

- `pds4-information-model#415`_ CCB-342: NASA, CODMAC, and PDS Processing Levels for Science Data Sets (this theme has
not   epics in this repository)

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                         |I&T       |Priority / Bug Severity   |
+==============================================================================================================+==========+==========================+
|`pds4-information-model#424`_ Missing JSON LDDs (alt & particle)                                              |          |s.low                     |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds4-information-model#418`_ Inconsistent naming of JSON schema files                                        ||iandt|   |s.medium                  |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds4-information-model#351`_ Contradictory DISP rule assertions exist in the PDS4 IM from legacy ingestion   ||iandt|   |s.medium                  |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds4-information-model#375`_ LDDTool documentation inconsistency                                             ||iandt|   |s.low                     |
+--------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================================================================+==========+==========================+
|`pds4-information-model#450`_ CCB-340 : <Local_Internal_Reference>.<local_identifier_reference> cardinality                 ||iandt|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds4-information-model#453`_ CCB-335: Inventory Specification Allows Too Many Delimiters                                   ||iandt|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds4-information-model#446`_ CCB-344:  Add data_to_partially_processed_product to reference types for Internal_Reference   ||iandt|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds4-information-model#448`_ CCB-343: Revise Product_Metadata_Supplemental                                                 ||iandt|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                           |I&T   |Priority / Bug Severity   |
+================================================================================+======+==========================+
|`pds4-information-model#421`_ [namespace-registry] add new namespace "<neas>"   |      |p.must-have               |
+--------------------------------------------------------------------------------+------+--------------------------+
|`pds4-information-model#435`_ [namespace-registry] add new namespace "lt"       |      |p.must-have               |
+--------------------------------------------------------------------------------+------+--------------------------+

--------

Pds4-jparser
------------
*Java Library providing APIs for parsing and exporting information on PDS4 products, including table and image objects to various formats including CSV, PNG, VICAR, FITs, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-jparser/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-jparser>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-jparser/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds4-jparser/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-jparser/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-jparser/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                                                 |I&T   |Priority / Bug Severity   |
+======================================================================================================================+======+==========================+
|`pds4-jparser#55`_ Improve ArrayObject accessor with new methods for improved access to the array label information   |      |p.could-have              |
+----------------------------------------------------------------------------------------------------------------------+------+--------------------------+

--------

Plaid
-----
*APPS PDS Label Assistant for Interactive Design (PLAID). See an overview of the software on YouTube. https://www.youtube.com/watch?v=WCo8erW_rL8*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://plaid.jpl.nasa.gov>`_
     - `Github Repo <https://github.com/NASA-PDS/PLAID>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PLAID/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/PLAID/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PLAID/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PLAID/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------+----------+--------------------------+
|Issue                                                        |I&T       |Priority / Bug Severity   |
+=============================================================+==========+==========================+
|`PLAID#32`_ Base image used by APPS PLAID is not supported   ||iandt|   |s.high                    |
+-------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                  |I&T       |Priority / Bug Severity   |
+=======================================================================+==========+==========================+
|`PLAID#30`_ Revise Docker and deployment docs for open source access   ||iandt|   |p.must-have               |
+-----------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------+----------+--------------------------+
|Issue                                                |I&T       |Priority / Bug Severity   |
+=====================================================+==========+==========================+
|`PLAID#16`_ Document processes for deploying PLAID   ||iandt|   |unknown                   |
+-----------------------------------------------------+----------+--------------------------+

--------

Portal-tasks
------------
*PDS Portal tasks repo used to track update requests for the website. Actual code and website are managed in separate private repo*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://pds.nasa.gov>`_
     - `Github Repo <https://github.com/NASA-PDS/portal-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal-tasks/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/portal-tasks/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal-tasks/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                          |I&T       |Priority / Bug Severity   |
+===============================================================================+==========+==========================+
|`portal-tasks#9`_ Broken link to PDS4_PDS_1H00.zip                             |          |s.high                    |
+-------------------------------------------------------------------------------+----------+--------------------------+
|`portal-tasks#6`_ links not working on data dictionary pages                   ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------+----------+--------------------------+
|`portal-tasks#10`_ DD Search and Tool Registry not working on pdscloud-gamma   ||iandt|   |s.critical                |
+-------------------------------------------------------------------------------+----------+--------------------------+
|`portal-tasks#19`_ viewBundle not working properly for DOI search logic        ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================+==========+==========================+
|`portal-tasks#7`_ As a user, I want to see a DOI on all DOI landing pages   |          |p.should-have             |
+----------------------------------------------------------------------------+----------+--------------------------+
|`portal-tasks#3`_ improvement on citing page                                ||iandt|   |unknown                   |
+----------------------------------------------------------------------------+----------+--------------------------+

--------

Registry-api
------------
*web API service of the PDS registry*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-api#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry-api/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-api/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                         |I&T       |Priority / Bug Severity   |
+==============================================================================================+==========+==========================+
|`registry-api#89`_ Fix unstable integration build failure                                     |          |s.medium                  |
+----------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#2`_ CICD did not publish the jar on artifactory                                 |          |s.medium                  |
+----------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#81`_ Service using JSON blob in pds4+xml response when it should use ops blob   |          |s.medium                  |
+----------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#73`_ blob/json_blob should not be included in default response                  ||iandt|   |s.high                    |
+----------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#5`_ AWS cost analysis tag  is not 'Alpha' but instead 'Alfa'                    |          |s.high                    |
+----------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                                  |I&T       |Priority / Bug Severity   |
+=======================================================================================================================================+==========+==========================+
|`registry-api#10`_ Rename `engineering` package naming to `registry`                                                                   |          |unknown                   |
+---------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#102`_ add ops:Tracking_Meta/ops:node_name and ops:Tracking_Meta/ops:harvest_date_time  to meta section of API response   ||iandt|   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Registry-api-service
--------------------
*PDS Registry API service. Complies with PDS API specification*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-api-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-api-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-api-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry-api-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-api-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-api-service/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                   |I&T       |Priority / Bug Severity   |
+========================================================================================================================+==========+==========================+
|`registry-api-service#79`_ simple url requested in a browser generate a 500 error                                       ||iandt|   |s.critical                |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#97`_ Revert  ES High Level Java API version 7.13.3                                                ||iandt|   |s.critical                |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#102`_ when fields are selected in the 'application/kvp+json' format some extra fields are found   ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#87`_ service is not handling value of ES login correctly                                          ||iandt|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#103`_ All the supported format don't show in the swagger-ui                                       ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#85`_ AWS target groups created in terraform do not have intended targets                          ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#88`_ api should handle request with no Accept header                                              ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                                              |I&T   |Priority / Bug Severity   |
+===================================================================================================================+======+==========================+
|`registry-api-service#52`_ As a developer, I was to be able to use AWS Secrets Manager with registry api service   |      |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------+------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                   |I&T       |Priority / Bug Severity   |
+========================================================================================================+==========+==========================+
|`registry-api-service#78`_ Add aws cost tagging and secret/parameter creation to ECS terraform script   ||iandt|   |unknown                   |
+--------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#95`_ add creation of routing rule to terraform script                             ||iandt|   |s.high                    |
+--------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api-service#81`_ Support for node-specific routing in API paths                               |          |unknown                   |
+--------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Registry-common
---------------
*Common code used by both Harvest and Registry Manager*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-common#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-common>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-common/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry-common/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-common/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-common/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================================+==========+==========================+
|`registry-common#20`_ Missing support for datetime conversion for ASCII_Date_Time_DOY_UTC   ||iandt|   |s.low                     |
+--------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Registry-mgr
------------
*Tool for managing the Elastic Search back-end Registry Service for tracking, searching, auditing, locating, and maintaining artifacts within the Planetary Data System. See new PDS Registry App for more details (https://github.com/NASA-PDS/pds-registry-app)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-mgr>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-mgr/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry-mgr/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-mgr/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-mgr/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================+==========+==========================+
|`registry-mgr#43`_ Improve error message for corrupted registry_docs.json   ||iandt|   |s.medium                  |
+----------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                             |I&T       |Priority / Bug Severity   |
+==================================================================================+==========+==========================+
|`registry-mgr#31`_ Update registy-mgr to use schema from schemaLocation in file   ||iandt|   |p.should-have             |
+----------------------------------------------------------------------------------+----------+--------------------------+

--------

Software-issues-repo
--------------------
*Issue tracking repository as a centralized entry point for general PDS software bugs and feature requests.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/software-issues-repo#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/software-issues-repo>`_
     - `Issue Tracking <https://github.com/NASA-PDS/software-issues-repo/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/software-issues-repo/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/software-issues-repo/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/software-issues-repo/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `software-issues-repo#14`_ B12.0 Prep for I&T
    
+---------------------------------------------------------------+----------+--------+--------------------------+
|Issue                                                          |I&T       |Level   |Priority / Bug Severity   |
+===============================================================+==========+========+==========================+
|`software-issues-repo#15`_ Generate Draft B12.0 RDD            ||iandt|   |task    |unknown                   |
+---------------------------------------------------------------+----------+--------+--------------------------+
|`software-issues-repo#16`_ Final testing and delivery to I&T   ||iandt|   |task    |unknown                   |
+---------------------------------------------------------------+----------+--------+--------------------------+


- `software-issues-repo#17`_ B12.1 Generate Release Plan (this theme has not epics in this repository)

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                             |I&T       |Priority / Bug Severity   |
+==================================================================================+==========+==========================+
|`software-issues-repo#19`_ viewHostProfile.jsp never returns useful information   ||iandt|   |s.medium                  |
+----------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------+----------+--------------------------+
|Issue                                                               |I&T       |Priority / Bug Severity   |
+====================================================================+==========+==========================+
|`software-issues-repo#9`_ Update login logic for Resource Manager   ||iandt|   |unknown                   |
+--------------------------------------------------------------------+----------+--------------------------+

--------

Template-repo-java
------------------
*Template for new NASA PDS repositories. For Python software, see https://github.com/nasa-pds/pds-template-repo-python*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/template-repo-java#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/template-repo-java>`_
     - `Issue Tracking <https://github.com/NASA-PDS/template-repo-java/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/template-repo-java/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/template-repo-java/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/template-repo-java/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                           |I&T       |Priority / Bug Severity   |
+================================================================================================+==========+==========================+
|`template-repo-java#9`_ Update README to include more details similar to python template repo   ||iandt|   |unknown                   |
+------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Validate
--------
*Validates PDS4 product labels, data and PDS3 Volumes*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/validate/>`_
     - `Github Repo <https://github.com/NASA-PDS/validate>`_
     - `Issue Tracking <https://github.com/NASA-PDS/validate/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/validate/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/validate/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/validate/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
- `validate#407`_ B12.1 Referential Integrity Improvements (this theme has not epics in this repository)

- `validate#409`_ B12.1 PDF/A Handling Improvements
    
+-------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                      |I&T       |Level         |Priority / Bug Severity   |
+===========================================================================================+==========+==============+==========================+
|`validate#388`_ Improve PDF/A validation to include more robust reporting on failures      ||iandt|   |requirement   |p.could-have              |
+-------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`validate#412`_ Update PDF validation to check against flavour specified in PDF metadata   ||iandt|   |task          |unknown                   |
+-------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


- `validate#426`_ B12.1 Content Validation Improvements
    
+------------------------------------------------------------------------------------------+----------+--------+--------------------------+
|Issue                                                                                     |I&T       |Level   |Priority / Bug Severity   |
+==========================================================================================+==========+========+==========================+
|`validate#423`_ Validate does not allow a single-character subdirectory                   ||iandt|   |bug     |s.medium                  |
+------------------------------------------------------------------------------------------+----------+--------+--------------------------+
|`validate#424`_ Validate does not allow SIP tab file to have lines of differing lengths   ||iandt|   |bug     |s.medium                  |
+------------------------------------------------------------------------------------------+----------+--------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                               |I&T       |Priority / Bug Severity   |
+====================================================================================================================================+==========+==========================+
|`validate#411`_ Validate repo cannot be checked out on Windows without errors                                                       ||iandt|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#349`_ validate allows absolute path in directory_path_name but shouldn't                                                  ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#390`_ validate does not flag *.tab files with variable length records                                                     ||iandt|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#376`_ Checksums output lowercase and do not accept uppercase checksums                                                    ||iandt|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#439`_ Incorrect Warning for Missing document_standard_id is Stream_Text                                                   ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#408`_ Validate 2.1.0-SNAPSHOT skips a collection XML label                                                                ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#441`_ Validate is reporting a 'String index out of range' error for a text file                                           ||iandt|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#461`_ [SECURITY] Patch log4j library                                                                                      ||iandt|   |s.critical                |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#470`_ Fix validate compilation issues due to removal of veraPDF artifacts from maven central                              ||iandt|   |s.critical                |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#419`_ validate 2.2.0-SNAPSHOT warns about a pretty benign bundle + readme.txt                                             ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#469`_ Validate content validation does not handle properly special_constants and field_statistics when they both appear   ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#435`_ Array Content Validator is not accepting values at the min/max due to false precision                               ||iandt|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#447`_ Validate does not correctly pass PDF/A files that are in a subdirectory                                             ||iandt|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================+==========+==========================+
|`validate#421`_ Improve warning message for missing_context_reference       ||iandt|   |p.must-have               |
+----------------------------------------------------------------------------+----------+--------------------------+
|`validate#377`_ Update rule documentation to remove "auto-detect" mention   |          |unknown                   |
+----------------------------------------------------------------------------+----------+--------------------------+

Liens
=====

+------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Issue                                                                                           |Title                                                                               |Rationale                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+================================================================================================+====================================================================================+============================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================+
|pds-swg_15_ [CR] B12.1 Defer Registry external source integration task                          |[CR] B12.1 Defer Registry external source integration task                          |<!-- enter rationale for deviation from plan here -->  With `Product_Metadata_Supplemental` and accompanying CSV ingestion supported, a workaround exists for ingesting database data. More use detailed use cases needed for what data needs to be ingested and how we can support it. Additionally, other API tasks have taken precedence ([Staging vs. Operational Data](https://github.com/nasa-pds/pds-registry-app/issues/190), [Handling "deprecated" LIDs and Versions](https://github.com/nasa-pds/pds-registry-app/issues/219))   |
+------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|pds-swg_14_ [CR] B12.1 Defer Validate Referential Integrity Checking and Logging Improvements   |[CR] B12.1 Defer Validate Referential Integrity Checking and Logging Improvements   |<!-- enter rationale for deviation from plan here -->  Validate CogE retired in December causing significant delays in content validation improvements and bug fixes (https://github.com/nasa-pds/validate/issues/426). Considering content validation is a critical component ensuring a valid archive, these tasks for improvements to existing capabilities is being tabled to B13.0.                                                                                                                                                    |
+------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B12.1-SNAPSHOT)`_

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

.. _Plan B12.1: https://nasa-pds.github.io/releases/12.1/plan.html
.. _pds4-information-model#446: https://github.com/NASA-PDS/pds4-information-model/issues/446
.. _pds4-information-model#448: https://github.com/NASA-PDS/pds4-information-model/issues/448
.. _pds4-information-model#450: https://github.com/NASA-PDS/pds4-information-model/issues/450
.. _pds4-information-model#453: https://github.com/NASA-PDS/pds4-information-model/issues/453
.. |iandt| image:: https://nasa-pds.github.io/_static/images/noun_certified_18093.png
   :alt: I&T
   :width: 20
.. _cloud-tasks#3: https://github.com/NASA-PDS/cloud-tasks/issues/3
.. _cloud-tasks#9: https://github.com/NASA-PDS/cloud-tasks/issues/9
.. _cloud-tasks#4: https://github.com/NASA-PDS/cloud-tasks/issues/4
.. _cloud-tasks#9: https://github.com/NASA-PDS/cloud-tasks/issues/9
.. _cloud-tasks#5: https://github.com/NASA-PDS/cloud-tasks/issues/5
.. _cloud-tasks#7: https://github.com/NASA-PDS/cloud-tasks/issues/7
.. _cloud-tasks#1: https://github.com/NASA-PDS/cloud-tasks/issues/1
.. _cloud-tasks#13: https://github.com/NASA-PDS/cloud-tasks/issues/13
.. _cloud-tasks#8: https://github.com/NASA-PDS/cloud-tasks/issues/8
.. _cloud-tasks#10: https://github.com/NASA-PDS/cloud-tasks/issues/10
.. _cloud-tasks#22: https://github.com/NASA-PDS/cloud-tasks/issues/22
.. _cloud-tasks#11: https://github.com/NASA-PDS/cloud-tasks/issues/11
.. _cloud-tasks#12: https://github.com/NASA-PDS/cloud-tasks/issues/12
.. _cloud-tasks#14: https://github.com/NASA-PDS/cloud-tasks/issues/14
.. _cloud-tasks#15: https://github.com/NASA-PDS/cloud-tasks/issues/15
.. _deep-archive#115: https://github.com/NASA-PDS/deep-archive/issues/115
.. _deep-archive#107: https://github.com/NASA-PDS/deep-archive/issues/107
.. _deep-archive#124: https://github.com/NASA-PDS/deep-archive/issues/124
.. _devops#11: https://github.com/NASA-PDS/devops/issues/11
.. _devops#13: https://github.com/NASA-PDS/devops/issues/13
.. _devops#10: https://github.com/NASA-PDS/devops/issues/10
.. _devops#12: https://github.com/NASA-PDS/devops/issues/12
.. _devops#14: https://github.com/NASA-PDS/devops/issues/14
.. _devops#15: https://github.com/NASA-PDS/devops/issues/15
.. _devops#20: https://github.com/NASA-PDS/devops/issues/20
.. _doi-service#203: https://github.com/NASA-PDS/doi-service/issues/203
.. _doi-service#201: https://github.com/NASA-PDS/doi-service/issues/201
.. _doi-service#202: https://github.com/NASA-PDS/doi-service/issues/202
.. _doi-service#256: https://github.com/NASA-PDS/doi-service/issues/256
.. _doi-service#251: https://github.com/NASA-PDS/doi-service/issues/251
.. _doi-service#102: https://github.com/NASA-PDS/doi-service/issues/102
.. _doi-service#294: https://github.com/NASA-PDS/doi-service/issues/294
.. _doi-service#303: https://github.com/NASA-PDS/doi-service/issues/303
.. _doi-service#270: https://github.com/NASA-PDS/doi-service/issues/270
.. _doi-service#257: https://github.com/NASA-PDS/doi-service/issues/257
.. _doi-service#278: https://github.com/NASA-PDS/doi-service/issues/278
.. _doi-service#287: https://github.com/NASA-PDS/doi-service/issues/287
.. _doi-service#312: https://github.com/NASA-PDS/doi-service/issues/312
.. _doi-service#318: https://github.com/NASA-PDS/doi-service/issues/318
.. _doi-service#259: https://github.com/NASA-PDS/doi-service/issues/259
.. _doi-service#258: https://github.com/NASA-PDS/doi-service/issues/258
.. _doi-service#310: https://github.com/NASA-PDS/doi-service/issues/310
.. _doi-service#291: https://github.com/NASA-PDS/doi-service/issues/291
.. _doi-service#305: https://github.com/NASA-PDS/doi-service/issues/305
.. _doi-service#273: https://github.com/NASA-PDS/doi-service/issues/273
.. _doi-service#299: https://github.com/NASA-PDS/doi-service/issues/299
.. _doi-service#321: https://github.com/NASA-PDS/doi-service/issues/321
.. _doi-service#214: https://github.com/NASA-PDS/doi-service/issues/214
.. _doi-service#317: https://github.com/NASA-PDS/doi-service/issues/317
.. _doi-service#279: https://github.com/NASA-PDS/doi-service/issues/279
.. _doi-service#231: https://github.com/NASA-PDS/doi-service/issues/231
.. _doi-service#260: https://github.com/NASA-PDS/doi-service/issues/260
.. _doi-service#289: https://github.com/NASA-PDS/doi-service/issues/289
.. _doi-ui#60: https://github.com/NASA-PDS/doi-ui/issues/60
.. _doi-ui#111: https://github.com/NASA-PDS/doi-ui/issues/111
.. _doi-ui#106: https://github.com/NASA-PDS/doi-ui/issues/106
.. _doi-ui#115: https://github.com/NASA-PDS/doi-ui/issues/115
.. _doi-ui#67: https://github.com/NASA-PDS/doi-ui/issues/67
.. _doi-ui#87: https://github.com/NASA-PDS/doi-ui/issues/87
.. _doi-ui#88: https://github.com/NASA-PDS/doi-ui/issues/88
.. _doi-ui#117: https://github.com/NASA-PDS/doi-ui/issues/117
.. _doi-ui#63: https://github.com/NASA-PDS/doi-ui/issues/63
.. _doi-ui#68: https://github.com/NASA-PDS/doi-ui/issues/68
.. _doi-ui#102: https://github.com/NASA-PDS/doi-ui/issues/102
.. _feedback-widget#16: https://github.com/NASA-PDS/feedback-widget/issues/16
.. _feedback-widget#17: https://github.com/NASA-PDS/feedback-widget/issues/17
.. _harvest#75: https://github.com/NASA-PDS/harvest/issues/75
.. _harvest#78: https://github.com/NASA-PDS/harvest/issues/78
.. _harvest#70: https://github.com/NASA-PDS/harvest/issues/70
.. _harvest#64: https://github.com/NASA-PDS/harvest/issues/64
.. _mi-label#21: https://github.com/NASA-PDS/mi-label/issues/21
.. _pds-api#111: https://github.com/NASA-PDS/pds-api/issues/111
.. _pds-api#114: https://github.com/NASA-PDS/pds-api/issues/114
.. _pds-api#122: https://github.com/NASA-PDS/pds-api/issues/122
.. _pds-api#123: https://github.com/NASA-PDS/pds-api/issues/123
.. _pds-api#139: https://github.com/NASA-PDS/pds-api/issues/139
.. _pds-api#140: https://github.com/NASA-PDS/pds-api/issues/140
.. _pds-api#142: https://github.com/NASA-PDS/pds-api/issues/142
.. _pds-api#150: https://github.com/NASA-PDS/pds-api/issues/150
.. _pds-api#117: https://github.com/NASA-PDS/pds-api/issues/117
.. _pds-api#66: https://github.com/NASA-PDS/pds-api/issues/66
.. _pds-api#125: https://github.com/NASA-PDS/pds-api/issues/125
.. _pds-api#127: https://github.com/NASA-PDS/pds-api/issues/127
.. _pds-api#151: https://github.com/NASA-PDS/pds-api/issues/151
.. _pds-api#152: https://github.com/NASA-PDS/pds-api/issues/152
.. _pds-api#153: https://github.com/NASA-PDS/pds-api/issues/153
.. _pds-api#154: https://github.com/NASA-PDS/pds-api/issues/154
.. _pds-api#129: https://github.com/NASA-PDS/pds-api/issues/129
.. _pds-api#133: https://github.com/NASA-PDS/pds-api/issues/133
.. _pds-api#136: https://github.com/NASA-PDS/pds-api/issues/136
.. _pds-api#137: https://github.com/NASA-PDS/pds-api/issues/137
.. _pds-api#156: https://github.com/NASA-PDS/pds-api/issues/156
.. _pds-api#155: https://github.com/NASA-PDS/pds-api/issues/155
.. _pds-api#164: https://github.com/NASA-PDS/pds-api/issues/164
.. _pds-api#124: https://github.com/NASA-PDS/pds-api/issues/124
.. _pds-api#121: https://github.com/NASA-PDS/pds-api/issues/121
.. _pds-api#120: https://github.com/NASA-PDS/pds-api/issues/120
.. _pds-api#106: https://github.com/NASA-PDS/pds-api/issues/106
.. _pds-api#74: https://github.com/NASA-PDS/pds-api/issues/74
.. _pds-api#134: https://github.com/NASA-PDS/pds-api/issues/134
.. _pds-api#72: https://github.com/NASA-PDS/pds-api/issues/72
.. _pds-api#65: https://github.com/NASA-PDS/pds-api/issues/65
.. _pds-api#112: https://github.com/NASA-PDS/pds-api/issues/112
.. _pds-api#145: https://github.com/NASA-PDS/pds-api/issues/145
.. _pds-api#108: https://github.com/NASA-PDS/pds-api/issues/108
.. _pds-api#110: https://github.com/NASA-PDS/pds-api/issues/110
.. _pds-api-client#17: https://github.com/NASA-PDS/pds-api-client/issues/17
.. _pds-api-client#19: https://github.com/NASA-PDS/pds-api-client/issues/19
.. _pds-api-client#18: https://github.com/NASA-PDS/pds-api-client/issues/18
.. _pds-registry-app#26: https://github.com/NASA-PDS/pds-registry-app/issues/26
.. _pds-registry-app#184: https://github.com/NASA-PDS/pds-registry-app/issues/184
.. _pds-registry-app#179: https://github.com/NASA-PDS/pds-registry-app/issues/179
.. _pds-registry-app#200: https://github.com/NASA-PDS/pds-registry-app/issues/200
.. _pds-registry-app#217: https://github.com/NASA-PDS/pds-registry-app/issues/217
.. _pds-registry-app#218: https://github.com/NASA-PDS/pds-registry-app/issues/218
.. _pds-registry-app#190: https://github.com/NASA-PDS/pds-registry-app/issues/190
.. _pds-registry-app#201: https://github.com/NASA-PDS/pds-registry-app/issues/201
.. _pds-registry-app#223: https://github.com/NASA-PDS/pds-registry-app/issues/223
.. _pds-registry-app#224: https://github.com/NASA-PDS/pds-registry-app/issues/224
.. _pds-registry-app#228: https://github.com/NASA-PDS/pds-registry-app/issues/228
.. _pds-registry-app#194: https://github.com/NASA-PDS/pds-registry-app/issues/194
.. _pds-registry-app#199: https://github.com/NASA-PDS/pds-registry-app/issues/199
.. _pds-registry-app#187: https://github.com/NASA-PDS/pds-registry-app/issues/187
.. _pds-registry-app#208: https://github.com/NASA-PDS/pds-registry-app/issues/208
.. _pds-registry-app#219: https://github.com/NASA-PDS/pds-registry-app/issues/219
.. _pds-registry-app#226: https://github.com/NASA-PDS/pds-registry-app/issues/226
.. _pds-registry-app#250: https://github.com/NASA-PDS/pds-registry-app/issues/250
.. _pds-registry-app#220: https://github.com/NASA-PDS/pds-registry-app/issues/220
.. _pds-registry-app#177: https://github.com/NASA-PDS/pds-registry-app/issues/177
.. _pds-registry-app#231: https://github.com/NASA-PDS/pds-registry-app/issues/231
.. _pds-registry-app#205: https://github.com/NASA-PDS/pds-registry-app/issues/205
.. _pds-registry-app#238: https://github.com/NASA-PDS/pds-registry-app/issues/238
.. _pds-registry-app#241: https://github.com/NASA-PDS/pds-registry-app/issues/241
.. _pds-registry-app#186: https://github.com/NASA-PDS/pds-registry-app/issues/186
.. _pds-registry-app#237: https://github.com/NASA-PDS/pds-registry-app/issues/237
.. _pds-registry-app#257: https://github.com/NASA-PDS/pds-registry-app/issues/257
.. _pds-registry-app#230: https://github.com/NASA-PDS/pds-registry-app/issues/230
.. _pds-registry-app#90: https://github.com/NASA-PDS/pds-registry-app/issues/90
.. _pds-registry-app#260: https://github.com/NASA-PDS/pds-registry-app/issues/260
.. _pds-registry-app#245: https://github.com/NASA-PDS/pds-registry-app/issues/245
.. _pds-report-service#9: https://github.com/NASA-PDS/pds-report-service/issues/9
.. _pds-wds-react#13: https://github.com/NASA-PDS/pds-wds-react/issues/13
.. _pds-wds-react#5: https://github.com/NASA-PDS/pds-wds-react/issues/5
.. _pds-wds-react#9: https://github.com/NASA-PDS/pds-wds-react/issues/9
.. _pds-wds-react#10: https://github.com/NASA-PDS/pds-wds-react/issues/10
.. _pds-wds-react#12: https://github.com/NASA-PDS/pds-wds-react/issues/12
.. _pds-wds-react#26: https://github.com/NASA-PDS/pds-wds-react/issues/26
.. _pds-wds-react#28: https://github.com/NASA-PDS/pds-wds-react/issues/28
.. _pds-wds-react#27: https://github.com/NASA-PDS/pds-wds-react/issues/27
.. _pds-wds-react#29: https://github.com/NASA-PDS/pds-wds-react/issues/29
.. _pds-wds-react#14: https://github.com/NASA-PDS/pds-wds-react/issues/14
.. _pds-wds-react#22: https://github.com/NASA-PDS/pds-wds-react/issues/22
.. _pds-wds-react#17: https://github.com/NASA-PDS/pds-wds-react/issues/17
.. _pds-wds-react#19: https://github.com/NASA-PDS/pds-wds-react/issues/19
.. _pds-wds-react#4: https://github.com/NASA-PDS/pds-wds-react/issues/4
.. _pds-wds-react#8: https://github.com/NASA-PDS/pds-wds-react/issues/8
.. _pds-wds-react#15: https://github.com/NASA-PDS/pds-wds-react/issues/15
.. _pds-wds-react#30: https://github.com/NASA-PDS/pds-wds-react/issues/30
.. _pds-wds-react#18: https://github.com/NASA-PDS/pds-wds-react/issues/18
.. _pds-web-mgmt#1: https://github.com/NASA-PDS/pds-web-mgmt/issues/1
.. _pds-web-mgmt#2: https://github.com/NASA-PDS/pds-web-mgmt/issues/2
.. _pds-web-mgmt#3: https://github.com/NASA-PDS/pds-web-mgmt/issues/3
.. _PDS.nasa.gov-UX#77: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/77
.. _PDS.nasa.gov-UX#78: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/78
.. _PDS.nasa.gov-UX#100: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/100
.. _PDS.nasa.gov-UX#99: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/99
.. _PDS.nasa.gov-UX#103: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/103
.. _PDS.nasa.gov-UX#107: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/107
.. _PDS.nasa.gov-UX#101: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/101
.. _PDS.nasa.gov-UX#109: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/109
.. _PDS.nasa.gov-UX#115: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/115
.. _PDS.nasa.gov-UX#116: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/116
.. _PDS.nasa.gov-UX#117: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/117
.. _PDS.nasa.gov-UX#118: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/118
.. _PDS.nasa.gov-UX#119: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/119
.. _PDS.nasa.gov-UX#120: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/120
.. _PDS.nasa.gov-UX#121: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/121
.. _PDS.nasa.gov-UX#128: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/128
.. _PDS.nasa.gov-UX#110: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/110
.. _PDS.nasa.gov-UX#122: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/122
.. _PDS.nasa.gov-UX#123: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/123
.. _PDS.nasa.gov-UX#111: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/111
.. _PDS.nasa.gov-UX#127: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/127
.. _pds4-information-model#306: https://github.com/NASA-PDS/pds4-information-model/issues/306
.. _pds4-information-model#239: https://github.com/NASA-PDS/pds4-information-model/issues/239
.. _pds4-information-model#281: https://github.com/NASA-PDS/pds4-information-model/issues/281
.. _pds4-information-model#428: https://github.com/NASA-PDS/pds4-information-model/issues/428
.. _pds4-information-model#440: https://github.com/NASA-PDS/pds4-information-model/issues/440
.. _pds4-information-model#444: https://github.com/NASA-PDS/pds4-information-model/issues/444
.. _pds4-information-model#356: https://github.com/NASA-PDS/pds4-information-model/issues/356
.. _pds4-information-model#401: https://github.com/NASA-PDS/pds4-information-model/issues/401
.. _pds4-information-model#269: https://github.com/NASA-PDS/pds4-information-model/issues/269
.. _pds4-information-model#341: https://github.com/NASA-PDS/pds4-information-model/issues/341
.. _pds4-information-model#410: https://github.com/NASA-PDS/pds4-information-model/issues/410
.. _pds4-information-model#415: https://github.com/NASA-PDS/pds4-information-model/issues/415
.. _pds4-information-model#424: https://github.com/NASA-PDS/pds4-information-model/issues/424
.. _pds4-information-model#418: https://github.com/NASA-PDS/pds4-information-model/issues/418
.. _pds4-information-model#351: https://github.com/NASA-PDS/pds4-information-model/issues/351
.. _pds4-information-model#375: https://github.com/NASA-PDS/pds4-information-model/issues/375
.. _pds4-information-model#450: https://github.com/NASA-PDS/pds4-information-model/issues/450
.. _pds4-information-model#453: https://github.com/NASA-PDS/pds4-information-model/issues/453
.. _pds4-information-model#446: https://github.com/NASA-PDS/pds4-information-model/issues/446
.. _pds4-information-model#448: https://github.com/NASA-PDS/pds4-information-model/issues/448
.. _pds4-information-model#421: https://github.com/NASA-PDS/pds4-information-model/issues/421
.. _pds4-information-model#435: https://github.com/NASA-PDS/pds4-information-model/issues/435
.. _pds4-jparser#55: https://github.com/NASA-PDS/pds4-jparser/issues/55
.. _PLAID#32: https://github.com/NASA-PDS/PLAID/issues/32
.. _PLAID#30: https://github.com/NASA-PDS/PLAID/issues/30
.. _PLAID#16: https://github.com/NASA-PDS/PLAID/issues/16
.. _portal-tasks#9: https://github.com/NASA-PDS/portal-tasks/issues/9
.. _portal-tasks#6: https://github.com/NASA-PDS/portal-tasks/issues/6
.. _portal-tasks#10: https://github.com/NASA-PDS/portal-tasks/issues/10
.. _portal-tasks#19: https://github.com/NASA-PDS/portal-tasks/issues/19
.. _portal-tasks#7: https://github.com/NASA-PDS/portal-tasks/issues/7
.. _portal-tasks#3: https://github.com/NASA-PDS/portal-tasks/issues/3
.. _registry-api#89: https://github.com/NASA-PDS/registry-api/issues/89
.. _registry-api#2: https://github.com/NASA-PDS/registry-api/issues/2
.. _registry-api#81: https://github.com/NASA-PDS/registry-api/issues/81
.. _registry-api#73: https://github.com/NASA-PDS/registry-api/issues/73
.. _registry-api#5: https://github.com/NASA-PDS/registry-api/issues/5
.. _registry-api#10: https://github.com/NASA-PDS/registry-api/issues/10
.. _registry-api#102: https://github.com/NASA-PDS/registry-api/issues/102
.. _registry-api-service#79: https://github.com/NASA-PDS/registry-api-service/issues/79
.. _registry-api-service#97: https://github.com/NASA-PDS/registry-api-service/issues/97
.. _registry-api-service#102: https://github.com/NASA-PDS/registry-api-service/issues/102
.. _registry-api-service#87: https://github.com/NASA-PDS/registry-api-service/issues/87
.. _registry-api-service#103: https://github.com/NASA-PDS/registry-api-service/issues/103
.. _registry-api-service#85: https://github.com/NASA-PDS/registry-api-service/issues/85
.. _registry-api-service#88: https://github.com/NASA-PDS/registry-api-service/issues/88
.. _registry-api-service#52: https://github.com/NASA-PDS/registry-api-service/issues/52
.. _registry-api-service#78: https://github.com/NASA-PDS/registry-api-service/issues/78
.. _registry-api-service#95: https://github.com/NASA-PDS/registry-api-service/issues/95
.. _registry-api-service#81: https://github.com/NASA-PDS/registry-api-service/issues/81
.. _registry-common#20: https://github.com/NASA-PDS/registry-common/issues/20
.. _registry-mgr#43: https://github.com/NASA-PDS/registry-mgr/issues/43
.. _registry-mgr#31: https://github.com/NASA-PDS/registry-mgr/issues/31
.. _software-issues-repo#14: https://github.com/NASA-PDS/software-issues-repo/issues/14
.. _software-issues-repo#15: https://github.com/NASA-PDS/software-issues-repo/issues/15
.. _software-issues-repo#16: https://github.com/NASA-PDS/software-issues-repo/issues/16
.. _software-issues-repo#17: https://github.com/NASA-PDS/software-issues-repo/issues/17
.. _software-issues-repo#19: https://github.com/NASA-PDS/software-issues-repo/issues/19
.. _software-issues-repo#9: https://github.com/NASA-PDS/software-issues-repo/issues/9
.. _template-repo-java#9: https://github.com/NASA-PDS/template-repo-java/issues/9
.. _validate#407: https://github.com/NASA-PDS/validate/issues/407
.. _validate#409: https://github.com/NASA-PDS/validate/issues/409
.. _validate#388: https://github.com/NASA-PDS/validate/issues/388
.. _validate#412: https://github.com/NASA-PDS/validate/issues/412
.. _validate#426: https://github.com/NASA-PDS/validate/issues/426
.. _validate#423: https://github.com/NASA-PDS/validate/issues/423
.. _validate#424: https://github.com/NASA-PDS/validate/issues/424
.. _validate#411: https://github.com/NASA-PDS/validate/issues/411
.. _validate#349: https://github.com/NASA-PDS/validate/issues/349
.. _validate#390: https://github.com/NASA-PDS/validate/issues/390
.. _validate#376: https://github.com/NASA-PDS/validate/issues/376
.. _validate#439: https://github.com/NASA-PDS/validate/issues/439
.. _validate#408: https://github.com/NASA-PDS/validate/issues/408
.. _validate#441: https://github.com/NASA-PDS/validate/issues/441
.. _validate#461: https://github.com/NASA-PDS/validate/issues/461
.. _validate#470: https://github.com/NASA-PDS/validate/issues/470
.. _validate#419: https://github.com/NASA-PDS/validate/issues/419
.. _validate#469: https://github.com/NASA-PDS/validate/issues/469
.. _validate#435: https://github.com/NASA-PDS/validate/issues/435
.. _validate#447: https://github.com/NASA-PDS/validate/issues/447
.. _validate#421: https://github.com/NASA-PDS/validate/issues/421
.. _validate#377: https://github.com/NASA-PDS/validate/issues/377
.. _pds-swg_15: https://github.com/NASA-PDS/pds-swg/issues/15
.. _pds-swg_14: https://github.com/NASA-PDS/pds-swg/issues/14
.. _Software Release Summary (B12.1-SNAPSHOT): https://nasa-pds.github.io/releases/12.1-SNAPSHOT/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
