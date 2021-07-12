=========================================
Release Description Document (Build 11.1)
=========================================

This release of the PDS4 System is intended as an operational release of the system components to date. The following sections can be found in this document:

..  toctree::
    :glob:
    :maxdepth: 2

    rdd.rst


PDS4 Standards and Information Model Changes
============================================

This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Boarda and implemented by the PDS within the latest build period.

+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#255`_ CCB-300: Apparently deprecated units of measure are not actually deprecated                      |
+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#257`_ CCB-302: No <reference_type> values defined in DD_Attribute or DD_Class contexts                 |
+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#252`_ CCB-304: Cleanup unused Vector classes in IM before 2.0.0.0                                      |
+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#254`_ CCB-305: Missing validation constraint on <specified_unit_id>                                    |
+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#253`_ CCB-313: Definition of <external_source_product_identifier> refers to non-existent documentation |
+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#250`_ CCB-315: "PDS3" is an allowed parsing standard for Bundle documentation file                     |
+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#288`_ CCB-321: Add MPEG-4 as an encoding_standard_id for Product_Native                                |
+-------------------------------------------------------------------------------------------------------------------------------+
|`pds4-information-model#339`_ CCB-328 : Inconsistency in <title> type definition                                               |
+-------------------------------------------------------------------------------------------------------------------------------+

----

Software Changes
================

This section details the new, modified and corrected capabilities that comprise this release . They are summarized here for a system-level view. A more detailed list of capabilities can be found in the change logs for each component.

Note on Requirements: Requirement are now being provided for some project. The coverage is not yet complete. Please contact the `PDS Operator <mailto:pds-operator@jpl.nasa.gov>`_ or PDS EN staff if you would like additional details on software Requirements.

----

api-search-query-lexer
----------------------
*Lexer to parse the search query of the PDS API*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/api-search-query-lexer#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/api-search-query-lexer>`_
     - `Issue Tracking <https://github.com/NASA-PDS/api-search-query-lexer/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/api-search-query-lexer/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/api-search-query-lexer/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/api-search-query-lexer/releases>`_ 


Bug
~~~

+------------------------------------------------------------------------+--------------------------+
|Issue                                                                   |Priority / Bug Severity   |
+========================================================================+==========================+
|`api-search-query-lexer#1`_ parsing of string does not succeed          |unknown                   |
+------------------------------------------------------------------------+--------------------------+

----

archive-analytics
-----------------
*Processes, tools, and configuration for managing PDS archive analytics software and reports*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/archive-analytics#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/archive-analytics>`_
     - `Issue Tracking <https://github.com/NASA-PDS/archive-analytics/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/archive-analytics/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/archive-analytics/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/archive-analytics/releases>`_ 


Requirement
~~~~~~~~~~~

+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                         |Priority / Bug Severity   |
+==============================================================================================================================+==========================+
|`archive-analytics#2`_ As a manager, I want to know the current total volume of PDS holdings                                  |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`archive-analytics#7`_ As a PDS Project Office, I want to know the historical total volume of PDS holdings over time          |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`archive-analytics#10`_ As a Node Manager, I want to report on the number of artifacts within the archive                     |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+

----

harvest
-------
*Provides software provides functionality for capturing and indexing product metadata in PDS Registry. A sub-component of the PDS Registry App (https://github.com/NASA-PDS/pds-registry-app)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app>`_
     - `Github Repo <https://github.com/NASA-PDS/harvest>`_
     - `Issue Tracking <https://github.com/NASA-PDS/harvest/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/harvest/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/harvest/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/harvest/releases>`_ 


Bug
~~~

+---------------------------------------------------------------------------------+--------------------------+
|Issue                                                                            |Priority / Bug Severity   |
+=================================================================================+==========================+
|`harvest#6`_ Check input URIs to avoid potential security vulnerability          |s.low                     |
+---------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+--------------------------------------------------------+--------------------------+
|Issue                                                   |Priority / Bug Severity   |
+========================================================+==========================+
|`harvest#18`_ Track collection file inventory           |unknown                   |
+--------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+---------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================+==========================+
|`harvest#37`_ As a user, I want a default configuration for harvest included in the tool package               |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|`harvest#45`_ As a user, I want to be able to ingest a directory of data that is not part of a bundle          |unknown                   |
+---------------------------------------------------------------------------------------------------------------+--------------------------+

----

mi-label
--------
*Metadata Injector for PDS Labels (MILabel), formerly known as Generate Tool*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/mi-label/>`_
     - `Github Repo <https://github.com/NASA-PDS/mi-label>`_
     - `Issue Tracking <https://github.com/NASA-PDS/mi-label/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/mi-label/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/mi-label/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/mi-label/releases>`_ 


Bug
~~~

+--------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                 |Priority / Bug Severity   |
+======================================================================================+==========================+
|`mi-label#10`_ Windows version will not run because of error in generate.bat          |s.high                    |
+--------------------------------------------------------------------------------------+--------------------------+

----

pds-api
-------
*PDS API Application with client and server integrated into one package*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-api/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 


Bug
~~~

+------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                 |Priority / Bug Severity   |
+======================================================================================================+==========================+
|`pds-api#73`_ As a n00b paginator, there might be an off-by-1 error in the `limit` parameter          |s.medium                  |
+------------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                       |Priority / Bug Severity   |
+============================================================================================================================+==========================+
|`pds-api#31`_ Streamline testing of API server implementation                                                               |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#12`_ Initial Query Syntax Lexer Implementation                                                                     |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#17`_ Define initial structure for response format conventions and parameter definition                             |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#34`_ Deploy PDS API v0 (alpha) for beta testing                                                                    |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#35`_ Initial Federated API implementation                                                                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#40`_ add lexer to registry api                                                                                     |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#41`_ Manage field preselection in queries                                                                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#43`_ Implement content negotiation                                                                                 |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#47`_ develop a jupyter notebook demo where a user can browse PDS archive from bundle to product data file          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#52`_ Get investigation area/targets/instruments from external ids                                                  |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================================+==========================+
|`pds-api#54`_ As an API user, I want to perform a search using wildcards                                                       |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#56`_ As an API user, I want to know the children and ancestors of bundle, collections, and products                   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#59`_ As an API user, I want to know the Product(s) that belong to a given Bundle.                                     |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#60`_ As an API user, I want to know the Bundle for a given Product.                                                   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#61`_ As an API user, I want to know the Collection(s) for a given Product.                                            |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#62`_ As an API user, I want to know the Bundle for a given Collection.                                                |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#64`_ As a user, when I request specific fields I want to get records which have at least one of these fields          |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+

----

pds-api-client
--------------
*PDS API Client*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-api-client/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api-client>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api-client/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-api-client/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api-client/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api-client/releases>`_ 


Bug
~~~

+------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                               |Priority / Bug Severity   |
+====================================================================================+==========================+
|`pds-api-client#2`_ PDS API Client 1.0.0 cannot communicate with pds-gamma          |s.high                    |
+------------------------------------------------------------------------------------+--------------------------+

pds-api-javalib
---------------
*base repository for PDS API definition and libraries*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-api-javalib>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api-javalib>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api-javalib/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-api-javalib/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api-javalib/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api-javalib/releases>`_ 


Enhancement
~~~~~~~~~~~

+---------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                        |Priority / Bug Severity   |
+=============================================================================================+==========================+
|`pds-api-javalib#1`_ Add time out specification in swaggerHub definition of the API          |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+
|`pds-api-javalib#2`_ Add list of available fields in response format                         |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+

----

pds-deep-archive
----------------
*PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-deep-archive/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-deep-archive>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-deep-archive/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-deep-archive/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-deep-archive/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-deep-archive/releases>`_ 


Bug
~~~

+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                  |Priority / Bug Severity   |
+=======================================================================================================================+==========================+
|`pds-deep-archive#90`_ Small typo on package documentation                                                             |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-deep-archive#92`_ SIP manifest table erroneously includes secondary collections and their basic products          |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-deep-archive#99`_ aip_label_checksum is not for the correct file                                                  |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------+--------------------------+
|Issue                                                                              |Priority / Bug Severity   |
+===================================================================================+==========================+
|`pds-deep-archive#93`_ add year to directory path in URL                           |unknown                   |
+-----------------------------------------------------------------------------------+--------------------------+
|`pds-deep-archive#95`_ Bash required for default installation description          |unknown                   |
+-----------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                     |Priority / Bug Severity   |
+==========================================================================================+==========================+
|`pds-deep-archive#7`_ As a user, I want to generate AIPs and SIPs using Registry          |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|`pds-deep-archive#102`_ As a user, I want the SIP manifest to include valid URLs          |p.must-have               |
+------------------------------------------------------------------------------------------+--------------------------+

----

pds-doi-service
---------------
*Service and tools for generating DOIs for PDS bundles, collections, and data sets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-doi-service>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-service/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-doi-service/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-service/releases>`_ 


Bug
~~~

+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                |Priority / Bug Severity   |
+=====================================================================================================================================+==========================+
|`pds-doi-service#119`_ Raise a specific exception when the OSTI server is not reachable                                              |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#121`_ GET /dois must support empty vid field                                                                        |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#122`_ the sqllite database should be created at the same location, whereever the command are launched from          |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#126`_ get /dois/{lidvid}                                                                                            |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#128`_ command pds-doi-cmd list returns update date in timestamp instead of iso8601                                  |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#138`_ xlsx file extension for reserve not supported                                                                 |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#141`_ api does not ignore '/' at the end of url                                                                     |s.low                     |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#143`_ when release command keywords are broken with encoded characters                                              |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#150`_ when doing draft with warnings (e.g. duplicated title) the -f option does not help                            |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#154`_ draft OSTI label                                                                                              |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#159`_ The url /dois/{lidvid} should still return XML in the record attribute                                        |s.critical                |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                           |Priority / Bug Severity   |
+================================================================================================================================+==========================+
|`pds-doi-service#52`_ API Implementation for DOI Service                                                                        |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#91`_ Develop User Access / Management Strategy                                                                 |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#114`_ Draft action: read the doi from the pds4 label                                                           |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#116`_ Extraction of the OSTI XML in /dois?... GET requests                                                     |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#125`_ Update DOI UI and Service with new workflow for operational deployment                                   |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#134`_ Update draft action with new option --lidvid to change from review to draft the status of a DOI          |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#135`_ Update API to deactivate 'release' end point, create a 'submit' end-point                                |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#140`_ Update submission to OSTI to handle the removal of a field from the OSTI metadata                        |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#144`_ enable filter by status in sub-action 'pds-doi-cmd list'                                                 |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#148`_ API POST /dois should accept DOI OSTI format in payload                                                  |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#157`_ When a pds4 label or osti can not be parsed generate error 400 in API                                    |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#162`_ Implement Application Server to wrap Flask service                                                       |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#163`_ Dockerize API Service                                                                                    |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#165`_ Add service to API for update of the status of records with OSTI (check sub command)                     |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+----------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                           |Priority / Bug Severity   |
+================================================================================================================+==========================+
|`pds-doi-service#167`_ As a user, I want to see the lidvid of my DOIs in the email report                       |p.should-have             |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#177`_ As an API user I want to filter on lidvids with wildcards                                |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#180`_ As an API user I want to filter on PDS3 Data Set IDs with wildcards                      |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#183`_ As a user of the API, I want to see the DOI's title when I go GET /dois request          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#184`_ As an API user, I want to always have an update date for the DOIs                        |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+

----

pds-doi-ui
----------
*web UI for pds-doi-service*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-ui/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-doi-ui/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-ui/releases>`_ 


Bug
~~~

+------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                     |Priority / Bug Severity   |
+==========================================================================================+==========================+
|`pds-doi-ui#35`_ As a SA, I don't want security vulnerabilities in the public UI          |s.medium                  |
+------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                 |Priority / Bug Severity   |
+======================================================================================================+==========================+
|`pds-doi-ui#1`_ Reserve DOI UI forms                                                                  |unknown                   |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#9`_ Return API error message in UI                                                        |unknown                   |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#10`_ Provide a mean to come back to release action when on reserve screen                 |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#14`_ Prevent the discipline node for doing DOI release without a ENG node review          |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#17`_  PDS Label url should take a public URL                                              |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#19`_ Release step needs a submitter/node                                                  |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#27`_ Error need to be catched when one draft a pds4 label from the url                    |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#28`_ Enable force warning                                                                 |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#30`_ Display errors and warning when user clicks "save" on the release screen             |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#31`_ On release screen, have only one "ignore warning" checkbox                           |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                       |Priority / Bug Severity   |
+============================================================================================================================+==========================+
|`pds-doi-ui#25`_ As a user, I want to search for a DOI and associated metadata by LID/LIDVID                                |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#34`_ As a user, I want to see the error/warnings messages on the same page from where they were raised          |p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+

----

pds-registry-app
----------------
*Registry application enabling a PDS node to register all its data products for long term preservation and sharing with the rest of the PDS system.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-registry-app>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-registry-app/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-registry-app/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-registry-app/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-registry-app/releases>`_ 


Bug
~~~

+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                 |Priority / Bug Severity   |
+======================================================================================================================================+==========================+
|`pds-registry-app#108`_ harvest and registry manager in pds-registry-app-0.2.2-bin.zip are missing batch scripts for windows          |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#109`_ Test data in pds-registry-app-0.2.2-bin.zip contains invalid PDS4 labels                                      |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#110`_ Test data in pds-registry-app-0.2.2-bin.zip is missing data products.                                         |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#135`_ docker build is version locked                                                                                |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                |Priority / Bug Severity   |
+=====================================================================================================================+==========================+
|`pds-registry-app#20`_ Update Schema Generator for handling special cases where ancestor classes are needed          |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#27`_ Manage PDS4 product relationships                                                             |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#102`_ Add the API to the pds-registry-app package, with documentation                              |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#103`_ update registry-manager load-data to handle additional use cases                             |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#113`_ Have pds4 properties syntax match the syntax decided for the PDS API                         |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#122`_ Initial deployment of API on AWS - ASG/ELB solution                                          |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#123`_ Update registry-mgr documentation as stated in #86                                           |p.could-have              |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#129`_ Create a registry docker for developer testing                                               |p.could-have              |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#131`_ Develop ElasticSearch client library to be utilized by harvest / registry-mgr                |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================================================+==========================+
|`pds-registry-app#57`_ The service shall accept artifact registrations.                                                                        |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#58`_ The service shall provide a means identifying relationships between artifact registrations                              |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#59`_ The service shall maintain configuration regarding the classes of artifacts to be registered                            |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#75`_ The service shall accept metadata for a registered artifact in a defined format                                         |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#56`_ The service shall assign a global unique identifier to a registered artifact                                            |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#73`_ The service shall require a logical identifier and version be provided for all registered artifacts                     |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#72`_ The service shall store metadata for a registered artifact in an underlying metadata store                              |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#71`_ The service shall allow updates to registered artifacts                                                                 |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#70`_ The service shall allow deletion of registered artifacts                                                                |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#55`_ The service shall allow for queries for registered artifacts                                                            |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#68`_ The service shall require checksums as metadata for registry artifact to enable system-wide integrity checking          |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#67`_ The service shall require a subset of file system metadata in order to support data metrics generation                  |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#66`_ The service shall require user authorization for updating registry metadata                                             |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#65`_ The service shall provide a staging capability for artifacts staged for release                                         |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#141`_ As a manager, I want a cost model for deploying a registry + API in AWS                                                |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#142`_ As a node operator, I want actionable, user-friendly error messages for registry schema failures                       |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#143`_ As a node operator, I want to ingest metadata regarding secondary products that belong to a collection.                |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#144`_ As a node operator, I want to ingest metadata regarding secondary collections that belong to a bundle.                 |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#145`_ As a developer, I want to include supplemental file data sizes in the registry                                         |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#146`_ As a node operator, I want the the registry schema to update autonomously when new data is ingested.                   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#147`_ As a node operator,  I want to be able to tag ingested data with the node it is ingested by.                           |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

----

pds-wds-web
-----------
*PDS Web Design System - Basic web implementation*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds-web>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-wds-web>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-wds-web/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds-wds-web/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-wds-web/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-wds-web/releases>`_ 


Bug
~~~

+------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                     |Priority / Bug Severity   |
+==========================================================================================+==========================+
|`pds-wds-web#9`_ App Bar causes usability issues on mobile                                |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|`pds-wds-web#10`_ PDS App Bar does not work if it's included after the DOM loads          |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|`pds-wds-web#15`_ App Bar breaks facet selection on Photojournal Beta                     |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|`pds-wds-web#19`_ Update NAIF in App Bar                                                  |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+----------------------------------------------------------------+--------------------------+
|Issue                                                           |Priority / Bug Severity   |
+================================================================+==========================+
|`pds-wds-web#12`_ Show screenshot of app-bar in README          |unknown                   |
+----------------------------------------------------------------+--------------------------+
|`pds-wds-web#17`_ App Bar Node List Reordering                  |unknown                   |
+----------------------------------------------------------------+--------------------------+

----

PDS.nasa.gov-Search
-------------------
*Front-end interface for PDS.nasa.gov data search capability*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS.nasa.gov-Search#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS.nasa.gov-Search>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS.nasa.gov-Search/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS.nasa.gov-Search/releases>`_ 


Enhancement
~~~~~~~~~~~

+----------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                               |Priority / Bug Severity   |
+====================================================================================================+==========================+
|`PDS.nasa.gov-Search#20`_ Search Details Page / DOI Landing Page                                    |unknown                   |
+----------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-Search#29`_ Iterate with DOI Working Group for improvements to landing pages          |unknown                   |
+----------------------------------------------------------------------------------------------------+--------------------------+
----

PDS.nasa.gov-UX
---------------
*PDS.nasa.gov User Experience Task Issue and Prototype repository*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS.nasa.gov-UX#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS.nasa.gov-UX>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases>`_ 


Enhancement
~~~~~~~~~~~

+----------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                           |Priority / Bug Severity   |
+================================================================================================================+==========================+
|`PDS.nasa.gov-UX#3`_ Formulate user stories for prototype                                                       |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#5`_ Synthesize interview results into user research knowledge base and produce report          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#6`_ Model workflows and initial design directions                                              |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#8`_ Design mockups and develop Figma prototype                                                 |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#61`_ Refine user interview and survey analysis per MC comments                                 |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#70`_ Refine PDS Web Modernization working group plan                                           |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#71`_ Upload all data from airtable / survey to GDrive                                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#73`_ Rev 3 of milestones to breakdown of notional goals and deliverables                       |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+

----

pds4-information-model
----------------------
*The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-information-model/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-information-model>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-information-model/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds4-information-model/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-information-model/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-information-model/releases>`_ 


Bug
~~~

+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                         |Priority / Bug Severity   |
+==============================================================================================================================================+==========================+
|`pds4-information-model#175`_ LDDTool: Displaying invalid Imaging Discipline Classes                                                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#188`_ LDDTool: requires one class with (element_flag = true), even when no classes defined                            |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#266`_ Throw WARNING message when enumeration_flag = false but enumerations are specified                              |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#271`_ LDDTool forces use of LDD versions based upon config                                                            |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#277`_ LDD versionId list in the Data Dictionary Document introduction does not contain valid versionIds               |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#280`_ CSV files fail to escape double quotes.                                                                         |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#283`_ LDDTool generated LIDs for XML Schema Label Products  do not contain IM or LDD Version Ids                      |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#302`_ LDDTool does not allow the bundle to be specified for generated dictionaries                                    |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#304`_ LDDTool does include the PSA namespace                                                                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#312`_ LDDTool does not generate the complete "All LDD" version of the  WebHelp PDS4 Data Dictionary Document          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#316`_ The 1F00 directory is missing from the Data directory for the 1G00 development release.                         |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#322`_ LDDTool generates a 1C00 file when -V 1B00 is specified                                                         |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#327`_ Repo tests fail when trying to run back-to-back maven steps                                                     |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#328`_ LDDTool outputs invalid schema with v13.0.0                                                                     |s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#331`_ Invalid output schema when trying to set an Internal_Reference reference_type value set                         |s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+----------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                           |Priority / Bug Severity   |
+================================================================================================================+==========================+
|`pds4-information-model#167`_ LDDTool: Use sch:value-of to display a variable in Schematron validation          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#238`_ Continuing refactoring of IMTool / LDDTool                                        |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#241`_ Improvements from Build 11.0 testing                                              |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#242`_ DocBook HTML/WebHelp generation and conversion processes                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#293`_ Update JSON output to include dependencies in output                              |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#298`_ Add title to Rule Assertion to allow generation of regression tests.              |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#332`_ [namespace-registry] add new namespace "<clementine>"                             |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+

----

pds4-jparser
------------
*Java Library providing APIs for parsing and exporting information on PDS4 products, including table and image objects to various formats including CSV, PNG, VICAR, FITs, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-jparser/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-jparser>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-jparser/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/pds4-jparser/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-jparser/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-jparser/releases>`_ 


Bug
~~~

+---------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                        |Priority / Bug Severity   |
+=============================================================================================+==========================+
|`pds4-jparser#21`_ Update table reads for large files and improve memory footprints          |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+
|`pds4-jparser#32`_ NIO Library causes error when trying to build with openJDK 8              |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+
|`pds4-jparser#36`_ NoSuchMethodError: java.nio.ByteBuffer with Java9 Builds                  |s.medium                  |
+---------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------+--------------------------+
|Issue                                                                  |Priority / Bug Severity   |
+=======================================================================+==========================+
|`pds4-jparser#33`_ Upgrade pds4-jparser to build with Java11+          |unknown                   |
+-----------------------------------------------------------------------+--------------------------+

----

PLAID
-----
*APPS PDS Label Assistant for Interactive Design (PLAID). See an overview of the software on YouTube. https://www.youtube.com/watch?v=WCo8erW_rL8*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://plaid.jpl.nasa.gov>`_
     - `Github Repo <https://github.com/NASA-PDS/PLAID>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PLAID/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/PLAID/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PLAID/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PLAID/releases>`_ 


Enhancement
~~~~~~~~~~~

+------------------------------------------------------------------------------+--------------------------+
|Issue                                                                         |Priority / Bug Severity   |
+==============================================================================+==========================+
|`PLAID#10`_ Develop procedure for how to update PLAID with latest IM          |unknown                   |
+------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+----------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                               |Priority / Bug Severity   |
+====================================================================================================+==========================+
|`PLAID#15`_ As a PDS Operator, I want to update PLAID to the latest PDS4 Information Model          |unknown                   |
+----------------------------------------------------------------------------------------------------+--------------------------+

----

registry-api-service
--------------------
*PDS Registry API service. Complies with PDS API specification*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-api-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-api-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-api-service/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/registry-api-service/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-api-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-api-service/releases>`_ 


Bug
~~~

+------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                 |Priority / Bug Severity   |
+======================================================================================================+==========================+
|`registry-api-service#16`_ API server crashes with OutOfMemoryError if invalid query is used          |s.high                    |
+------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#17`_ error 500 on GET /collections/:lidvid:/products                            |s.high                    |
+------------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                    |Priority / Bug Severity   |
+=========================================================================================+==========================+
|`registry-api-service#2`_ Manage relationships bundle-collection-product in API          |unknown                   |
+-----------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#3`_ implement the start/limit efficiently                          |unknown                   |
+-----------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#4`_ Implement a lid resolver                                       |unknown                   |
+-----------------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                     |Priority / Bug Severity   |
+==========================================================================================================================+==========================+
|`registry-api-service#14`_ As a node operators, I want to deploy the Registry API Service with the PDS Registry.          |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------+--------------------------+

----

tracking-service
----------------
*Provides functionality for tracking status and other aspects pertaining to PDS products that are not captured in the Registry Service.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/tracking-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/tracking-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/tracking-service/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/tracking-service/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/tracking-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/tracking-service/releases>`_ 


Bug
~~~

+---------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                              |Priority / Bug Severity   |
+===================================================================================================+==========================+
|`tracking-service#18`_ tracking front page does not keep tracking in relative anchor href          |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+------------------------------------------------------------------------+--------------------------+
|Issue                                                                   |Priority / Bug Severity   |
+========================================================================+==========================+
|`tracking-service#10`_ Dockerize Tracking Service                       |unknown                   |
+------------------------------------------------------------------------+--------------------------+
|`tracking-service#14`_ Add mysql database to docker deployment          |unknown                   |
+------------------------------------------------------------------------+--------------------------+

----

validate
--------
*Validates PDS4 product labels, data and PDS3 Volumes*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/validate/>`_
     - `Github Repo <https://github.com/NASA-PDS/validate>`_
     - `Issue Tracking <https://github.com/NASA-PDS/validate/issues>`_ 
     - `Up Next <https://github.com/NASA-PDS/validate/issues?q=is%3Aopen+is%3Aissue+label%3AB12.0>`_ 
     - `Stable Release <https://github.com/NASA-PDS/validate/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/validate/releases>`_ 


Bug
~~~

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                              |Priority / Bug Severity   |
+===================================================================================================================================================================+==========================+
|`validate#5`_ Improve file base name check according to Standards Reference                                                                                        |s.low                     |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#6`_ Improve pds4.bundle unlabeled files check to handle files without a file suffix                                                                      |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#11`_ Update allowable field_format values per Standards Reference definition regarding [+-] characters                                                   |s.low                     |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#153`_ Update validate to throw error when a file has a space in the filename                                                                             |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#189`_ Validate error reading tables > 2GiB                                                                                                               |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#240`_ Unexpected error for data collection in a sub-directory                                                                                            |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#256`_ validate should only do integrity checking on latest version of a collection when referenced by LID                                                |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#257`_ Product with incorrect table binary definition pass validation                                                                                     |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#260`_ Missing documentation about deprecated flags                                                                                                       |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#271`_ validate 1.25.0-SNAPSHOT raises an exception when validating a product                                                                             |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#273`_ Bug performing bundle validation with nested directories                                                                                           |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#278`_ Registered context products file does not retain older versions of context products                                                                |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#281`_ Validate fails to report error in   File.file_size                                                                                                 |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#291`_ When validating a product with a bad schematron definition, bundle validation also fails indicating the associated product does not exist          |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#294`_ Content validation incorrectly reports error for floating-point values out of specified min/max range                                              |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#297`_ Content validation of ASCII_Integer field does not accept value with leading zeroes                                                                |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#298`_ validate misses double quotes within a delimited table                                                                                             |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#299`_ Validate tool does not PASS a bundle with a single-character filename                                                                              |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#300`_ validate -u flag reports an error on Windows                                                                                                       |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#301`_ unclear error message for field count matching                                                                                                     |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#310`_ Validate missing collections in bundle after CCB-282 updates                                                                                       |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#325`_ Validate Incorrectly Throws Error When Embedded Field_Character Contains <CR><LF>                                                                  |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#326`_ File-size check fails for large data files                                                                                                         |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#327`_ validate fails to process large data file                                                                                                          |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancement
~~~~~~~~~~~

+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                   |Priority / Bug Severity   |
+========================================================================================================================+==========================+
|`validate#17`_ Validate schematron references and throw fatal error if invalid URI specified                            |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#24`_ Update context check to retrieve and use latest context products from EN Registry                        |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#51`_ Provide the capability to specify multiple locations for pds4.bundle validation                          |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#81`_ Validate and throw error when duplicate LIDs are found in Bundle                                         |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#230`_ Update validate per SR Requirements for collection inventories                                          |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#238`_ validate does not perform full bundle validation when using a specific bundle.xml                       |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#246`_ Add output directory flag to validate-bundle tool                                                       |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#249`_ Improvements for validating accumulating bundles / collections                                          |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#252`_ Implement initial behavioral testing framework with cucumber                                            |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#254`_ validate does not perform expediently when doing bundle-level validation against large bundles          |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#264`_ Update installation documentation to include 64-bit Java as system Requirement                          |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#290`_ Migrate subset of existing regression tests to cucumber behavioral testing                              |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#322`_ Update installation documentation to require Java 1.9+                                                  |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#323`_ Upgrade to Java 9+                                                                                      |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+

Requirement
~~~~~~~~~~~

+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                             |Priority / Bug Severity   |
+==================================================================================================================================================================+==========================+
|`validate#57`_ As a user, I want to be warned when there are alphanumeric characters between fields in Table_Character                                            |p.could-have              |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#149`_ As a user, I want validate to check number of records/fields specified in label matches the records in the actual data table                      |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#164`_ As a user, I want to validate PDF files are PDF/A                                                                                                 |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#188`_ As a user, I want to validate a bundle that uses multiple versions of the Information Model / Discipline LDDs                                     |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#210`_ As a user, I want validate to raise a WARNING when differing versions of IM are used within a bundle                                              |p.could-have              |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#292`_ CCB-264: Make the Line Feed (LF) character an allowed record delimiter                                                                            |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#303`_ As a user, I want to the raise a WARNING if the object-defined size in the label does not match the file_size value                               |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

----

Theme
~~~~~

+--------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                               |Priority / Bug Severity   |
+====================================================================================================================+==========================+
|`validate#250`_ Improvements to meet updated Standards Reference since initial Requirements implementation          |unknown                   |
+--------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#318`_ B12.0 Content Validation Improvements                                                               |unknown                   |
+--------------------------------------------------------------------------------------------------------------------+--------------------------+
----

Liens
=====

+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Issue                                                      |Title                                           |Rationale                                                                                                                                                                                                                                                                                                                                                                              |
+===========================================================+================================================+=======================================================================================================================================================================================================================================================================================================================================================================================+
|`pds-swg#7`_ [CR] Defer PDS UX Tasks to B12.0                |[CR] Defer PDS UX Tasks to B12.0                |Deferring these tasks to B12.0 in order to develop a comprehensive, detailed plan, milestones, and activities for a PDS Web Modernization Team. https://github.com/nasa-pds/pds.nasa.gov-ux/issues/70                                                                                                                                                                                  |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|`pds-swg#6`_ [CR] Defer PDS API Tasks to B12.0               |[CR] Defer PDS API Tasks to B12.0               |Inaccurate estimates for time to complete other designs and implementations with PDS API WG.                                                                                                                                                                                                                                                                                           |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|`pds-swg#5`_ [CR] Defer Tracking Service Tasks to B12.0      |[CR] Defer Tracking Service Tasks to B12.0      |Tracking Service design and partial implementation was completed in 2018. Misunderstanding during handoff from previous developers that the software design did not include Requirements definition, and design did not form to common API standards. Caused significant increase in scope for [Requirements definition task](https://github.com/nasa-pds/tracking-service/issues/2)   |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|p`ds-swg#4`_ [CR] Add additional PDS4 SCRs to Release Plan   |[CR] Add additional PDS4 SCRs to Release Plan   |Several additional SCRs passed by the CCB.                                                                                                                                                                                                                                                                                                                                             |
+-----------------------------------------------------------+------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

----


Software Catalog
=================
The Engineering Node-provided Software resources are listed in the `software
release summary (B11.1)`_

Installation and Operation
==========================
PDS Engineering node software are meant to be deployed in 3 contexts:
standalone, discipline nodes or engineering node
For the installation and operation manual see the `users manuals` in the
software summary sections below:

- `PDS Standalone`_

- `PDS Discipline Nodes`_

- `PDS Engineering Node only`_

----


Reference Documents
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

.. _pds4-information-model#255: https://github.com/NASA-PDS/pds4-information-model/issues/255
.. _pds4-information-model#257: https://github.com/NASA-PDS/pds4-information-model/issues/257
.. _pds4-information-model#252: https://github.com/NASA-PDS/pds4-information-model/issues/252
.. _pds4-information-model#254: https://github.com/NASA-PDS/pds4-information-model/issues/254
.. _pds4-information-model#253: https://github.com/NASA-PDS/pds4-information-model/issues/253
.. _pds4-information-model#250: https://github.com/NASA-PDS/pds4-information-model/issues/250
.. _pds4-information-model#288: https://github.com/NASA-PDS/pds4-information-model/issues/288
.. _pds4-information-model#339: https://github.com/NASA-PDS/pds4-information-model/issues/339
.. _api-search-query-lexer#1: https://github.com/NASA-PDS/api-search-query-lexer/issues/1
.. _archive-analytics#2: https://github.com/NASA-PDS/archive-analytics/issues/2
.. _archive-analytics#7: https://github.com/NASA-PDS/archive-analytics/issues/7
.. _archive-analytics#10: https://github.com/NASA-PDS/archive-analytics/issues/10
.. _harvest#6: https://github.com/NASA-PDS/harvest/issues/6
.. _harvest#18: https://github.com/NASA-PDS/harvest/issues/18
.. _harvest#37: https://github.com/NASA-PDS/harvest/issues/37
.. _harvest#45: https://github.com/NASA-PDS/harvest/issues/45
.. _mi-label#10: https://github.com/NASA-PDS/mi-label/issues/10
.. _pds-api#73: https://github.com/NASA-PDS/pds-api/issues/73
.. _pds-api#31: https://github.com/NASA-PDS/pds-api/issues/31
.. _pds-api#12: https://github.com/NASA-PDS/pds-api/issues/12
.. _pds-api#17: https://github.com/NASA-PDS/pds-api/issues/17
.. _pds-api#34: https://github.com/NASA-PDS/pds-api/issues/34
.. _pds-api#35: https://github.com/NASA-PDS/pds-api/issues/35
.. _pds-api#40: https://github.com/NASA-PDS/pds-api/issues/40
.. _pds-api#41: https://github.com/NASA-PDS/pds-api/issues/41
.. _pds-api#43: https://github.com/NASA-PDS/pds-api/issues/43
.. _pds-api#47: https://github.com/NASA-PDS/pds-api/issues/47
.. _pds-api#52: https://github.com/NASA-PDS/pds-api/issues/52
.. _pds-api#54: https://github.com/NASA-PDS/pds-api/issues/54
.. _pds-api#56: https://github.com/NASA-PDS/pds-api/issues/56
.. _pds-api#59: https://github.com/NASA-PDS/pds-api/issues/59
.. _pds-api#60: https://github.com/NASA-PDS/pds-api/issues/60
.. _pds-api#61: https://github.com/NASA-PDS/pds-api/issues/61
.. _pds-api#62: https://github.com/NASA-PDS/pds-api/issues/62
.. _pds-api#64: https://github.com/NASA-PDS/pds-api/issues/64
.. _pds-api-client#2: https://github.com/NASA-PDS/pds-api-client/issues/2
.. _pds-api-javalib#1: https://github.com/NASA-PDS/pds-api-javalib/issues/1
.. _pds-api-javalib#2: https://github.com/NASA-PDS/pds-api-javalib/issues/2
.. _pds-deep-archive#90: https://github.com/NASA-PDS/pds-deep-archive/issues/90
.. _pds-deep-archive#92: https://github.com/NASA-PDS/pds-deep-archive/issues/92
.. _pds-deep-archive#99: https://github.com/NASA-PDS/pds-deep-archive/issues/99
.. _pds-deep-archive#93: https://github.com/NASA-PDS/pds-deep-archive/issues/93
.. _pds-deep-archive#95: https://github.com/NASA-PDS/pds-deep-archive/issues/95
.. _pds-deep-archive#7: https://github.com/NASA-PDS/pds-deep-archive/issues/7
.. _pds-deep-archive#102: https://github.com/NASA-PDS/pds-deep-archive/issues/102
.. _pds-doi-service#119: https://github.com/NASA-PDS/pds-doi-service/issues/119
.. _pds-doi-service#121: https://github.com/NASA-PDS/pds-doi-service/issues/121
.. _pds-doi-service#122: https://github.com/NASA-PDS/pds-doi-service/issues/122
.. _pds-doi-service#126: https://github.com/NASA-PDS/pds-doi-service/issues/126
.. _pds-doi-service#128: https://github.com/NASA-PDS/pds-doi-service/issues/128
.. _pds-doi-service#138: https://github.com/NASA-PDS/pds-doi-service/issues/138
.. _pds-doi-service#141: https://github.com/NASA-PDS/pds-doi-service/issues/141
.. _pds-doi-service#143: https://github.com/NASA-PDS/pds-doi-service/issues/143
.. _pds-doi-service#150: https://github.com/NASA-PDS/pds-doi-service/issues/150
.. _pds-doi-service#154: https://github.com/NASA-PDS/pds-doi-service/issues/154
.. _pds-doi-service#159: https://github.com/NASA-PDS/pds-doi-service/issues/159
.. _pds-doi-service#52: https://github.com/NASA-PDS/pds-doi-service/issues/52
.. _pds-doi-service#91: https://github.com/NASA-PDS/pds-doi-service/issues/91
.. _pds-doi-service#114: https://github.com/NASA-PDS/pds-doi-service/issues/114
.. _pds-doi-service#116: https://github.com/NASA-PDS/pds-doi-service/issues/116
.. _pds-doi-service#125: https://github.com/NASA-PDS/pds-doi-service/issues/125
.. _pds-doi-service#134: https://github.com/NASA-PDS/pds-doi-service/issues/134
.. _pds-doi-service#135: https://github.com/NASA-PDS/pds-doi-service/issues/135
.. _pds-doi-service#140: https://github.com/NASA-PDS/pds-doi-service/issues/140
.. _pds-doi-service#144: https://github.com/NASA-PDS/pds-doi-service/issues/144
.. _pds-doi-service#148: https://github.com/NASA-PDS/pds-doi-service/issues/148
.. _pds-doi-service#157: https://github.com/NASA-PDS/pds-doi-service/issues/157
.. _pds-doi-service#162: https://github.com/NASA-PDS/pds-doi-service/issues/162
.. _pds-doi-service#163: https://github.com/NASA-PDS/pds-doi-service/issues/163
.. _pds-doi-service#165: https://github.com/NASA-PDS/pds-doi-service/issues/165
.. _pds-doi-service#167: https://github.com/NASA-PDS/pds-doi-service/issues/167
.. _pds-doi-service#177: https://github.com/NASA-PDS/pds-doi-service/issues/177
.. _pds-doi-service#180: https://github.com/NASA-PDS/pds-doi-service/issues/180
.. _pds-doi-service#183: https://github.com/NASA-PDS/pds-doi-service/issues/183
.. _pds-doi-service#184: https://github.com/NASA-PDS/pds-doi-service/issues/184
.. _pds-doi-ui#35: https://github.com/NASA-PDS/pds-doi-ui/issues/35
.. _pds-doi-ui#1: https://github.com/NASA-PDS/pds-doi-ui/issues/1
.. _pds-doi-ui#9: https://github.com/NASA-PDS/pds-doi-ui/issues/9
.. _pds-doi-ui#10: https://github.com/NASA-PDS/pds-doi-ui/issues/10
.. _pds-doi-ui#14: https://github.com/NASA-PDS/pds-doi-ui/issues/14
.. _pds-doi-ui#17: https://github.com/NASA-PDS/pds-doi-ui/issues/17
.. _pds-doi-ui#19: https://github.com/NASA-PDS/pds-doi-ui/issues/19
.. _pds-doi-ui#27: https://github.com/NASA-PDS/pds-doi-ui/issues/27
.. _pds-doi-ui#28: https://github.com/NASA-PDS/pds-doi-ui/issues/28
.. _pds-doi-ui#30: https://github.com/NASA-PDS/pds-doi-ui/issues/30
.. _pds-doi-ui#31: https://github.com/NASA-PDS/pds-doi-ui/issues/31
.. _pds-doi-ui#25: https://github.com/NASA-PDS/pds-doi-ui/issues/25
.. _pds-doi-ui#34: https://github.com/NASA-PDS/pds-doi-ui/issues/34
.. _pds-registry-app#108: https://github.com/NASA-PDS/pds-registry-app/issues/108
.. _pds-registry-app#109: https://github.com/NASA-PDS/pds-registry-app/issues/109
.. _pds-registry-app#110: https://github.com/NASA-PDS/pds-registry-app/issues/110
.. _pds-registry-app#135: https://github.com/NASA-PDS/pds-registry-app/issues/135
.. _pds-registry-app#20: https://github.com/NASA-PDS/pds-registry-app/issues/20
.. _pds-registry-app#27: https://github.com/NASA-PDS/pds-registry-app/issues/27
.. _pds-registry-app#102: https://github.com/NASA-PDS/pds-registry-app/issues/102
.. _pds-registry-app#103: https://github.com/NASA-PDS/pds-registry-app/issues/103
.. _pds-registry-app#113: https://github.com/NASA-PDS/pds-registry-app/issues/113
.. _pds-registry-app#122: https://github.com/NASA-PDS/pds-registry-app/issues/122
.. _pds-registry-app#123: https://github.com/NASA-PDS/pds-registry-app/issues/123
.. _pds-registry-app#129: https://github.com/NASA-PDS/pds-registry-app/issues/129
.. _pds-registry-app#131: https://github.com/NASA-PDS/pds-registry-app/issues/131
.. _pds-registry-app#57: https://github.com/NASA-PDS/pds-registry-app/issues/57
.. _pds-registry-app#58: https://github.com/NASA-PDS/pds-registry-app/issues/58
.. _pds-registry-app#59: https://github.com/NASA-PDS/pds-registry-app/issues/59
.. _pds-registry-app#75: https://github.com/NASA-PDS/pds-registry-app/issues/75
.. _pds-registry-app#56: https://github.com/NASA-PDS/pds-registry-app/issues/56
.. _pds-registry-app#73: https://github.com/NASA-PDS/pds-registry-app/issues/73
.. _pds-registry-app#72: https://github.com/NASA-PDS/pds-registry-app/issues/72
.. _pds-registry-app#71: https://github.com/NASA-PDS/pds-registry-app/issues/71
.. _pds-registry-app#70: https://github.com/NASA-PDS/pds-registry-app/issues/70
.. _pds-registry-app#55: https://github.com/NASA-PDS/pds-registry-app/issues/55
.. _pds-registry-app#68: https://github.com/NASA-PDS/pds-registry-app/issues/68
.. _pds-registry-app#67: https://github.com/NASA-PDS/pds-registry-app/issues/67
.. _pds-registry-app#66: https://github.com/NASA-PDS/pds-registry-app/issues/66
.. _pds-registry-app#65: https://github.com/NASA-PDS/pds-registry-app/issues/65
.. _pds-registry-app#141: https://github.com/NASA-PDS/pds-registry-app/issues/141
.. _pds-registry-app#142: https://github.com/NASA-PDS/pds-registry-app/issues/142
.. _pds-registry-app#143: https://github.com/NASA-PDS/pds-registry-app/issues/143
.. _pds-registry-app#144: https://github.com/NASA-PDS/pds-registry-app/issues/144
.. _pds-registry-app#145: https://github.com/NASA-PDS/pds-registry-app/issues/145
.. _pds-registry-app#146: https://github.com/NASA-PDS/pds-registry-app/issues/146
.. _pds-registry-app#147: https://github.com/NASA-PDS/pds-registry-app/issues/147
.. _pds-wds-web#9: https://github.com/NASA-PDS/pds-wds-web/issues/9
.. _pds-wds-web#10: https://github.com/NASA-PDS/pds-wds-web/issues/10
.. _pds-wds-web#15: https://github.com/NASA-PDS/pds-wds-web/issues/15
.. _pds-wds-web#19: https://github.com/NASA-PDS/pds-wds-web/issues/19
.. _pds-wds-web#12: https://github.com/NASA-PDS/pds-wds-web/issues/12
.. _pds-wds-web#17: https://github.com/NASA-PDS/pds-wds-web/issues/17
.. _PDS.nasa.gov-Search#20: https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/20
.. _PDS.nasa.gov-Search#29: https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/29
.. _PDS.nasa.gov-UX#3: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/3
.. _PDS.nasa.gov-UX#5: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/5
.. _PDS.nasa.gov-UX#6: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/6
.. _PDS.nasa.gov-UX#8: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/8
.. _PDS.nasa.gov-UX#61: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/61
.. _PDS.nasa.gov-UX#70: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/70
.. _PDS.nasa.gov-UX#71: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/71
.. _PDS.nasa.gov-UX#73: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/73
.. _pds4-information-model#175: https://github.com/NASA-PDS/pds4-information-model/issues/175
.. _pds4-information-model#188: https://github.com/NASA-PDS/pds4-information-model/issues/188
.. _pds4-information-model#266: https://github.com/NASA-PDS/pds4-information-model/issues/266
.. _pds4-information-model#271: https://github.com/NASA-PDS/pds4-information-model/issues/271
.. _pds4-information-model#277: https://github.com/NASA-PDS/pds4-information-model/issues/277
.. _pds4-information-model#280: https://github.com/NASA-PDS/pds4-information-model/issues/280
.. _pds4-information-model#283: https://github.com/NASA-PDS/pds4-information-model/issues/283
.. _pds4-information-model#302: https://github.com/NASA-PDS/pds4-information-model/issues/302
.. _pds4-information-model#304: https://github.com/NASA-PDS/pds4-information-model/issues/304
.. _pds4-information-model#312: https://github.com/NASA-PDS/pds4-information-model/issues/312
.. _pds4-information-model#316: https://github.com/NASA-PDS/pds4-information-model/issues/316
.. _pds4-information-model#322: https://github.com/NASA-PDS/pds4-information-model/issues/322
.. _pds4-information-model#327: https://github.com/NASA-PDS/pds4-information-model/issues/327
.. _pds4-information-model#328: https://github.com/NASA-PDS/pds4-information-model/issues/328
.. _pds4-information-model#331: https://github.com/NASA-PDS/pds4-information-model/issues/331
.. _pds4-information-model#167: https://github.com/NASA-PDS/pds4-information-model/issues/167
.. _pds4-information-model#238: https://github.com/NASA-PDS/pds4-information-model/issues/238
.. _pds4-information-model#241: https://github.com/NASA-PDS/pds4-information-model/issues/241
.. _pds4-information-model#242: https://github.com/NASA-PDS/pds4-information-model/issues/242
.. _pds4-information-model#293: https://github.com/NASA-PDS/pds4-information-model/issues/293
.. _pds4-information-model#298: https://github.com/NASA-PDS/pds4-information-model/issues/298
.. _pds4-information-model#332: https://github.com/NASA-PDS/pds4-information-model/issues/332
.. _pds4-jparser#21: https://github.com/NASA-PDS/pds4-jparser/issues/21
.. _pds4-jparser#32: https://github.com/NASA-PDS/pds4-jparser/issues/32
.. _pds4-jparser#36: https://github.com/NASA-PDS/pds4-jparser/issues/36
.. _pds4-jparser#33: https://github.com/NASA-PDS/pds4-jparser/issues/33
.. _PLAID#10: https://github.com/NASA-PDS/PLAID/issues/10
.. _PLAID#15: https://github.com/NASA-PDS/PLAID/issues/15
.. _registry-api-service#16: https://github.com/NASA-PDS/registry-api-service/issues/16
.. _registry-api-service#17: https://github.com/NASA-PDS/registry-api-service/issues/17
.. _registry-api-service#2: https://github.com/NASA-PDS/registry-api-service/issues/2
.. _registry-api-service#3: https://github.com/NASA-PDS/registry-api-service/issues/3
.. _registry-api-service#4: https://github.com/NASA-PDS/registry-api-service/issues/4
.. _registry-api-service#14: https://github.com/NASA-PDS/registry-api-service/issues/14
.. _tracking-service#18: https://github.com/NASA-PDS/tracking-service/issues/18
.. _tracking-service#10: https://github.com/NASA-PDS/tracking-service/issues/10
.. _tracking-service#14: https://github.com/NASA-PDS/tracking-service/issues/14
.. _validate#5: https://github.com/NASA-PDS/validate/issues/5
.. _validate#6: https://github.com/NASA-PDS/validate/issues/6
.. _validate#11: https://github.com/NASA-PDS/validate/issues/11
.. _validate#153: https://github.com/NASA-PDS/validate/issues/153
.. _validate#189: https://github.com/NASA-PDS/validate/issues/189
.. _validate#240: https://github.com/NASA-PDS/validate/issues/240
.. _validate#256: https://github.com/NASA-PDS/validate/issues/256
.. _validate#257: https://github.com/NASA-PDS/validate/issues/257
.. _validate#260: https://github.com/NASA-PDS/validate/issues/260
.. _validate#271: https://github.com/NASA-PDS/validate/issues/271
.. _validate#273: https://github.com/NASA-PDS/validate/issues/273
.. _validate#278: https://github.com/NASA-PDS/validate/issues/278
.. _validate#281: https://github.com/NASA-PDS/validate/issues/281
.. _validate#291: https://github.com/NASA-PDS/validate/issues/291
.. _validate#294: https://github.com/NASA-PDS/validate/issues/294
.. _validate#297: https://github.com/NASA-PDS/validate/issues/297
.. _validate#298: https://github.com/NASA-PDS/validate/issues/298
.. _validate#299: https://github.com/NASA-PDS/validate/issues/299
.. _validate#300: https://github.com/NASA-PDS/validate/issues/300
.. _validate#301: https://github.com/NASA-PDS/validate/issues/301
.. _validate#310: https://github.com/NASA-PDS/validate/issues/310
.. _validate#325: https://github.com/NASA-PDS/validate/issues/325
.. _validate#326: https://github.com/NASA-PDS/validate/issues/326
.. _validate#327: https://github.com/NASA-PDS/validate/issues/327
.. _validate#17: https://github.com/NASA-PDS/validate/issues/17
.. _validate#24: https://github.com/NASA-PDS/validate/issues/24
.. _validate#51: https://github.com/NASA-PDS/validate/issues/51
.. _validate#81: https://github.com/NASA-PDS/validate/issues/81
.. _validate#230: https://github.com/NASA-PDS/validate/issues/230
.. _validate#238: https://github.com/NASA-PDS/validate/issues/238
.. _validate#246: https://github.com/NASA-PDS/validate/issues/246
.. _validate#249: https://github.com/NASA-PDS/validate/issues/249
.. _validate#252: https://github.com/NASA-PDS/validate/issues/252
.. _validate#254: https://github.com/NASA-PDS/validate/issues/254
.. _validate#264: https://github.com/NASA-PDS/validate/issues/264
.. _validate#290: https://github.com/NASA-PDS/validate/issues/290
.. _validate#322: https://github.com/NASA-PDS/validate/issues/322
.. _validate#323: https://github.com/NASA-PDS/validate/issues/323
.. _validate#57: https://github.com/NASA-PDS/validate/issues/57
.. _validate#149: https://github.com/NASA-PDS/validate/issues/149
.. _validate#164: https://github.com/NASA-PDS/validate/issues/164
.. _validate#188: https://github.com/NASA-PDS/validate/issues/188
.. _validate#210: https://github.com/NASA-PDS/validate/issues/210
.. _validate#292: https://github.com/NASA-PDS/validate/issues/292
.. _validate#303: https://github.com/NASA-PDS/validate/issues/303
.. _validate#308: https://github.com/NASA-PDS/validate/issues/308
.. _validate#250: https://github.com/NASA-PDS/validate/issues/250
.. _validate#318: https://github.com/NASA-PDS/validate/issues/318
.. _pds-swg#7: https://github.com/NASA-PDS/pds-swg/issues/7
.. _pds-swg#6: https://github.com/NASA-PDS/pds-swg/issues/6
.. _pds-swg#5: https://github.com/NASA-PDS/pds-swg/issues/5
.. _pds-swg#4: https://github.com/NASA-PDS/pds-swg/issues/4
.. _software release summary (B11.1): https://nasa-pds.github.io/releases/B11.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Sotware Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/main/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/main/docs/design/pds-doi-service-srd.md
