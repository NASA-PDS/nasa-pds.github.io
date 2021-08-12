=========================================
Release Description Document (build 11.1)
=========================================
This release of the PDS4 System is intended as an operational release of
the system components to date.
The original plan for this release can be found here: `plan B11.1`_

The following sections can be found in this document:

.. toctree::
   :glob: 
   :maxdepth: 2

   rdd.rst

PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information
Model approved by the PDS4 Change Control Board and implemented by the
PDS within the latest build period.

+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|Ref                             |Title                                                                                                          |
+================================+===============================================================================================================+
|`pds4-information-model#97`_    |CCB-204: Define and enforce best practices for discipline and project dictionaries. - Part 1                   |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#99`_    |CCB-268 Add optional attribute to class Terminological_Entry                                                   |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#101`_   |CCB-204: Validate that no attribute is named "unit" - Part 2                                                   |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#103`_   |CCB-138 Fix mismatch between context object types and values of <type> in <Observing_System_Component> class   |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#109`_   |Clean up IMTool/LDDTool UML/XMI file writer for MagicDraw UML Class Diagrams                                   |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#111`_   |LDDTool aborts on short filename                                                                               |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#113`_   |CCB-204: Define and enforce best practices for discipline and project dictionaries. Part-3                     |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#116`_   |CCB-220: Add ability to specify many source products via table                                                 |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#120`_   |CCB-271: Add appropriate reference_type values for Product_Ancillary                                           |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#122`_   |CCB-204: Define and enforce best practices for discipline and project dictionaries. Part-4                     |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#125`_   |Nillable attributes are not declared nillable in class definitions.                                            |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#127`_   |Sync up LDDTool version with Maven build version                                                               |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#130`_   |CCB-256: Need method for providing permissible value definitions for external namespaces in Ingest_LDD         |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#133`_   |CCB-271: Add reference_types for Product_Ancillary                                                             |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#135`_   |CCB-220: Add ability to specify many source products via table.                                                |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#137`_   |CCB-274 - Add attribute dictionary_type to Ingest_LDD                                                          |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#139`_   |CCB-278: Fix errors in logical_identifier, ASCII_LID, ASCIIVID and ASCII_LIDVID_LID                            |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#144`_   |CCB-274 - Add attribute dictionary_type to Ingest_LDD - Update                                                 |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#148`_   |CCB-272: Reinstate Array_1D in the Information Model                                                           |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#152`_   |CCB-279: Mis-Matched <axes> and Axis_Array Specifications                                                      |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#165`_   |CCB-284: Streamline process for adding or removing standard values.                                            |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#166`_   |CCB-285:  GeoTIFF format as operational PDS4 image                                                             |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#270`_   |CCB-323: Fix schema formation rule for lidvid_reference (Part II)                                              |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#250`_   |CCB-315: "PDS3" is an allowed parsing standard for Bundle documentation file                                   |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#252`_   |CCB-304: Cleanup unused Vector classes in IM before 2.0.0.0                                                    |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#253`_   |CCB-313: Definition of <external_source_product_identifier> refers to non-existent documentation               |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#254`_   |CCB-305: Missing validation constraint on <specified_unit_id>                                                  |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#255`_   |CCB-300: Apparently deprecated units of measure are not actually deprecated                                    |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#256`_   |CCB-312: <ldd_version_id> does not appear to be constrained the way LDDTool expects                            |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#257`_   |CCB-302: No <reference_type> values defined in DD_Attribute or DD_Class contexts                               |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#273`_   |CCB-317: Add FITS 4.0 to parsing_standard_id enumerated values for Header object                               |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#275`_   |CCB-313: Definition of <external_source_product_identifier> refers to non-existent documentation.              |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#288`_   |CCB-321: Add MPEG-4 as an encoding_standard_id for Product_Native                                              |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#339`_   |CCB-328 : Inconsistency in <title> type definition                                                             |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+

Software changes
================
harvest
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


requirement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                   |Priority / Bug Severity   |
+========================================================================================================+==========================+
|`harvest#37`_ As a user, I want a default configuration for harvest included in the tool package        |p.must-have               |
+--------------------------------------------------------------------------------------------------------+--------------------------+
|`harvest#45`_ As a user, I want to be able to ingest a directory of data that is not part of a bundle   |unknown                   |
+--------------------------------------------------------------------------------------------------------+--------------------------+

pds-api
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


enhancement
~~~~~~~~~~~

+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                |Priority / Bug Severity   |
+=====================================================================================================================+==========================+
|`pds-api#31`_ Streamline testing of API server implementation                                                        |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#12`_ Initial Query Syntax Lexer Implementation                                                              |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#14`_ Define initial set of intra-discipline (product-level) search scope                                    |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#17`_ Define initial structure for response format conventions and parameter definition                      |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#34`_ Deploy PDS API v0 (alpha) for beta testing                                                             |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#35`_ Initial Federated API implementation                                                                   |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#40`_ add lexer to registry api                                                                              |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#41`_ Manage field preselection in queries                                                                   |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#43`_ Implement content negotiation                                                                          |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#47`_ develop a jupyter notebook demo where a user can browse PDS archive from bundle to product data file   |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#52`_ Get investigation area/targets/instruments from external ids                                           |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+

pds-api-javalib
---------------
*base repository for PDS API definition and libraries*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-api-javalib>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api-javalib>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api-javalib/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api-javalib/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api-javalib/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api-javalib/releases>`_ 


enhancement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                 |Priority / Bug Severity   |
+======================================================================================+==========================+
|`pds-api-javalib#1`_ Add time out specification in swaggerHub definition of the API   |unknown                   |
+--------------------------------------------------------------------------------------+--------------------------+
|`pds-api-javalib#2`_ Add list of available fields in response format                  |unknown                   |
+--------------------------------------------------------------------------------------+--------------------------+

pds-deep-archive
----------------
*PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-deep-archive/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-deep-archive>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-deep-archive/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-deep-archive/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-deep-archive/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-deep-archive/releases>`_ 


bug
~~~

+------------------------------------------------------------------------+--------------------------+
|Issue                                                                   |Priority / Bug Severity   |
+========================================================================+==========================+
|`pds-deep-archive#99`_ aip_label_checksum is not for the correct file   |unknown                   |
+------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+-----------------------------------------------------------+--------------------------+
|Issue                                                      |Priority / Bug Severity   |
+===========================================================+==========================+
|`pds-deep-archive#80`_ NSSDCA Delivery Onboarding          |unknown                   |
+-----------------------------------------------------------+--------------------------+
|`pds-deep-archive#93`_ add year to directory path in URL   |unknown                   |
+-----------------------------------------------------------+--------------------------+

pds-doi-service
---------------
*Service and tools for generating DOIs for PDS bundles, collections, and data sets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-doi-service>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-doi-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-service/releases>`_ 


bug
~~~

+------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                       |Priority / Bug Severity   |
+============================================================================================================+==========================+
|`pds-doi-service#119`_ Raise a specific exception when the OSTI server is not reachable                     |s.medium                  |
+------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#141`_ api does not ignore '/' at the end of url                                            |s.low                     |
+------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#143`_ when release command keywords are broken with encoded characters                     |s.high                    |
+------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#150`_ when doing draft with warnings (e.g. duplicated title) the -f option does not help   |s.high                    |
+------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#154`_ draft OSTI label                                                                     |s.high                    |
+------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#159`_ The url /dois/{lidvid} should still return XML in the record attribute               |s.critical                |
+------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                      |Priority / Bug Severity   |
+===========================================================================================================+==========================+
|`pds-doi-service#52`_ API Implementation for DOI Service                                                   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#91`_ Develop User Access / Management Strategy                                            |unknown                   |
+-----------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#114`_ Draft action: read the doi from the pds4 label                                      |p.must-have               |
+-----------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#125`_ Update DOI UI and Service with new workflow for operational deployment              |unknown                   |
+-----------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#140`_ Update submission to OSTI to handle the removal of a field from the OSTI metadata   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#144`_ enable filter by status in sub-action 'pds-doi-cmd list'                            |unknown                   |
+-----------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#148`_ API POST /dois should accept DOI OSTI format in payload                             |p.must-have               |
+-----------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#157`_ When a pds4 label or osti can not be parsed generate error 400 in API               |p.should-have             |
+-----------------------------------------------------------------------------------------------------------+--------------------------+

pds-doi-ui
----------
*web UI for pds-doi-service*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-ui/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-doi-ui/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-ui/releases>`_ 


enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                          |Priority / Bug Severity   |
+===============================================================================================+==========================+
|`pds-doi-ui#14`_ Prevent the discipline node for doing DOI release without a ENG node review   |p.must-have               |
+-----------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#17`_  PDS Label url should take a public URL                                       |p.must-have               |
+-----------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#19`_ Release step needs a submitter/node                                           |p.must-have               |
+-----------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#27`_ Error need to be catched when one draft a pds4 label from the url             |p.must-have               |
+-----------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#28`_ Enable force warning                                                          |p.must-have               |
+-----------------------------------------------------------------------------------------------+--------------------------+

pds-registry-app
----------------
*Registry application enabling a PDS node to register all its data products for long term preservation and sharing with the rest of the PDS system.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-registry-app>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-registry-app/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-registry-app/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-registry-app/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-registry-app/releases>`_ 


enhancement
~~~~~~~~~~~

+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                         |Priority / Bug Severity   |
+==============================================================================================================================+==========================+
|`pds-registry-app#13`_ Beta test operational deployment                                                                       |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#27`_ Manage PDS4 product relationships                                                                      |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#92`_ Update Registry API per PDS API v0-beta                                                                |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#102`_ Add the API to the pds-registry-app package, with documentation                                       |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#107`_ Prep Registry Demo for Discipline Nodes                                                               |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#114`_ Manage product relationships v2 - collection inventories                                              |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#120`_ Develop kibana configuration for EN registry UI                                                       |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#123`_ Update registry-mgr documentation as stated in #86                                                    |p.could-have              |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#125`_ analyze need, propose architecture                                                                    |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#127`_ load data for kibana test                                                                             |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#133`_ Verify pds-registry-app doc is up to date, have registry configuration in the harvest conf examples   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
~~~~~~~~~~~

+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================================+==========================+
|`pds-registry-app#141`_ As a manager, I want a cost model for deploying a registry + API in AWS                                |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#146`_ As a node operator, I want the the registry schema to update autonomously when new data is ingested.   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+

pds-registry-common
-------------------
*Common code used by both Harvest and Registry Manager*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-registry-common#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-registry-common>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-registry-common/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-registry-common/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-registry-common/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-registry-common/releases>`_ 


enhancement
~~~~~~~~~~~

+---------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                  |Priority / Bug Severity   |
+=======================================================================================+==========================+
|`pds-registry-common#1`_ verify artifact is pushed to Maven central and setup the ci   |unknown                   |
+---------------------------------------------------------------------------------------+--------------------------+

pds-wds-web
-----------
*PDS Web Design System - Basic web implementation*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds-web>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-wds-web>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-wds-web/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-wds-web/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-wds-web/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-wds-web/releases>`_ 


enhancement
~~~~~~~~~~~

+-------------------------------------------------+--------------------------+
|Issue                                            |Priority / Bug Severity   |
+=================================================+==========================+
|`pds-wds-web#17`_ App Bar Node List Reordering   |p.could-have              |
+-------------------------------------------------+--------------------------+

PDS.nasa.gov-Search
-------------------
*Front-end interface for PDS.nasa.gov data search capability*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS.nasa.gov-Search#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS.nasa.gov-Search>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS.nasa.gov-Search/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS.nasa.gov-Search/releases>`_ 


enhancement
~~~~~~~~~~~

+---------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                        |Priority / Bug Severity   |
+=============================================================================================+==========================+
|`PDS.nasa.gov-Search#29`_ Iterate with DOI Working Group for improvements to landing pages   |p.must-have               |
+---------------------------------------------------------------------------------------------+--------------------------+

PDS.nasa.gov-UX
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


enhancement
~~~~~~~~~~~

+----------------------------------------------------------------------------------+--------------------------+
|Issue                                                                             |Priority / Bug Severity   |
+==================================================================================+==========================+
|`PDS.nasa.gov-UX#3`_ Formulate user stories for prototype                         |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#6`_ Model workflows and initial design directions                |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#8`_ Design mockups and develop Figma prototype                   |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#61`_ Refine user interview and survey analysis per MC comments   |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#70`_ Refine PDS Web Modernization working group plan             |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#71`_ Upload all data from airtable / survey to GDrive            |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+

pds4-information-model
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


bug
~~~

+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                   |Priority / Bug Severity   |
+========================================================================================================================+==========================+
|`pds4-information-model#266`_ Throw WARNING message when enumeration_flag = false but enumerations are specified        |s.low                     |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#280`_ CSV files fail to escape double quotes.                                                   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#302`_ LDDTool does not allow the bundle to be specified for generated dictionaries              |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#331`_ Invalid output schema when trying to set an Internal_Reference reference_type value set   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#339`_ CCB-328 : Inconsistency in <title> type definition                                        |s.low                     |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                    |Priority / Bug Severity   |
+=========================================================================================+==========================+
|`pds4-information-model#238`_ Continuing refactoring of IMTool / LDDTool                 |p.should-have             |
+-----------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#242`_ DocBook HTML/WebHelp generation and conversion processes   |unknown                   |
+-----------------------------------------------------------------------------------------+--------------------------+

pds4-jparser
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


bug
~~~

+------------------------------------------------------------------------------+--------------------------+
|Issue                                                                         |Priority / Bug Severity   |
+==============================================================================+==========================+
|`pds4-jparser#36`_ NoSuchMethodError: java.nio.ByteBuffer with Java9 Builds   |s.medium                  |
+------------------------------------------------------------------------------+--------------------------+

PLAID
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


enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------+--------------------------+
|Issue                                                                  |Priority / Bug Severity   |
+=======================================================================+==========================+
|`PLAID#10`_ Develop procedure for how to update PLAID with latest IM   |unknown                   |
+-----------------------------------------------------------------------+--------------------------+

registry-api-service
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


enhancement
~~~~~~~~~~~

+----------------------------------------------------------------------------------+--------------------------+
|Issue                                                                             |Priority / Bug Severity   |
+==================================================================================+==========================+
|`registry-api-service#2`_ Manage relationships bundle-collection-product in API   |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#4`_ Implement a lid resolver                                |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+

tracking-service
----------------
*Provides functionality for tracking status and other aspects pertaining to PDS products that are not captured in the Registry Service.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/tracking-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/tracking-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/tracking-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/tracking-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/tracking-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/tracking-service/releases>`_ 


bug
~~~

+--------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                       |Priority / Bug Severity   |
+============================================================================================+==========================+
|`tracking-service#18`_ tracking front page does not keep tracking in relative anchor href   |unknown                   |
+--------------------------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------+--------------------------+
|Issue                                                            |Priority / Bug Severity   |
+=================================================================+==========================+
|`tracking-service#10`_ Dockerize Tracking Service                |unknown                   |
+-----------------------------------------------------------------+--------------------------+
|`tracking-service#14`_ Add mysql database to docker deployment   |unknown                   |
+-----------------------------------------------------------------+--------------------------+

validate
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


bug
~~~

+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                       |Priority / Bug Severity   |
+============================================================================================================================================================+==========================+
|`validate#5`_ Improve file base name check according to Standards Reference                                                                                 |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#6`_ Improve pds4.bundle unlabeled files check to handle files without a file suffix                                                               |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#11`_ Update allowable field_format values per Standards Reference definition regarding [+-] characters                                            |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#153`_ Update validate to throw error when a file has a space in the filename                                                                      |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#240`_ Unexpected error for data collection in a sub-directory                                                                                     |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#271`_ validate 1.25.0-SNAPSHOT raises an exception when validating a product                                                                      |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#273`_ Bug performing bundle validation with nested directories                                                                                    |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#278`_ Registered context products file does not retain older versions of context products                                                         |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#281`_ Validate fails to report error in   File.file_size                                                                                          |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#291`_ When validating a product with a bad schematron definition, bundle validation also fails indicating the associated product does not exist   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#294`_ Content validation incorrectly reports error for floating-point values out of specified min/max range                                       |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#298`_ validate misses double quotes within a delimited table                                                                                      |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#301`_ unclear error message for field count matching                                                                                              |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+-------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                            |Priority / Bug Severity   |
+=================================================================================================+==========================+
|`validate#51`_ Provide the capability to specify multiple locations for pds4.bundle validation   |p.could-have              |
+-------------------------------------------------------------------------------------------------+--------------------------+
|`validate#81`_ Validate and throw error when duplicate LIDs are found in Bundle                  |p.should-have             |
+-------------------------------------------------------------------------------------------------+--------------------------+
|`validate#230`_ Update validate per SR requirements for collection inventories                   |p.should-have             |
+-------------------------------------------------------------------------------------------------+--------------------------+
|`validate#249`_ Improvements for validating accumulating bundles / collections                   |unknown                   |
+-------------------------------------------------------------------------------------------------+--------------------------+
|`validate#252`_ Implement initial behavioral testing framework with cucumber                     |p.should-have             |
+-------------------------------------------------------------------------------------------------+--------------------------+
|`validate#290`_ Migrate subset of existing regression tests to cucumber behavioral testing       |p.should-have             |
+-------------------------------------------------------------------------------------------------+--------------------------+
|`validate#322`_ Update installation documentation to require Java 1.9+                           |p.could-have              |
+-------------------------------------------------------------------------------------------------+--------------------------+
|`validate#323`_ Upgrade to Java 9+                                                               |p.should-have             |
+-------------------------------------------------------------------------------------------------+--------------------------+

requirement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                           |Priority / Bug Severity   |
+================================================================================================================================+==========================+
|`validate#188`_ As a user, I want to validate a bundle that uses multiple versions of the Information Model / Discipline LDDs   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#210`_ As a user, I want validate to raise a WARNING when differing versions of IM are used within a bundle            |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#292`_ CCB-264: Make the Line Feed (LF) character an allowed record delimiter                                          |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+

theme
~~~~~

+-------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                        |Priority / Bug Severity   |
+=============================================================================================================+==========================+
|`validate#250`_ Improvements to meet updated Standards Reference since initial requirements implementation   |unknown                   |
+-------------------------------------------------------------------------------------------------------------+--------------------------+

Liens
=====

+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Issue                                                      |Title                                           |Rationale                                                                                                                                                                                                                                                                                                                                                                              |
+===========================================================+================================================+=======================================================================================================================================================================================================================================================================================================================================================================================+
|pds-swg_7_ [CR] Defer PDS UX Tasks to B12.0                |[CR] Defer PDS UX Tasks to B12.0                |Deferring these tasks to B12.0 in order to develop a comprehensive, detailed plan, milestones, and activities for a PDS Web Modernization Team. https://github.com/nasa-pds/pds.nasa.gov-ux/issues/70                                                                                                                                                                                  |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|pds-swg_6_ [CR] Defer PDS API Tasks to B12.0               |[CR] Defer PDS API Tasks to B12.0               |Inaccurate estimates for time to complete other designs and implementations with PDS API WG.                                                                                                                                                                                                                                                                                           |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|pds-swg_5_ [CR] Defer Tracking Service Tasks to B12.0      |[CR] Defer Tracking Service Tasks to B12.0      |Tracking Service design and partial implementation was completed in 2018. Misunderstanding during handoff from previous developers that the software design did not include requirements definition, and design did not form to common API standards. Caused significant increase in scope for [requirements definition task](https://github.com/nasa-pds/tracking-service/issues/2)   |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|pds-swg_4_ [CR] Add additional PDS4 SCRs to Release Plan   |[CR] Add additional PDS4 SCRs to Release Plan   |Several additional SCRs passed by the CCB.                                                                                                                                                                                                                                                                                                                                             |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `software
release summary (B11.1)`_

Installation and operation
==========================
PDS Engineering node software are meant to be deployed in 3 contexts:
standalone, discipline nodes or engineering node
For the installation and operation manual see the `users manuals` in the
software summary sections below:

- `PDS Standalone`_

- `PDS Discipline Nodes`_

- `PDS Engineering Node only`_

Reference documents
===================
This section details the controlling and applicable documents referenced
for this release. The controlling documents are as follows:

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

- `PDS Deep Archive Sotware Requirements and Design Document (SRD/SDD)`_

- `PDS DOI Service Requirements and Design Document (SRD/SDD)`_

.. _plan B11.1: https://nasa-pds.github.io/releases/11.1/plan.html
.. _pds4-information-model#97: https://github.com/NASA-PDS/pds4-information-model/issues/97
.. _pds4-information-model#99: https://github.com/NASA-PDS/pds4-information-model/issues/99
.. _pds4-information-model#101: https://github.com/NASA-PDS/pds4-information-model/issues/101
.. _pds4-information-model#103: https://github.com/NASA-PDS/pds4-information-model/issues/103
.. _pds4-information-model#109: https://github.com/NASA-PDS/pds4-information-model/issues/109
.. _pds4-information-model#111: https://github.com/NASA-PDS/pds4-information-model/issues/111
.. _pds4-information-model#113: https://github.com/NASA-PDS/pds4-information-model/issues/113
.. _pds4-information-model#116: https://github.com/NASA-PDS/pds4-information-model/issues/116
.. _pds4-information-model#120: https://github.com/NASA-PDS/pds4-information-model/issues/120
.. _pds4-information-model#122: https://github.com/NASA-PDS/pds4-information-model/issues/122
.. _pds4-information-model#125: https://github.com/NASA-PDS/pds4-information-model/issues/125
.. _pds4-information-model#127: https://github.com/NASA-PDS/pds4-information-model/issues/127
.. _pds4-information-model#130: https://github.com/NASA-PDS/pds4-information-model/issues/130
.. _pds4-information-model#133: https://github.com/NASA-PDS/pds4-information-model/issues/133
.. _pds4-information-model#135: https://github.com/NASA-PDS/pds4-information-model/issues/135
.. _pds4-information-model#137: https://github.com/NASA-PDS/pds4-information-model/issues/137
.. _pds4-information-model#139: https://github.com/NASA-PDS/pds4-information-model/issues/139
.. _pds4-information-model#144: https://github.com/NASA-PDS/pds4-information-model/issues/144
.. _pds4-information-model#148: https://github.com/NASA-PDS/pds4-information-model/issues/148
.. _pds4-information-model#152: https://github.com/NASA-PDS/pds4-information-model/issues/152
.. _pds4-information-model#165: https://github.com/NASA-PDS/pds4-information-model/issues/165
.. _pds4-information-model#166: https://github.com/NASA-PDS/pds4-information-model/issues/166
.. _pds4-information-model#270: https://github.com/NASA-PDS/pds4-information-model/issues/270
.. _pds4-information-model#250: https://github.com/NASA-PDS/pds4-information-model/issues/250
.. _pds4-information-model#252: https://github.com/NASA-PDS/pds4-information-model/issues/252
.. _pds4-information-model#253: https://github.com/NASA-PDS/pds4-information-model/issues/253
.. _pds4-information-model#254: https://github.com/NASA-PDS/pds4-information-model/issues/254
.. _pds4-information-model#255: https://github.com/NASA-PDS/pds4-information-model/issues/255
.. _pds4-information-model#256: https://github.com/NASA-PDS/pds4-information-model/issues/256
.. _pds4-information-model#257: https://github.com/NASA-PDS/pds4-information-model/issues/257
.. _pds4-information-model#273: https://github.com/NASA-PDS/pds4-information-model/issues/273
.. _pds4-information-model#275: https://github.com/NASA-PDS/pds4-information-model/issues/275
.. _pds4-information-model#288: https://github.com/NASA-PDS/pds4-information-model/issues/288
.. _pds4-information-model#339: https://github.com/NASA-PDS/pds4-information-model/issues/339
.. _harvest#37: https://github.com/NASA-PDS/harvest/issues/37
.. _harvest#45: https://github.com/NASA-PDS/harvest/issues/45
.. _pds-api#31: https://github.com/NASA-PDS/pds-api/issues/31
.. _pds-api#12: https://github.com/NASA-PDS/pds-api/issues/12
.. _pds-api#14: https://github.com/NASA-PDS/pds-api/issues/14
.. _pds-api#17: https://github.com/NASA-PDS/pds-api/issues/17
.. _pds-api#34: https://github.com/NASA-PDS/pds-api/issues/34
.. _pds-api#35: https://github.com/NASA-PDS/pds-api/issues/35
.. _pds-api#40: https://github.com/NASA-PDS/pds-api/issues/40
.. _pds-api#41: https://github.com/NASA-PDS/pds-api/issues/41
.. _pds-api#43: https://github.com/NASA-PDS/pds-api/issues/43
.. _pds-api#47: https://github.com/NASA-PDS/pds-api/issues/47
.. _pds-api#52: https://github.com/NASA-PDS/pds-api/issues/52
.. _pds-api-javalib#1: https://github.com/NASA-PDS/pds-api-javalib/issues/1
.. _pds-api-javalib#2: https://github.com/NASA-PDS/pds-api-javalib/issues/2
.. _pds-deep-archive#99: https://github.com/NASA-PDS/pds-deep-archive/issues/99
.. _pds-deep-archive#80: https://github.com/NASA-PDS/pds-deep-archive/issues/80
.. _pds-deep-archive#93: https://github.com/NASA-PDS/pds-deep-archive/issues/93
.. _pds-doi-service#119: https://github.com/NASA-PDS/pds-doi-service/issues/119
.. _pds-doi-service#141: https://github.com/NASA-PDS/pds-doi-service/issues/141
.. _pds-doi-service#143: https://github.com/NASA-PDS/pds-doi-service/issues/143
.. _pds-doi-service#150: https://github.com/NASA-PDS/pds-doi-service/issues/150
.. _pds-doi-service#154: https://github.com/NASA-PDS/pds-doi-service/issues/154
.. _pds-doi-service#159: https://github.com/NASA-PDS/pds-doi-service/issues/159
.. _pds-doi-service#52: https://github.com/NASA-PDS/pds-doi-service/issues/52
.. _pds-doi-service#91: https://github.com/NASA-PDS/pds-doi-service/issues/91
.. _pds-doi-service#114: https://github.com/NASA-PDS/pds-doi-service/issues/114
.. _pds-doi-service#125: https://github.com/NASA-PDS/pds-doi-service/issues/125
.. _pds-doi-service#140: https://github.com/NASA-PDS/pds-doi-service/issues/140
.. _pds-doi-service#144: https://github.com/NASA-PDS/pds-doi-service/issues/144
.. _pds-doi-service#148: https://github.com/NASA-PDS/pds-doi-service/issues/148
.. _pds-doi-service#157: https://github.com/NASA-PDS/pds-doi-service/issues/157
.. _pds-doi-ui#14: https://github.com/NASA-PDS/pds-doi-ui/issues/14
.. _pds-doi-ui#17: https://github.com/NASA-PDS/pds-doi-ui/issues/17
.. _pds-doi-ui#19: https://github.com/NASA-PDS/pds-doi-ui/issues/19
.. _pds-doi-ui#27: https://github.com/NASA-PDS/pds-doi-ui/issues/27
.. _pds-doi-ui#28: https://github.com/NASA-PDS/pds-doi-ui/issues/28
.. _pds-registry-app#13: https://github.com/NASA-PDS/pds-registry-app/issues/13
.. _pds-registry-app#27: https://github.com/NASA-PDS/pds-registry-app/issues/27
.. _pds-registry-app#92: https://github.com/NASA-PDS/pds-registry-app/issues/92
.. _pds-registry-app#102: https://github.com/NASA-PDS/pds-registry-app/issues/102
.. _pds-registry-app#107: https://github.com/NASA-PDS/pds-registry-app/issues/107
.. _pds-registry-app#114: https://github.com/NASA-PDS/pds-registry-app/issues/114
.. _pds-registry-app#120: https://github.com/NASA-PDS/pds-registry-app/issues/120
.. _pds-registry-app#123: https://github.com/NASA-PDS/pds-registry-app/issues/123
.. _pds-registry-app#125: https://github.com/NASA-PDS/pds-registry-app/issues/125
.. _pds-registry-app#127: https://github.com/NASA-PDS/pds-registry-app/issues/127
.. _pds-registry-app#133: https://github.com/NASA-PDS/pds-registry-app/issues/133
.. _pds-registry-app#141: https://github.com/NASA-PDS/pds-registry-app/issues/141
.. _pds-registry-app#146: https://github.com/NASA-PDS/pds-registry-app/issues/146
.. _pds-registry-common#1: https://github.com/NASA-PDS/pds-registry-common/issues/1
.. _pds-wds-web#17: https://github.com/NASA-PDS/pds-wds-web/issues/17
.. _PDS.nasa.gov-Search#29: https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/29
.. _PDS.nasa.gov-UX#3: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/3
.. _PDS.nasa.gov-UX#6: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/6
.. _PDS.nasa.gov-UX#8: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/8
.. _PDS.nasa.gov-UX#61: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/61
.. _PDS.nasa.gov-UX#70: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/70
.. _PDS.nasa.gov-UX#71: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/71
.. _pds4-information-model#266: https://github.com/NASA-PDS/pds4-information-model/issues/266
.. _pds4-information-model#280: https://github.com/NASA-PDS/pds4-information-model/issues/280
.. _pds4-information-model#302: https://github.com/NASA-PDS/pds4-information-model/issues/302
.. _pds4-information-model#331: https://github.com/NASA-PDS/pds4-information-model/issues/331
.. _pds4-information-model#339: https://github.com/NASA-PDS/pds4-information-model/issues/339
.. _pds4-information-model#238: https://github.com/NASA-PDS/pds4-information-model/issues/238
.. _pds4-information-model#242: https://github.com/NASA-PDS/pds4-information-model/issues/242
.. _pds4-jparser#36: https://github.com/NASA-PDS/pds4-jparser/issues/36
.. _PLAID#10: https://github.com/NASA-PDS/PLAID/issues/10
.. _registry-api-service#2: https://github.com/NASA-PDS/registry-api-service/issues/2
.. _registry-api-service#4: https://github.com/NASA-PDS/registry-api-service/issues/4
.. _tracking-service#18: https://github.com/NASA-PDS/tracking-service/issues/18
.. _tracking-service#10: https://github.com/NASA-PDS/tracking-service/issues/10
.. _tracking-service#14: https://github.com/NASA-PDS/tracking-service/issues/14
.. _validate#5: https://github.com/NASA-PDS/validate/issues/5
.. _validate#6: https://github.com/NASA-PDS/validate/issues/6
.. _validate#11: https://github.com/NASA-PDS/validate/issues/11
.. _validate#153: https://github.com/NASA-PDS/validate/issues/153
.. _validate#240: https://github.com/NASA-PDS/validate/issues/240
.. _validate#271: https://github.com/NASA-PDS/validate/issues/271
.. _validate#273: https://github.com/NASA-PDS/validate/issues/273
.. _validate#278: https://github.com/NASA-PDS/validate/issues/278
.. _validate#281: https://github.com/NASA-PDS/validate/issues/281
.. _validate#291: https://github.com/NASA-PDS/validate/issues/291
.. _validate#294: https://github.com/NASA-PDS/validate/issues/294
.. _validate#298: https://github.com/NASA-PDS/validate/issues/298
.. _validate#301: https://github.com/NASA-PDS/validate/issues/301
.. _validate#51: https://github.com/NASA-PDS/validate/issues/51
.. _validate#81: https://github.com/NASA-PDS/validate/issues/81
.. _validate#230: https://github.com/NASA-PDS/validate/issues/230
.. _validate#249: https://github.com/NASA-PDS/validate/issues/249
.. _validate#252: https://github.com/NASA-PDS/validate/issues/252
.. _validate#290: https://github.com/NASA-PDS/validate/issues/290
.. _validate#322: https://github.com/NASA-PDS/validate/issues/322
.. _validate#323: https://github.com/NASA-PDS/validate/issues/323
.. _validate#188: https://github.com/NASA-PDS/validate/issues/188
.. _validate#210: https://github.com/NASA-PDS/validate/issues/210
.. _validate#292: https://github.com/NASA-PDS/validate/issues/292
.. _validate#250: https://github.com/NASA-PDS/validate/issues/250
.. _pds-swg_7: https://github.com/NASA-PDS/pds-swg/issues/7
.. _pds-swg_6: https://github.com/NASA-PDS/pds-swg/issues/6
.. _pds-swg_5: https://github.com/NASA-PDS/pds-swg/issues/5
.. _pds-swg_4: https://github.com/NASA-PDS/pds-swg/issues/4
.. _software release summary (B11.1): https://nasa-pds.github.io/releases/B11.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Sotware Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
