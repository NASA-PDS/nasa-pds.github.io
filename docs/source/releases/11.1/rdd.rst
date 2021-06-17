=========================================
Release Description Document (build 11.1)
=========================================
Software changes
----------------
api-search-query-lexer
~~~~~~~~~~~~~~~~~~~~~~
*Lexer to parse the search query of the PDS API*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/api-search-query-lexer#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/api-search-query-lexer>`_
     - `Issue Tracking <https://github.com/NASA-PDS/api-search-query-lexer/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/api-search-query-lexer/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/api-search-query-lexer/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/api-search-query-lexer/releases>`_ 


bug
+++

+------------------------------------------------------------------------+--------------------------+
|Issue                                                                   |Priority / Bug Severity   |
+========================================================================+==========================+
|NASA-PDS/api-search-query-lexer_1_ parsing of string does not succeed   |unknown                   |
+------------------------------------------------------------------------+--------------------------+

archive-analytics
~~~~~~~~~~~~~~~~~
*Processes, tools, and configuration for managing PDS archive analytics software and reports*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/archive-analytics#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/archive-analytics>`_
     - `Issue Tracking <https://github.com/NASA-PDS/archive-analytics/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/archive-analytics/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/archive-analytics/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/archive-analytics/releases>`_ 


requirement
+++++++++++

+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                         |Priority / Bug Severity   |
+==============================================================================================================================+==========================+
|NASA-PDS/archive-analytics_2_ As a manager, I want to know the current total volume of PDS holdings                           |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/archive-analytics_7_ As a PDS Project Office, I want to know the historical total volume of PDS holdings over time   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/archive-analytics_10_ As a Node Manager, I want to report on the number of artifacts within the archive              |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+

harvest
~~~~~~~
*Provides software provides functionality for capturing and indexing product metadata in PDS Registry. A sub-component of the PDS Registry App (https://github.com/NASA-PDS/pds-registry-app)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app>`_
     - `Github Repo <https://github.com/NASA-PDS/harvest>`_
     - `Issue Tracking <https://github.com/NASA-PDS/harvest/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/harvest/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/harvest/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/harvest/releases>`_ 


bug
+++

+---------------------------------------------------------------------------------+--------------------------+
|Issue                                                                            |Priority / Bug Severity   |
+=================================================================================+==========================+
|NASA-PDS/harvest_6_ Check input URIs to avoid potential security vulnerability   |s.low                     |
+---------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+--------------------------------------------------------+--------------------------+
|Issue                                                   |Priority / Bug Severity   |
+========================================================+==========================+
|NASA-PDS/harvest_18_ Track collection file inventory    |unknown                   |
+--------------------------------------------------------+--------------------------+

requirement
+++++++++++

+---------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================+==========================+
|NASA-PDS/harvest_37_ As a user, I want a default configuration for harvest included in the tool package        |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/harvest_45_ As a user, I want to be able to ingest a directory of data that is not part of a bundle   |unknown                   |
+---------------------------------------------------------------------------------------------------------------+--------------------------+

mi-label
~~~~~~~~
*Metadata Injector for PDS Labels (MILabel), formerly known as Generate Tool*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/mi-label/>`_
     - `Github Repo <https://github.com/NASA-PDS/mi-label>`_
     - `Issue Tracking <https://github.com/NASA-PDS/mi-label/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/mi-label/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/mi-label/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/mi-label/releases>`_ 


bug
+++

+--------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                 |Priority / Bug Severity   |
+======================================================================================+==========================+
|NASA-PDS/mi-label_10_ Windows version will not run because of error in generate.bat   |s.high                    |
+--------------------------------------------------------------------------------------+--------------------------+

pds-api
~~~~~~~
*PDS API Application with client and server integrated into one package*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 


bug
+++

+------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                 |Priority / Bug Severity   |
+======================================================================================================+==========================+
|NASA-PDS/pds-api_73_ As a n00b paginator, there might be an off-by-1 error in the `limit` parameter   |s.medium                  |
+------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                       |Priority / Bug Severity   |
+============================================================================================================================+==========================+
|NASA-PDS/pds-api_31_ Streamline testing of API server implementation                                                        |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_12_ Initial Query Syntax Lexer Implementation                                                              |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_17_ Define initial structure for response format conventions and parameter definition                      |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_34_ Deploy PDS API v0 (alpha) for beta testing                                                             |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_35_ Initial Federated API implementation                                                                   |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_40_ add lexer to registry api                                                                              |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_41_ Manage field preselection in queries                                                                   |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_43_ Implement content negotiation                                                                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_47_ develop a jupyter notebook demo where a user can browse PDS archive from bundle to product data file   |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_52_ Get investigation area/targets/instruments from external ids                                           |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================================+==========================+
|NASA-PDS/pds-api_54_ As an API user, I want to perform a search using wildcards                                                |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_56_ As an API user, I want to know the children and ancestors of bundle, collections, and products            |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_59_ As an API user, I want to know the Product(s) that belong to a given Bundle.                              |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_60_ As an API user, I want to know the Bundle for a given Product.                                            |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_61_ As an API user, I want to know the Collection(s) for a given Product.                                     |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_62_ As an API user, I want to know the Bundle for a given Collection.                                         |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api_64_ As a user, when I request specific fields I want to get records which have at least one of these fields   |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------------+

pds-api-client
~~~~~~~~~~~~~~
*PDS API Client*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-api-client/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api-client>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api-client/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api-client/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api-client/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api-client/releases>`_ 


bug
+++

+------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                               |Priority / Bug Severity   |
+====================================================================================+==========================+
|NASA-PDS/pds-api-client_2_ PDS API Client 1.0.0 cannot communicate with pds-gamma   |s.high                    |
+------------------------------------------------------------------------------------+--------------------------+

pds-api-javalib
~~~~~~~~~~~~~~~
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
+++++++++++

+---------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                        |Priority / Bug Severity   |
+=============================================================================================+==========================+
|NASA-PDS/pds-api-javalib_1_ Add time out specification in swaggerHub definition of the API   |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-api-javalib_2_ Add list of available fields in response format                  |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+

pds-deep-archive
~~~~~~~~~~~~~~~~
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
+++

+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                  |Priority / Bug Severity   |
+=======================================================================================================================+==========================+
|NASA-PDS/pds-deep-archive_90_ Small typo on package documentation                                                      |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-deep-archive_92_ SIP manifest table erroneously includes secondary collections and their basic products   |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-deep-archive_99_ aip_label_checksum is not for the correct file                                           |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+-----------------------------------------------------------------------------------+--------------------------+
|Issue                                                                              |Priority / Bug Severity   |
+===================================================================================+==========================+
|NASA-PDS/pds-deep-archive_93_ add year to directory path in URL                    |unknown                   |
+-----------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-deep-archive_95_ Bash required for default installation description   |unknown                   |
+-----------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                     |Priority / Bug Severity   |
+==========================================================================================+==========================+
|NASA-PDS/pds-deep-archive_7_ As a user, I want to generate AIPs and SIPs using Registry   |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-deep-archive_102_ As a user, I want the SIP manifest to include valid URLs   |p.must-have               |
+------------------------------------------------------------------------------------------+--------------------------+

pds-doi-service
~~~~~~~~~~~~~~~
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
+++

+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                |Priority / Bug Severity   |
+=====================================================================================================================================+==========================+
|NASA-PDS/pds-doi-service_119_ Raise a specific exception when the OSTI server is not reachable                                       |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_121_ GET /dois must support empty vid field                                                                 |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_122_ the sqllite database should be created at the same location, whereever the command are launched from   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_126_ get /dois/{lidvid}                                                                                     |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_128_ command pds-doi-cmd list returns update date in timestamp instead of iso8601                           |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_138_ xlsx file extension for reserve not supported                                                          |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_141_ api does not ignore '/' at the end of url                                                              |s.low                     |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_143_ when release command keywords are broken with encoded characters                                       |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_150_ when doing draft with warnings (e.g. duplicated title) the -f option does not help                     |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_154_ draft OSTI label                                                                                       |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_159_ The url /dois/{lidvid} should still return XML in the record attribute                                 |s.critical                |
+-------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                           |Priority / Bug Severity   |
+================================================================================================================================+==========================+
|NASA-PDS/pds-doi-service_52_ API Implementation for DOI Service                                                                 |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_91_ Develop User Access / Management Strategy                                                          |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_114_ Draft action: read the doi from the pds4 label                                                    |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_116_ Extraction of the OSTI XML in /dois?... GET requests                                              |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_125_ Update DOI UI and Service with new workflow for operational deployment                            |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_134_ Update draft action with new option --lidvid to change from review to draft the status of a DOI   |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_135_ Update API to deactivate 'release' end point, create a 'submit' end-point                         |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_140_ Update submission to OSTI to handle the removal of a field from the OSTI metadata                 |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_144_ enable filter by status in sub-action 'pds-doi-cmd list'                                          |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_148_ API POST /dois should accept DOI OSTI format in payload                                           |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_157_ When a pds4 label or osti can not be parsed generate error 400 in API                             |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_162_ Implement Application Server to wrap Flask service                                                |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_163_ Dockerize API Service                                                                             |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_165_ Add service to API for update of the status of records with OSTI (check sub command)              |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+----------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                           |Priority / Bug Severity   |
+================================================================================================================+==========================+
|NASA-PDS/pds-doi-service_167_ As a user, I want to see the lidvid of my DOIs in the email report                |p.should-have             |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_177_ As an API user I want to filter on lidvids with wildcards                         |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_180_ As an API user I want to filter on PDS3 Data Set IDs with wildcards               |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_183_ As a user of the API, I want to see the DOI's title when I go GET /dois request   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-service_184_ As an API user, I want to always have an update date for the DOIs                 |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+

pds-doi-ui
~~~~~~~~~~
*web UI for pds-doi-service*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-ui/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-doi-ui/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-ui/releases>`_ 


bug
+++

+------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                     |Priority / Bug Severity   |
+==========================================================================================+==========================+
|NASA-PDS/pds-doi-ui_35_ As a SA, I don't want security vulnerabilities in the public UI   |s.medium                  |
+------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                 |Priority / Bug Severity   |
+======================================================================================================+==========================+
|NASA-PDS/pds-doi-ui_1_ Reserve DOI UI forms                                                           |unknown                   |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_9_ Return API error message in UI                                                 |unknown                   |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_10_ Provide a mean to come back to release action when on reserve screen          |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_14_ Prevent the discipline node for doing DOI release without a ENG node review   |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_17_  PDS Label url should take a public URL                                       |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_19_ Release step needs a submitter/node                                           |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_27_ Error need to be catched when one draft a pds4 label from the url             |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_28_ Enable force warning                                                          |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_30_ Display errors and warning when user clicks "save" on the release screen      |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_31_ On release screen, have only one "ignore warning" checkbox                    |p.must-have               |
+------------------------------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                       |Priority / Bug Severity   |
+============================================================================================================================+==========================+
|NASA-PDS/pds-doi-ui_25_ As a user, I want to search for a DOI and associated metadata by LID/LIDVID                         |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-doi-ui_34_ As a user, I want to see the error/warnings messages on the same page from where they were raised   |p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------+--------------------------+

pds-registry-app
~~~~~~~~~~~~~~~~
*Registry application enabling a PDS node to register all its data products for long term preservation and sharing with the rest of the PDS system.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-registry-app>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-registry-app/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-registry-app/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-registry-app/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-registry-app/releases>`_ 


bug
+++

+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                 |Priority / Bug Severity   |
+======================================================================================================================================+==========================+
|NASA-PDS/pds-registry-app_108_ harvest and registry manager in pds-registry-app-0.2.2-bin.zip are missing batch scripts for windows   |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_109_ Test data in pds-registry-app-0.2.2-bin.zip contains invalid PDS4 labels                               |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_110_ Test data in pds-registry-app-0.2.2-bin.zip is missing data products.                                  |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_135_ docker build is version locked                                                                         |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                |Priority / Bug Severity   |
+=====================================================================================================================+==========================+
|NASA-PDS/pds-registry-app_20_ Update Schema Generator for handling special cases where ancestor classes are needed   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_27_ Manage PDS4 product relationships                                                      |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_102_ Add the API to the pds-registry-app package, with documentation                       |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_103_ update registry-manager load-data to handle additional use cases                      |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_113_ Have pds4 properties syntax match the syntax decided for the PDS API                  |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_122_ Initial deployment of API on AWS - ASG/ELB solution                                   |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_123_ Update registry-mgr documentation as stated in #86                                    |p.could-have              |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_129_ Create a registry docker for developer testing                                        |p.could-have              |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_131_ Develop ElasticSearch client library to be utilized by harvest / registry-mgr         |unknown                   |
+---------------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================================================+==========================+
|NASA-PDS/pds-registry-app_57_ The service shall accept artifact registrations.                                                                 |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_58_ The service shall provide a means identifying relationships between artifact registrations                       |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_59_ The service shall maintain configuration regarding the classes of artifacts to be registered                     |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_75_ The service shall accept metadata for a registered artifact in a defined format                                  |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_56_ The service shall assign a global unique identifier to a registered artifact                                     |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_73_ The service shall require a logical identifier and version be provided for all registered artifacts              |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_72_ The service shall store metadata for a registered artifact in an underlying metadata store                       |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_71_ The service shall allow updates to registered artifacts                                                          |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_70_ The service shall allow deletion of registered artifacts                                                         |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_55_ The service shall allow for queries for registered artifacts                                                     |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_68_ The service shall require checksums as metadata for registry artifact to enable system-wide integrity checking   |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_67_ The service shall require a subset of file system metadata in order to support data metrics generation           |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_66_ The service shall require user authorization for updating registry metadata                                      |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_65_ The service shall provide a staging capability for artifacts staged for release                                  |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_141_ As a manager, I want a cost model for deploying a registry + API in AWS                                         |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_142_ As a node operator, I want actionable, user-friendly error messages for registry schema failures                |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_143_ As a node operator, I want to ingest metadata regarding secondary products that belong to a collection.         |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_144_ As a node operator, I want to ingest metadata regarding secondary collections that belong to a bundle.          |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_145_ As a developer, I want to include supplemental file data sizes in the registry                                  |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_146_ As a node operator, I want the the registry schema to update autonomously when new data is ingested.            |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-registry-app_147_ As a node operator,  I want to be able to tag ingested data with the node it is ingested by.                    |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

pds-wds-web
~~~~~~~~~~~
*PDS Web Design System - Basic web implementation*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds-web>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-wds-web>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-wds-web/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-wds-web/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-wds-web/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-wds-web/releases>`_ 


bug
+++

+------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                     |Priority / Bug Severity   |
+==========================================================================================+==========================+
|NASA-PDS/pds-wds-web_9_ App Bar causes usability issues on mobile                         |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-wds-web_10_ PDS App Bar does not work if it's included after the DOM loads   |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-wds-web_15_ App Bar breaks facet selection on Photojournal Beta              |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-wds-web_19_ Update NAIF in App Bar                                           |unknown                   |
+------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+----------------------------------------------------------------+--------------------------+
|Issue                                                           |Priority / Bug Severity   |
+================================================================+==========================+
|NASA-PDS/pds-wds-web_12_ Show screenshot of app-bar in README   |unknown                   |
+----------------------------------------------------------------+--------------------------+
|NASA-PDS/pds-wds-web_17_ App Bar Node List Reordering           |unknown                   |
+----------------------------------------------------------------+--------------------------+

PDS.nasa.gov-Search
~~~~~~~~~~~~~~~~~~~
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
+++++++++++

+----------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                               |Priority / Bug Severity   |
+====================================================================================================+==========================+
|NASA-PDS/PDS.nasa.gov-Search_20_ Search Details Page / DOI Landing Page                             |unknown                   |
+----------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-Search_29_ Iterate with DOI Working Group for improvements to landing pages   |unknown                   |
+----------------------------------------------------------------------------------------------------+--------------------------+

PDS.nasa.gov-UX
~~~~~~~~~~~~~~~
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
+++++++++++

+----------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                           |Priority / Bug Severity   |
+================================================================================================================+==========================+
|NASA-PDS/PDS.nasa.gov-UX_3_ Formulate user stories for prototype                                                |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-UX_5_ Synthesize interview results into user research knowledge base and produce report   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-UX_6_ Model workflows and initial design directions                                       |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-UX_8_ Design mockups and develop Figma prototype                                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-UX_61_ Refine user interview and survey analysis per MC comments                          |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-UX_70_ Refine PDS Web Modernization working group plan                                    |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-UX_71_ Upload all data from airtable / survey to GDrive                                   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/PDS.nasa.gov-UX_73_ Rev 3 of milestones to breakdown of notional goals and deliverables                |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+

pds4-information-model
~~~~~~~~~~~~~~~~~~~~~~
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
+++

+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                         |Priority / Bug Severity   |
+==============================================================================================================================================+==========================+
|NASA-PDS/pds4-information-model_175_ LDDTool: Displaying invalid Imaging Discipline Classes                                                   |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_188_ LDDTool: requires one class with (element_flag = true), even when no classes defined                     |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_266_ Throw WARNING message when enumeration_flag = false but enumerations are specified                       |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_271_ LDDTool forces use of LDD versions based upon config                                                     |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_277_ LDD versionId list in the Data Dictionary Document introduction does not contain valid versionIds        |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_280_ CSV files fail to escape double quotes.                                                                  |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_283_ LDDTool generated LIDs for XML Schema Label Products  do not contain IM or LDD Version Ids               |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_302_ LDDTool does not allow the bundle to be specified for generated dictionaries                             |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_304_ LDDTool does include the PSA namespace                                                                   |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_312_ LDDTool does not generate the complete "All LDD" version of the  WebHelp PDS4 Data Dictionary Document   |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_316_ The 1F00 directory is missing from the Data directory for the 1G00 development release.                  |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_322_ LDDTool generates a 1C00 file when -V 1B00 is specified                                                  |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_327_ Repo tests fail when trying to run back-to-back maven steps                                              |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_328_ LDDTool outputs invalid schema with v13.0.0                                                              |s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_331_ Invalid output schema when trying to set an Internal_Reference reference_type value set                  |s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+----------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                           |Priority / Bug Severity   |
+================================================================================================================+==========================+
|NASA-PDS/pds4-information-model_167_ LDDTool: Use sch:value-of to display a variable in Schematron validation   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_238_ Continuing refactoring of IMTool / LDDTool                                 |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_241_ Improvements from Build 11.0 testing                                       |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_242_ DocBook HTML/WebHelp generation and conversion processes                   |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_293_ Update JSON output to include dependencies in output                       |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_298_ Add title to Rule Assertion to allow generation of regression tests.       |unknown                   |
+----------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-information-model_332_ [namespace-registry] add new namespace "<clementine>"                      |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+--------------------------+

pds4-jparser
~~~~~~~~~~~~
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
+++

+---------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                        |Priority / Bug Severity   |
+=============================================================================================+==========================+
|NASA-PDS/pds4-jparser_21_ Update table reads for large files and improve memory footprints   |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-jparser_32_ NIO Library causes error when trying to build with openJDK 8       |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/pds4-jparser_36_ NoSuchMethodError: java.nio.ByteBuffer with Java9 Builds           |s.medium                  |
+---------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+-----------------------------------------------------------------------+--------------------------+
|Issue                                                                  |Priority / Bug Severity   |
+=======================================================================+==========================+
|NASA-PDS/pds4-jparser_33_ Upgrade pds4-jparser to build with Java11+   |unknown                   |
+-----------------------------------------------------------------------+--------------------------+

PLAID
~~~~~
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
+++++++++++

+------------------------------------------------------------------------------+--------------------------+
|Issue                                                                         |Priority / Bug Severity   |
+==============================================================================+==========================+
|NASA-PDS/PLAID_10_ Develop procedure for how to update PLAID with latest IM   |unknown                   |
+------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+----------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                               |Priority / Bug Severity   |
+====================================================================================================+==========================+
|NASA-PDS/PLAID_15_ As a PDS Operator, I want to update PLAID to the latest PDS4 Information Model   |unknown                   |
+----------------------------------------------------------------------------------------------------+--------------------------+

registry-api-service
~~~~~~~~~~~~~~~~~~~~
*PDS Registry API service. Complies with PDS API specification*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-api-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-api-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-api-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry-api-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-api-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-api-service/releases>`_ 


bug
+++

+------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                 |Priority / Bug Severity   |
+======================================================================================================+==========================+
|NASA-PDS/registry-api-service_16_ API server crashes with OutOfMemoryError if invalid query is used   |s.high                    |
+------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/registry-api-service_17_ error 500 on GET /collections/:lidvid:/products                     |s.high                    |
+------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+-----------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                    |Priority / Bug Severity   |
+=========================================================================================+==========================+
|NASA-PDS/registry-api-service_2_ Manage relationships bundle-collection-product in API   |unknown                   |
+-----------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/registry-api-service_3_ implement the start/limit efficiently                   |unknown                   |
+-----------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/registry-api-service_4_ Implement a lid resolver                                |unknown                   |
+-----------------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+--------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                     |Priority / Bug Severity   |
+==========================================================================================================================+==========================+
|NASA-PDS/registry-api-service_14_ As a node operators, I want to deploy the Registry API Service with the PDS Registry.   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------+--------------------------+

tracking-service
~~~~~~~~~~~~~~~~
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
+++

+---------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                              |Priority / Bug Severity   |
+===================================================================================================+==========================+
|NASA-PDS/tracking-service_18_ tracking front page does not keep tracking in relative anchor href   |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+------------------------------------------------------------------------+--------------------------+
|Issue                                                                   |Priority / Bug Severity   |
+========================================================================+==========================+
|NASA-PDS/tracking-service_10_ Dockerize Tracking Service                |unknown                   |
+------------------------------------------------------------------------+--------------------------+
|NASA-PDS/tracking-service_14_ Add mysql database to docker deployment   |unknown                   |
+------------------------------------------------------------------------+--------------------------+

validate
~~~~~~~~
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
+++

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                              |Priority / Bug Severity   |
+===================================================================================================================================================================+==========================+
|NASA-PDS/validate_5_ Improve file base name check according to Standards Reference                                                                                 |s.low                     |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_6_ Improve pds4.bundle unlabeled files check to handle files without a file suffix                                                               |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_11_ Update allowable field_format values per Standards Reference definition regarding [+-] characters                                            |s.low                     |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_153_ Update validate to throw error when a file has a space in the filename                                                                      |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_189_ Validate error reading tables > 2GiB                                                                                                        |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_240_ Unexpected error for data collection in a sub-directory                                                                                     |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_256_ validate should only do integrity checking on latest version of a collection when referenced by LID                                         |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_257_ Product with incorrect table binary definition pass validation                                                                              |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_260_ Missing documentation about deprecated flags                                                                                                |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_271_ validate 1.25.0-SNAPSHOT raises an exception when validating a product                                                                      |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_273_ Bug performing bundle validation with nested directories                                                                                    |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_278_ Registered context products file does not retain older versions of context products                                                         |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_281_ Validate fails to report error in   File.file_size                                                                                          |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_291_ When validating a product with a bad schematron definition, bundle validation also fails indicating the associated product does not exist   |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_294_ Content validation incorrectly reports error for floating-point values out of specified min/max range                                       |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_297_ Content validation of ASCII_Integer field does not accept value with leading zeroes                                                         |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_298_ validate misses double quotes within a delimited table                                                                                      |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_299_ Validate tool does not PASS a bundle with a single-character filename                                                                       |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_300_ validate -u flag reports an error on Windows                                                                                                |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_301_ unclear error message for field count matching                                                                                              |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_310_ Validate missing collections in bundle after CCB-282 updates                                                                                |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_325_ Validate Incorrectly Throws Error When Embedded Field_Character Contains <CR><LF>                                                           |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_326_ File-size check fails for large data files                                                                                                  |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_327_ validate fails to process large data file                                                                                                   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
+++++++++++

+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                   |Priority / Bug Severity   |
+========================================================================================================================+==========================+
|NASA-PDS/validate_17_ Validate schematron references and throw fatal error if invalid URI specified                     |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_24_ Update context check to retrieve and use latest context products from EN Registry                 |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_51_ Provide the capability to specify multiple locations for pds4.bundle validation                   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_81_ Validate and throw error when duplicate LIDs are found in Bundle                                  |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_230_ Update validate per SR requirements for collection inventories                                   |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_238_ validate does not perform full bundle validation when using a specific bundle.xml                |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_246_ Add output directory flag to validate-bundle tool                                                |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_249_ Improvements for validating accumulating bundles / collections                                   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_252_ Implement initial behavioral testing framework with cucumber                                     |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_254_ validate does not perform expediently when doing bundle-level validation against large bundles   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_264_ Update installation documentation to include 64-bit Java as system requirement                   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_290_ Migrate subset of existing regression tests to cucumber behavioral testing                       |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_322_ Update installation documentation to require Java 1.9+                                           |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_323_ Upgrade to Java 9+                                                                               |unknown                   |
+------------------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
+++++++++++

+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                             |Priority / Bug Severity   |
+==================================================================================================================================================================+==========================+
|NASA-PDS/validate_57_ As a user, I want to be warned when there are alphanumeric characters between fields in Table_Character                                     |p.could-have              |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_149_ As a user, I want validate to check number of records/fields specified in label matches the records in the actual data table               |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_164_ As a user, I want to validate PDF files are PDF/A                                                                                          |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_188_ As a user, I want to validate a bundle that uses multiple versions of the Information Model / Discipline LDDs                              |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_210_ As a user, I want validate to raise a WARNING when differing versions of IM are used within a bundle                                       |p.could-have              |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_292_ CCB-264: Make the Line Feed (LF) character an allowed record delimiter                                                                     |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_303_ As a user, I want to the raise a WARNING if the object-defined size in the label does not match the file_size value                        |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_308_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle   |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

theme
+++++

+--------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                               |Priority / Bug Severity   |
+====================================================================================================================+==========================+
|NASA-PDS/validate_250_ Improvements to meet updated Standards Reference since initial requirements implementation   |unknown                   |
+--------------------------------------------------------------------------------------------------------------------+--------------------------+
|NASA-PDS/validate_318_ B12.0 Content Validation Improvements                                                        |unknown                   |
+--------------------------------------------------------------------------------------------------------------------+--------------------------+

Liens
-----

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
---------------------------------
The Engineering Node Software resources are listed in the `software
release summary (B11.1)`_

Installation and operation
--------------------------
PDS Engineering node software are meant to be deployed in 3 contexts:
standalone, discipline nodes or engineering node
For the installation and operation manual see the `users manuals` in the
software summary sections below:
- `PDS Standalone`_
- `PDS Discipline Nodes`_
- `PDS Engineering Node only`_

Reference documents
-------------------
This section details the controlling and applicable documents referenced
for this release. The controlling documents are as follows:
- PDS Level 1, 2 and 3 Requirements, April 20, 2017.
- PDS4 Project Plan, July 17, 2013.
- PDS4 System Architecture Specification, Version 1.3, September 1,
2013.
- PDS4 Operations Concept, Version 1.0, September 1, 2013.
- PDS Harvest Tool Software Requirements and Design Document (SRD/SDD),
Version 1.2, September 1, 2013.
- PDS Preparation Tools Software Requirements and Design Document
(SRD/SDD), Version 0.3, September 1, 2013.
- PDS Registry Service Software Requirements and Design Document
(SRD/SDD), Version 1.1, September 1, 2013.
- PDS Report Service Software Requirements and Design Document
(SRD/SDD),   Version 1.1, September 1, 2013.
- PDS Search Service Software Requirements and Design Document
(SRD/SDD),   Version 1.0, September 1, 2013.
- PDS Search Scenarios, Version 1.0, September 1, 2013.
- PDS Search Protocol, Version 1.2, March 21, 2014.
- PDAP Search Protocol, Version 1.0, March 21, 2014.
- PDS Security Service Software Requirements and Design Document
(SRD/SDD), Version 1.1, September 1, 2013.
- `PDS Deep Archive Sotware Requirements and Design Document (SRD/SDD)`_
- `PDS DOI Service Requirements and Design Document (SRD/SDD)`_

.. _NASA-PDS/api-search-query-lexer_1: https://github.com/NASA-PDS/api-search-query-lexer/issues/1
.. _NASA-PDS/archive-analytics_2: https://github.com/NASA-PDS/archive-analytics/issues/2
.. _NASA-PDS/archive-analytics_7: https://github.com/NASA-PDS/archive-analytics/issues/7
.. _NASA-PDS/archive-analytics_10: https://github.com/NASA-PDS/archive-analytics/issues/10
.. _NASA-PDS/harvest_6: https://github.com/NASA-PDS/harvest/issues/6
.. _NASA-PDS/harvest_18: https://github.com/NASA-PDS/harvest/issues/18
.. _NASA-PDS/harvest_37: https://github.com/NASA-PDS/harvest/issues/37
.. _NASA-PDS/harvest_45: https://github.com/NASA-PDS/harvest/issues/45
.. _NASA-PDS/mi-label_10: https://github.com/NASA-PDS/mi-label/issues/10
.. _NASA-PDS/pds-api_73: https://github.com/NASA-PDS/pds-api/issues/73
.. _NASA-PDS/pds-api_31: https://github.com/NASA-PDS/pds-api/issues/31
.. _NASA-PDS/pds-api_12: https://github.com/NASA-PDS/pds-api/issues/12
.. _NASA-PDS/pds-api_17: https://github.com/NASA-PDS/pds-api/issues/17
.. _NASA-PDS/pds-api_34: https://github.com/NASA-PDS/pds-api/issues/34
.. _NASA-PDS/pds-api_35: https://github.com/NASA-PDS/pds-api/issues/35
.. _NASA-PDS/pds-api_40: https://github.com/NASA-PDS/pds-api/issues/40
.. _NASA-PDS/pds-api_41: https://github.com/NASA-PDS/pds-api/issues/41
.. _NASA-PDS/pds-api_43: https://github.com/NASA-PDS/pds-api/issues/43
.. _NASA-PDS/pds-api_47: https://github.com/NASA-PDS/pds-api/issues/47
.. _NASA-PDS/pds-api_52: https://github.com/NASA-PDS/pds-api/issues/52
.. _NASA-PDS/pds-api_54: https://github.com/NASA-PDS/pds-api/issues/54
.. _NASA-PDS/pds-api_56: https://github.com/NASA-PDS/pds-api/issues/56
.. _NASA-PDS/pds-api_59: https://github.com/NASA-PDS/pds-api/issues/59
.. _NASA-PDS/pds-api_60: https://github.com/NASA-PDS/pds-api/issues/60
.. _NASA-PDS/pds-api_61: https://github.com/NASA-PDS/pds-api/issues/61
.. _NASA-PDS/pds-api_62: https://github.com/NASA-PDS/pds-api/issues/62
.. _NASA-PDS/pds-api_64: https://github.com/NASA-PDS/pds-api/issues/64
.. _NASA-PDS/pds-api-client_2: https://github.com/NASA-PDS/pds-api-client/issues/2
.. _NASA-PDS/pds-api-javalib_1: https://github.com/NASA-PDS/pds-api-javalib/issues/1
.. _NASA-PDS/pds-api-javalib_2: https://github.com/NASA-PDS/pds-api-javalib/issues/2
.. _NASA-PDS/pds-deep-archive_90: https://github.com/NASA-PDS/pds-deep-archive/issues/90
.. _NASA-PDS/pds-deep-archive_92: https://github.com/NASA-PDS/pds-deep-archive/issues/92
.. _NASA-PDS/pds-deep-archive_99: https://github.com/NASA-PDS/pds-deep-archive/issues/99
.. _NASA-PDS/pds-deep-archive_93: https://github.com/NASA-PDS/pds-deep-archive/issues/93
.. _NASA-PDS/pds-deep-archive_95: https://github.com/NASA-PDS/pds-deep-archive/issues/95
.. _NASA-PDS/pds-deep-archive_7: https://github.com/NASA-PDS/pds-deep-archive/issues/7
.. _NASA-PDS/pds-deep-archive_102: https://github.com/NASA-PDS/pds-deep-archive/issues/102
.. _NASA-PDS/pds-doi-service_119: https://github.com/NASA-PDS/pds-doi-service/issues/119
.. _NASA-PDS/pds-doi-service_121: https://github.com/NASA-PDS/pds-doi-service/issues/121
.. _NASA-PDS/pds-doi-service_122: https://github.com/NASA-PDS/pds-doi-service/issues/122
.. _NASA-PDS/pds-doi-service_126: https://github.com/NASA-PDS/pds-doi-service/issues/126
.. _NASA-PDS/pds-doi-service_128: https://github.com/NASA-PDS/pds-doi-service/issues/128
.. _NASA-PDS/pds-doi-service_138: https://github.com/NASA-PDS/pds-doi-service/issues/138
.. _NASA-PDS/pds-doi-service_141: https://github.com/NASA-PDS/pds-doi-service/issues/141
.. _NASA-PDS/pds-doi-service_143: https://github.com/NASA-PDS/pds-doi-service/issues/143
.. _NASA-PDS/pds-doi-service_150: https://github.com/NASA-PDS/pds-doi-service/issues/150
.. _NASA-PDS/pds-doi-service_154: https://github.com/NASA-PDS/pds-doi-service/issues/154
.. _NASA-PDS/pds-doi-service_159: https://github.com/NASA-PDS/pds-doi-service/issues/159
.. _NASA-PDS/pds-doi-service_52: https://github.com/NASA-PDS/pds-doi-service/issues/52
.. _NASA-PDS/pds-doi-service_91: https://github.com/NASA-PDS/pds-doi-service/issues/91
.. _NASA-PDS/pds-doi-service_114: https://github.com/NASA-PDS/pds-doi-service/issues/114
.. _NASA-PDS/pds-doi-service_116: https://github.com/NASA-PDS/pds-doi-service/issues/116
.. _NASA-PDS/pds-doi-service_125: https://github.com/NASA-PDS/pds-doi-service/issues/125
.. _NASA-PDS/pds-doi-service_134: https://github.com/NASA-PDS/pds-doi-service/issues/134
.. _NASA-PDS/pds-doi-service_135: https://github.com/NASA-PDS/pds-doi-service/issues/135
.. _NASA-PDS/pds-doi-service_140: https://github.com/NASA-PDS/pds-doi-service/issues/140
.. _NASA-PDS/pds-doi-service_144: https://github.com/NASA-PDS/pds-doi-service/issues/144
.. _NASA-PDS/pds-doi-service_148: https://github.com/NASA-PDS/pds-doi-service/issues/148
.. _NASA-PDS/pds-doi-service_157: https://github.com/NASA-PDS/pds-doi-service/issues/157
.. _NASA-PDS/pds-doi-service_162: https://github.com/NASA-PDS/pds-doi-service/issues/162
.. _NASA-PDS/pds-doi-service_163: https://github.com/NASA-PDS/pds-doi-service/issues/163
.. _NASA-PDS/pds-doi-service_165: https://github.com/NASA-PDS/pds-doi-service/issues/165
.. _NASA-PDS/pds-doi-service_167: https://github.com/NASA-PDS/pds-doi-service/issues/167
.. _NASA-PDS/pds-doi-service_177: https://github.com/NASA-PDS/pds-doi-service/issues/177
.. _NASA-PDS/pds-doi-service_180: https://github.com/NASA-PDS/pds-doi-service/issues/180
.. _NASA-PDS/pds-doi-service_183: https://github.com/NASA-PDS/pds-doi-service/issues/183
.. _NASA-PDS/pds-doi-service_184: https://github.com/NASA-PDS/pds-doi-service/issues/184
.. _NASA-PDS/pds-doi-ui_35: https://github.com/NASA-PDS/pds-doi-ui/issues/35
.. _NASA-PDS/pds-doi-ui_1: https://github.com/NASA-PDS/pds-doi-ui/issues/1
.. _NASA-PDS/pds-doi-ui_9: https://github.com/NASA-PDS/pds-doi-ui/issues/9
.. _NASA-PDS/pds-doi-ui_10: https://github.com/NASA-PDS/pds-doi-ui/issues/10
.. _NASA-PDS/pds-doi-ui_14: https://github.com/NASA-PDS/pds-doi-ui/issues/14
.. _NASA-PDS/pds-doi-ui_17: https://github.com/NASA-PDS/pds-doi-ui/issues/17
.. _NASA-PDS/pds-doi-ui_19: https://github.com/NASA-PDS/pds-doi-ui/issues/19
.. _NASA-PDS/pds-doi-ui_27: https://github.com/NASA-PDS/pds-doi-ui/issues/27
.. _NASA-PDS/pds-doi-ui_28: https://github.com/NASA-PDS/pds-doi-ui/issues/28
.. _NASA-PDS/pds-doi-ui_30: https://github.com/NASA-PDS/pds-doi-ui/issues/30
.. _NASA-PDS/pds-doi-ui_31: https://github.com/NASA-PDS/pds-doi-ui/issues/31
.. _NASA-PDS/pds-doi-ui_25: https://github.com/NASA-PDS/pds-doi-ui/issues/25
.. _NASA-PDS/pds-doi-ui_34: https://github.com/NASA-PDS/pds-doi-ui/issues/34
.. _NASA-PDS/pds-registry-app_108: https://github.com/NASA-PDS/pds-registry-app/issues/108
.. _NASA-PDS/pds-registry-app_109: https://github.com/NASA-PDS/pds-registry-app/issues/109
.. _NASA-PDS/pds-registry-app_110: https://github.com/NASA-PDS/pds-registry-app/issues/110
.. _NASA-PDS/pds-registry-app_135: https://github.com/NASA-PDS/pds-registry-app/issues/135
.. _NASA-PDS/pds-registry-app_20: https://github.com/NASA-PDS/pds-registry-app/issues/20
.. _NASA-PDS/pds-registry-app_27: https://github.com/NASA-PDS/pds-registry-app/issues/27
.. _NASA-PDS/pds-registry-app_102: https://github.com/NASA-PDS/pds-registry-app/issues/102
.. _NASA-PDS/pds-registry-app_103: https://github.com/NASA-PDS/pds-registry-app/issues/103
.. _NASA-PDS/pds-registry-app_113: https://github.com/NASA-PDS/pds-registry-app/issues/113
.. _NASA-PDS/pds-registry-app_122: https://github.com/NASA-PDS/pds-registry-app/issues/122
.. _NASA-PDS/pds-registry-app_123: https://github.com/NASA-PDS/pds-registry-app/issues/123
.. _NASA-PDS/pds-registry-app_129: https://github.com/NASA-PDS/pds-registry-app/issues/129
.. _NASA-PDS/pds-registry-app_131: https://github.com/NASA-PDS/pds-registry-app/issues/131
.. _NASA-PDS/pds-registry-app_57: https://github.com/NASA-PDS/pds-registry-app/issues/57
.. _NASA-PDS/pds-registry-app_58: https://github.com/NASA-PDS/pds-registry-app/issues/58
.. _NASA-PDS/pds-registry-app_59: https://github.com/NASA-PDS/pds-registry-app/issues/59
.. _NASA-PDS/pds-registry-app_75: https://github.com/NASA-PDS/pds-registry-app/issues/75
.. _NASA-PDS/pds-registry-app_56: https://github.com/NASA-PDS/pds-registry-app/issues/56
.. _NASA-PDS/pds-registry-app_73: https://github.com/NASA-PDS/pds-registry-app/issues/73
.. _NASA-PDS/pds-registry-app_72: https://github.com/NASA-PDS/pds-registry-app/issues/72
.. _NASA-PDS/pds-registry-app_71: https://github.com/NASA-PDS/pds-registry-app/issues/71
.. _NASA-PDS/pds-registry-app_70: https://github.com/NASA-PDS/pds-registry-app/issues/70
.. _NASA-PDS/pds-registry-app_55: https://github.com/NASA-PDS/pds-registry-app/issues/55
.. _NASA-PDS/pds-registry-app_68: https://github.com/NASA-PDS/pds-registry-app/issues/68
.. _NASA-PDS/pds-registry-app_67: https://github.com/NASA-PDS/pds-registry-app/issues/67
.. _NASA-PDS/pds-registry-app_66: https://github.com/NASA-PDS/pds-registry-app/issues/66
.. _NASA-PDS/pds-registry-app_65: https://github.com/NASA-PDS/pds-registry-app/issues/65
.. _NASA-PDS/pds-registry-app_141: https://github.com/NASA-PDS/pds-registry-app/issues/141
.. _NASA-PDS/pds-registry-app_142: https://github.com/NASA-PDS/pds-registry-app/issues/142
.. _NASA-PDS/pds-registry-app_143: https://github.com/NASA-PDS/pds-registry-app/issues/143
.. _NASA-PDS/pds-registry-app_144: https://github.com/NASA-PDS/pds-registry-app/issues/144
.. _NASA-PDS/pds-registry-app_145: https://github.com/NASA-PDS/pds-registry-app/issues/145
.. _NASA-PDS/pds-registry-app_146: https://github.com/NASA-PDS/pds-registry-app/issues/146
.. _NASA-PDS/pds-registry-app_147: https://github.com/NASA-PDS/pds-registry-app/issues/147
.. _NASA-PDS/pds-wds-web_9: https://github.com/NASA-PDS/pds-wds-web/issues/9
.. _NASA-PDS/pds-wds-web_10: https://github.com/NASA-PDS/pds-wds-web/issues/10
.. _NASA-PDS/pds-wds-web_15: https://github.com/NASA-PDS/pds-wds-web/issues/15
.. _NASA-PDS/pds-wds-web_19: https://github.com/NASA-PDS/pds-wds-web/issues/19
.. _NASA-PDS/pds-wds-web_12: https://github.com/NASA-PDS/pds-wds-web/issues/12
.. _NASA-PDS/pds-wds-web_17: https://github.com/NASA-PDS/pds-wds-web/issues/17
.. _NASA-PDS/PDS.nasa.gov-Search_20: https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/20
.. _NASA-PDS/PDS.nasa.gov-Search_29: https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/29
.. _NASA-PDS/PDS.nasa.gov-UX_3: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/3
.. _NASA-PDS/PDS.nasa.gov-UX_5: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/5
.. _NASA-PDS/PDS.nasa.gov-UX_6: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/6
.. _NASA-PDS/PDS.nasa.gov-UX_8: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/8
.. _NASA-PDS/PDS.nasa.gov-UX_61: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/61
.. _NASA-PDS/PDS.nasa.gov-UX_70: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/70
.. _NASA-PDS/PDS.nasa.gov-UX_71: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/71
.. _NASA-PDS/PDS.nasa.gov-UX_73: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/73
.. _NASA-PDS/pds4-information-model_175: https://github.com/NASA-PDS/pds4-information-model/issues/175
.. _NASA-PDS/pds4-information-model_188: https://github.com/NASA-PDS/pds4-information-model/issues/188
.. _NASA-PDS/pds4-information-model_266: https://github.com/NASA-PDS/pds4-information-model/issues/266
.. _NASA-PDS/pds4-information-model_271: https://github.com/NASA-PDS/pds4-information-model/issues/271
.. _NASA-PDS/pds4-information-model_277: https://github.com/NASA-PDS/pds4-information-model/issues/277
.. _NASA-PDS/pds4-information-model_280: https://github.com/NASA-PDS/pds4-information-model/issues/280
.. _NASA-PDS/pds4-information-model_283: https://github.com/NASA-PDS/pds4-information-model/issues/283
.. _NASA-PDS/pds4-information-model_302: https://github.com/NASA-PDS/pds4-information-model/issues/302
.. _NASA-PDS/pds4-information-model_304: https://github.com/NASA-PDS/pds4-information-model/issues/304
.. _NASA-PDS/pds4-information-model_312: https://github.com/NASA-PDS/pds4-information-model/issues/312
.. _NASA-PDS/pds4-information-model_316: https://github.com/NASA-PDS/pds4-information-model/issues/316
.. _NASA-PDS/pds4-information-model_322: https://github.com/NASA-PDS/pds4-information-model/issues/322
.. _NASA-PDS/pds4-information-model_327: https://github.com/NASA-PDS/pds4-information-model/issues/327
.. _NASA-PDS/pds4-information-model_328: https://github.com/NASA-PDS/pds4-information-model/issues/328
.. _NASA-PDS/pds4-information-model_331: https://github.com/NASA-PDS/pds4-information-model/issues/331
.. _NASA-PDS/pds4-information-model_167: https://github.com/NASA-PDS/pds4-information-model/issues/167
.. _NASA-PDS/pds4-information-model_238: https://github.com/NASA-PDS/pds4-information-model/issues/238
.. _NASA-PDS/pds4-information-model_241: https://github.com/NASA-PDS/pds4-information-model/issues/241
.. _NASA-PDS/pds4-information-model_242: https://github.com/NASA-PDS/pds4-information-model/issues/242
.. _NASA-PDS/pds4-information-model_293: https://github.com/NASA-PDS/pds4-information-model/issues/293
.. _NASA-PDS/pds4-information-model_298: https://github.com/NASA-PDS/pds4-information-model/issues/298
.. _NASA-PDS/pds4-information-model_332: https://github.com/NASA-PDS/pds4-information-model/issues/332
.. _NASA-PDS/pds4-jparser_21: https://github.com/NASA-PDS/pds4-jparser/issues/21
.. _NASA-PDS/pds4-jparser_32: https://github.com/NASA-PDS/pds4-jparser/issues/32
.. _NASA-PDS/pds4-jparser_36: https://github.com/NASA-PDS/pds4-jparser/issues/36
.. _NASA-PDS/pds4-jparser_33: https://github.com/NASA-PDS/pds4-jparser/issues/33
.. _NASA-PDS/PLAID_10: https://github.com/NASA-PDS/PLAID/issues/10
.. _NASA-PDS/PLAID_15: https://github.com/NASA-PDS/PLAID/issues/15
.. _NASA-PDS/registry-api-service_16: https://github.com/NASA-PDS/registry-api-service/issues/16
.. _NASA-PDS/registry-api-service_17: https://github.com/NASA-PDS/registry-api-service/issues/17
.. _NASA-PDS/registry-api-service_2: https://github.com/NASA-PDS/registry-api-service/issues/2
.. _NASA-PDS/registry-api-service_3: https://github.com/NASA-PDS/registry-api-service/issues/3
.. _NASA-PDS/registry-api-service_4: https://github.com/NASA-PDS/registry-api-service/issues/4
.. _NASA-PDS/registry-api-service_14: https://github.com/NASA-PDS/registry-api-service/issues/14
.. _NASA-PDS/tracking-service_18: https://github.com/NASA-PDS/tracking-service/issues/18
.. _NASA-PDS/tracking-service_10: https://github.com/NASA-PDS/tracking-service/issues/10
.. _NASA-PDS/tracking-service_14: https://github.com/NASA-PDS/tracking-service/issues/14
.. _NASA-PDS/validate_5: https://github.com/NASA-PDS/validate/issues/5
.. _NASA-PDS/validate_6: https://github.com/NASA-PDS/validate/issues/6
.. _NASA-PDS/validate_11: https://github.com/NASA-PDS/validate/issues/11
.. _NASA-PDS/validate_153: https://github.com/NASA-PDS/validate/issues/153
.. _NASA-PDS/validate_189: https://github.com/NASA-PDS/validate/issues/189
.. _NASA-PDS/validate_240: https://github.com/NASA-PDS/validate/issues/240
.. _NASA-PDS/validate_256: https://github.com/NASA-PDS/validate/issues/256
.. _NASA-PDS/validate_257: https://github.com/NASA-PDS/validate/issues/257
.. _NASA-PDS/validate_260: https://github.com/NASA-PDS/validate/issues/260
.. _NASA-PDS/validate_271: https://github.com/NASA-PDS/validate/issues/271
.. _NASA-PDS/validate_273: https://github.com/NASA-PDS/validate/issues/273
.. _NASA-PDS/validate_278: https://github.com/NASA-PDS/validate/issues/278
.. _NASA-PDS/validate_281: https://github.com/NASA-PDS/validate/issues/281
.. _NASA-PDS/validate_291: https://github.com/NASA-PDS/validate/issues/291
.. _NASA-PDS/validate_294: https://github.com/NASA-PDS/validate/issues/294
.. _NASA-PDS/validate_297: https://github.com/NASA-PDS/validate/issues/297
.. _NASA-PDS/validate_298: https://github.com/NASA-PDS/validate/issues/298
.. _NASA-PDS/validate_299: https://github.com/NASA-PDS/validate/issues/299
.. _NASA-PDS/validate_300: https://github.com/NASA-PDS/validate/issues/300
.. _NASA-PDS/validate_301: https://github.com/NASA-PDS/validate/issues/301
.. _NASA-PDS/validate_310: https://github.com/NASA-PDS/validate/issues/310
.. _NASA-PDS/validate_325: https://github.com/NASA-PDS/validate/issues/325
.. _NASA-PDS/validate_326: https://github.com/NASA-PDS/validate/issues/326
.. _NASA-PDS/validate_327: https://github.com/NASA-PDS/validate/issues/327
.. _NASA-PDS/validate_17: https://github.com/NASA-PDS/validate/issues/17
.. _NASA-PDS/validate_24: https://github.com/NASA-PDS/validate/issues/24
.. _NASA-PDS/validate_51: https://github.com/NASA-PDS/validate/issues/51
.. _NASA-PDS/validate_81: https://github.com/NASA-PDS/validate/issues/81
.. _NASA-PDS/validate_230: https://github.com/NASA-PDS/validate/issues/230
.. _NASA-PDS/validate_238: https://github.com/NASA-PDS/validate/issues/238
.. _NASA-PDS/validate_246: https://github.com/NASA-PDS/validate/issues/246
.. _NASA-PDS/validate_249: https://github.com/NASA-PDS/validate/issues/249
.. _NASA-PDS/validate_252: https://github.com/NASA-PDS/validate/issues/252
.. _NASA-PDS/validate_254: https://github.com/NASA-PDS/validate/issues/254
.. _NASA-PDS/validate_264: https://github.com/NASA-PDS/validate/issues/264
.. _NASA-PDS/validate_290: https://github.com/NASA-PDS/validate/issues/290
.. _NASA-PDS/validate_322: https://github.com/NASA-PDS/validate/issues/322
.. _NASA-PDS/validate_323: https://github.com/NASA-PDS/validate/issues/323
.. _NASA-PDS/validate_57: https://github.com/NASA-PDS/validate/issues/57
.. _NASA-PDS/validate_149: https://github.com/NASA-PDS/validate/issues/149
.. _NASA-PDS/validate_164: https://github.com/NASA-PDS/validate/issues/164
.. _NASA-PDS/validate_188: https://github.com/NASA-PDS/validate/issues/188
.. _NASA-PDS/validate_210: https://github.com/NASA-PDS/validate/issues/210
.. _NASA-PDS/validate_292: https://github.com/NASA-PDS/validate/issues/292
.. _NASA-PDS/validate_303: https://github.com/NASA-PDS/validate/issues/303
.. _NASA-PDS/validate_308: https://github.com/NASA-PDS/validate/issues/308
.. _NASA-PDS/validate_250: https://github.com/NASA-PDS/validate/issues/250
.. _NASA-PDS/validate_318: https://github.com/NASA-PDS/validate/issues/318
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
