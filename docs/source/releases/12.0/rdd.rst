===========================================================
Release Description Document (build 11.1), software changes
===========================================================
This release of the PDS4 System is intended as an operational release of
the system components to date.
The original plan for this release can be found here: `plan B12.0`_

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
|`pds4-information-model#164`_   |CCB-283: Add reference_type value document_to_data                                                             |
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
|`pds4-information-model#403`_   |CCB-329 - Broaden Definition of Attribute aperture                                                             |
+--------------------------------+---------------------------------------------------------------------------------------------------------------+

Software changes
================
archive-analytics
-----------------
*Processes, tools, and configuration for managing PDS archive analytics software and reports*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/archive-analytics#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/archive-analytics>`_
     - `Issue Tracking <https://github.com/NASA-PDS/archive-analytics/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/archive-analytics/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/archive-analytics/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/archive-analytics/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                  |Priority / Bug Severity   |
+=======================================================================================================================+==========================+
|`archive-analytics#2`_ As a manager, I want to know the current total volume of PDS holdings                           |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`archive-analytics#7`_ As a PDS Project Office, I want to know the historical total volume of PDS holdings over time   |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------+--------------------------+
|Issue                                                                    |Priority / Bug Severity   |
+=========================================================================+==========================+
|`archive-analytics#16`_ Develop procedure and export of Kibana config    |unknown                   |
+-------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-----------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                    |Priority / Bug Severity   |
+=========================================================================================+==========================+
|`harvest#60`_ As a user, I want to ingest the PDS4 label as JSON in a binary blob form   |p.should-have             |
+-----------------------------------------------------------------------------------------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------+--------------------------+
|Issue                                                                             |Priority / Bug Severity   |
+==================================================================================+==========================+
|`harvest#55`_ Quick fix to support date/time conversion to "ISO instant" format   |p.must-have               |
+----------------------------------------------------------------------------------+--------------------------+
|`harvest#58`_ Enable blob ingestion by default                                    |unknown                   |
+----------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
- `pds-api#24`_ [registry] Handle PDS Supplemental Metadata

+-----------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                      |Level         |Priority / Bug Severity   |
+===========================================================================================================+==============+==========================+
|`pds-api#67`_ As an API user, I want to access supplemental metadata from Product_Metadata_Supplemental.   |requirement   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------+--------------+--------------------------+


- `pds-api#76`_ [pds-api] Improve API Performance

+---------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                      |Level         |Priority / Bug Severity   |
+===========================================================================+==============+==========================+
|`pds-api#80`_ As a developer, I never want the label blob to be returned   |requirement   |p.must-have               |
+---------------------------------------------------------------------------+--------------+--------------------------+


- `pds-api#75`_ [pds-api] B12.0 API Response Improvements

+-------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                                                      |Level         |Priority / Bug Severity   |
+===========================================================================================================================================+==============+==========================+
|`pds-api#91`_ Disable XML and HTML responses from current registry-api-service implementation                                              |enhancement   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-api#101`_ As a user, I want to receive a JSON response that contains the PDS4 label metadata in JSON format (application/pds4+json)   |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-api#105`_ As an API user, I want to know how long a request took to complete                                                          |requirement   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+


- `pds-api#77`_ [pds-api] PDS4 Product Relationships

+---------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                          |Level         |Priority / Bug Severity   |
+===============================================================================================================+==============+==========================+
|`pds-api#56`_ As an API user, I want to know the children and ancestors of bundle, collections, and products   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-api#59`_ As an API user, I want to know the Product(s) that belong to a given Bundle.                     |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-api#60`_ As an API user, I want to know the Bundle for a given Product.                                   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-api#61`_ As an API user, I want to know the Collection(s) for a given Product.                            |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-api#62`_ As an API user, I want to know the Bundle for a given Collection.                                |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+--------------+--------------------------+


- `pds-api#81`_ [pds-api] B12.0 Improve API query handling

+--------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                   |Level         |Priority / Bug Severity   |
+========================================================================================================+==============+==========================+
|`pds-api#74`_ As an API user, I want to specify whether I get the latest or all versions of a product   |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-api#83`_ As an API user, I want to search using URL parameters                                     |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------+--------------+--------------------------+


- `pds-api#84`_ [pds-api] Initial Google-like Search

+--------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                 |Level         |Priority / Bug Severity   |
+======================================================================================+==============+==========================+
|`pds-api#99`_ As an API user, I want to be able to use the API for free text search   |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------+--------------+--------------------------+


Other updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                          |Priority / Bug Severity   |
+===============================================================================================+==========================+
|`pds-api#73`_ As a n00b paginator, there might be an off-by-1 error in the `limit` parameter   |s.medium                  |
+-----------------------------------------------------------------------------------------------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                         |Priority / Bug Severity   |
+==============================================================================================+==========================+
|`pds-api#96`_ As an API user, I want to get the latest version of a product, by default       |p.must-have               |
+----------------------------------------------------------------------------------------------+--------------------------+
|`pds-api#107`_ As an API user, I want to explicitly request the latest version of a product   |p.could-have              |
+----------------------------------------------------------------------------------------------+--------------------------+

pds-api-client
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
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------+--------------------------+
|Issue                                                                        |Priority / Bug Severity   |
+=============================================================================+==========================+
|`pds-api-client#6`_ Stack trace when calling `BundlesApi.bundle_by_lidvid`   |s.medium                  |
+-----------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
- `pds-deep-archive#105`_ Integrate PDS Deep Archive with Registry

+---------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                  |Level         |Priority / Bug Severity   |
+=======================================================================================+==============+==========================+
|`pds-deep-archive#7`_ As a user, I want to generate AIPs and SIPs using Registry       |requirement   |unknown                   |
+---------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-deep-archive#106`_ Improvements per API updates to remove workarounds from code   |enhancement   |p.must-have               |
+---------------------------------------------------------------------------------------+--------------+--------------------------+


Other updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                     |Priority / Bug Severity   |
+==========================================================================================================+==========================+
|`pds-deep-archive#116`_ deep archive misses products that specify primary products using lower case 'p'   |s.low                     |
+----------------------------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
- `pds-doi-service#86`_ Deploy DOI API and UI

+-------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                            |Level         |Priority / Bug Severity   |
+=================================================================================================+==============+==========================+
|`pds-doi-service#90`_ Deploy point build of DOI service and UI                                   |task          |unknown                   |
+-------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-doi-service#145`_ review the full doi workflow and make it smooth for eng operators/users   |enhancement   |unknown                   |
+-------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-doi-service#187`_ As a SA, I want the operational deployment of the service to be secure    |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------+--------------+--------------------------+


- `pds-doi-service#178`_ B12.0 Refinements to DOI Service and UI for
Initial Release

+--------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                   |Level         |Priority / Bug Severity   |
+========================================================================================================+==============+==========================+
|`pds-doi-service#163`_ Dockerize API Service                                                            |enhancement   |unknown                   |
+--------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-doi-service#180`_ As an API user I want to filter on PDS3 Data Set IDs with wildcards              |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-doi-service#188`_ As a user, I want to make sure I can not override existing DOI with new LIDVID   |bug           |s.medium                  |
+--------------------------------------------------------------------------------------------------------+--------------+--------------------------+


Other updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------+--------------------------+
|Issue                                                                         |Priority / Bug Severity   |
+==============================================================================+==========================+
|`pds-doi-service#191`_ API accepts Reserve submissions with invalid LIDVIDs   |s.medium                  |
+------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#220`_ CI does not work on main branch for dev release        |unknown                   |
+------------------------------------------------------------------------------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                 |Priority / Bug Severity   |
+======================================================================================================================+==========================+
|`pds-doi-service#171`_ As an operator, I want to reserve a DOI through DataCite                                       |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#172`_ As an operator, I want query for one or more minted DOIs from DataCite                         |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#174`_ As an operator, I want to release a DOI through DataCite                                       |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#175`_ As an operator, I want to update DOI metadata through DataCite                                 |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#198`_ As a user, I want to use the API with ids containing a slash (/)                               |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#228`_ As an admistrator of the application,  I want to restrict access to API by specific referrer   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                         |Priority / Bug Severity   |
+==============================================================================================================+==========================+
|`pds-doi-service#162`_ Implement Application Server to wrap Flask service                                     |p.should-have             |
+--------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#165`_ Add service to API for update of the status of records with OSTI (check sub command)   |unknown                   |
+--------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#227`_ Update DOI service for handling existing DOIs acceptance criteria per #175             |unknown                   |
+--------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-service#229`_ As a user, I want to see the PDS3 ids as they originally are                           |unknown                   |
+--------------------------------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------+--------------------------+
|Issue                                                                              |Priority / Bug Severity   |
+===================================================================================+==========================+
|`pds-doi-ui#22`_ After reserve one file successfully, resubmit a new file          |s.low                     |
+-----------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#35`_ As a SA, I don't want security vulnerabilities in the public UI   |s.medium                  |
+-----------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#70`_ navigation issue when using the app bar                           |s.high                    |
+-----------------------------------------------------------------------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                        |Priority / Bug Severity   |
+=============================================================================================================================+==========================+
|`pds-doi-ui#25`_ As a user, I want to search for a DOI and associated metadata by LID/LIDVID                                 |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#34`_ As a user, I want to see the error/warnings messages on the same page from where they were raised           |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#41`_ As a user, I want to acquire a DOI for a PDS4 product prior to it's public release of the data              |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#42`_ As a user, I want to acquire a DOI for a PDS4 product that has been registered and is publicly accessible   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#65`_ As a user, I want my search criteria to persist in the URL                                                  |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#71`_ As a user, I want to have a dedicated favicon for the service                                               |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                              |Priority / Bug Severity   |
+===================================================================================================+==========================+
|`pds-doi-ui#1`_ Reserve DOI UI forms                                                               |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#9`_ Return API error message in UI                                                     |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#10`_ Provide a mean to come back to release action when on reserve screen              |p.must-have               |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#48`_ Enhancements per initial implementation of mockups                                |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#49`_ Add Feedback Widget to DOI UI                                                     |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#50`_ Add additional help information throughout DOI UI                                 |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#54`_ Update Release and Update DOI pages to follow similar design as Create DOI page   |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#75`_ Add link to landing page from `Identifier` column in search results               |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#79`_ Create javascript library for website integration                                 |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+
|`pds-doi-ui#82`_ Create PDS React Component Library Process For NPM Packages                       |unknown                   |
+---------------------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
- `pds-registry-app#155`_ [registry] Registry Regression Test and
Documentation

+-----------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                      |Level         |Priority / Bug Severity   |
+===========================================================================================================+==============+==========================+
|`pds-registry-app#153`_ As a developer, I want to extend the registry-mgr and harvest using the Java API   |requirement   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds-registry-app#154`_ As a manager, I want the registry to have regression tests included in CI          |requirement   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------+--------------+--------------------------+


Other updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------+--------------------------+
|Issue                                                                      |Priority / Bug Severity   |
+===========================================================================+==========================+
|`pds-registry-app#163`_ docker instructions in README.md are not working   |s.medium                  |
+---------------------------------------------------------------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                              |Priority / Bug Severity   |
+===================================================================================================================================+==========================+
|`pds-registry-app#12`_ As a registry user, I want to ingest supplemental metadata from Product_Metadata_Supplemental.              |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#130`_ As a node operator, I want to harvest and ingest a subset of a bundle based on existing registered data.   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#147`_ As a node operator,  I want to be able to tag ingested data with the node it is ingested by.               |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                               |Priority / Bug Severity   |
+====================================================================================+==========================+
|`pds-registry-app#122`_ Initial deployment of API on AWS - ASG/ELB solution         |unknown                   |
+------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#150`_ Develop plan for instituting AWS ES Cross Cluster Search    |p.must-have               |
+------------------------------------------------------------------------------------+--------------------------+
|`pds-registry-app#165`_ Initial deployment of API on AWS - Fargate solution         |unknown                   |
+------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-----------------------------------------------------+--------------------------+
|Issue                                                |Priority / Bug Severity   |
+=====================================================+==========================+
|`pds-wds-web#25`_ Review and merge App Bar Updates   |unknown                   |
+-----------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                               |Priority / Bug Severity   |
+====================================================================================================================+==========================+
|`PDS.nasa.gov-Search#33`_ Initial investigation for Search UI utilizing PDS API and identify new API user stories   |unknown                   |
+--------------------------------------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
- `PDS.nasa.gov-UX#74`_ Plan and Kick-off PDS WMWG

+--------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                       |Level         |Priority / Bug Severity   |
+============================================================================================+==============+==========================+
|`PDS.nasa.gov-UX#73`_ Rev 3 of milestones to breakdown of notional goals and deliverables   |enhancement   |p.must-have               |
+--------------------------------------------------------------------------------------------+--------------+--------------------------+


Other updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                        |Priority / Bug Severity   |
+=============================================================================================================+==========================+
|`PDS.nasa.gov-UX#81`_ [Training] incorporate new materials - misc videos and ancillary files for TBD video   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------------+
|`PDS.nasa.gov-UX#86`_ [Training] incorporate changes from June pow-wow                                       |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
- `pds4-information-model#349`_ Establish LDD Management Teams and
Processes

+--------------------------------------------------------------+--------+--------------------------+
|Issue                                                         |Level   |Priority / Bug Severity   |
+==============================================================+========+==========================+
|`pds4-information-model#347`_ Create dLDD CCB                 |task    |unknown                   |
+--------------------------------------------------------------+--------+--------------------------+
|`pds4-information-model#348`_ Create dLDD Stewardship Teams   |task    |unknown                   |
+--------------------------------------------------------------+--------+--------------------------+


- `pds4-information-model#326`_ B12.0 LDDTool Improvements

+--------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                         |Level         |Priority / Bug Severity   |
+==============================================================================================================+==============+==========================+
|`pds4-information-model#240`_ Improve argument handling using argument parsing library                        |task          |p.must-have               |
+--------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds4-information-model#330`_ As a user I want to know the output of the tool after it completes execution.   |requirement   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds4-information-model#338`_ As a developer, I want to know the dLDD version from the output JSON data       |requirement   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds4-information-model#346`_ lddtool's doc directory is not in tgz file                                      |bug           |s.low                     |
+--------------------------------------------------------------------------------------------------------------+--------------+--------------------------+


- `pds4-information-model#356`_ Kick-off PDS4 Information Model in
GraphDB

+-----------------------------------------------------------------------------------------+--------+--------------------------+
|Issue                                                                                    |Level   |Priority / Bug Severity   |
+=========================================================================================+========+==========================+
|`pds4-information-model#357`_ Ingest PDS4 IM into BlazeGraph                             |task    |unknown                   |
+-----------------------------------------------------------------------------------------+--------+--------------------------+
|`pds4-information-model#358`_ Replicate diagram from PDS4 IM Spec                        |task    |unknown                   |
+-----------------------------------------------------------------------------------------+--------+--------------------------+
|`pds4-information-model#359`_ Deploy new Amazon Neptune instance for PDS4 IM prototype   |task    |unknown                   |
+-----------------------------------------------------------------------------------------+--------+--------------------------+


- `pds4-information-model#368`_ B12.0 Evolution of
DD_Associate_External_Class

+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                                                                   |Level         |Priority / Bug Severity   |
+========================================================================================================================================================+==============+==========================+
|`pds4-information-model#324`_ An LDD developer desires to inherit a class/attribute defined using DD_Associate_External_Class                           |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds4-information-model#369`_ Evolution of CCB-256: Need method for providing permissible value definitions for external namespaces in Ingest_LDD.      |enhancement   |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds4-information-model#391`_ Issue with DD_Associate_External_Class when trying to reference pds:Internal_Reference and pds:Local_Internal_Reference   |bug           |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`pds4-information-model#397`_ Different formatting of JSON output between 1F00 and 1G00 generation                                                      |bug           |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+


Other updates
~~~~~~~~~~~~~
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


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------+--------------------------+
|Issue                                                       |Priority / Bug Severity   |
+============================================================+==========================+
|`pds4-jparser#40`_ SNAPSHOT dependencies in 2.0.0 release   |s.low                     |
+------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                     |Priority / Bug Severity   |
+==========================================================================================+==========================+
|`PLAID#21`_ Discipline LDD workflow page is missing new discipline LDDs added to config   |s.medium                  |
+------------------------------------------------------------------------------------------+--------------------------+
|`PLAID#25`_ All products are assumed to be Product_Observational by PLAID                 |s.high                    |
+------------------------------------------------------------------------------------------+--------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                        |Priority / Bug Severity   |
+=============================================================================================+==========================+
|`PLAID#15`_ As a PDS Operator, I want to update PLAID to the latest PDS4 Information Model   |unknown                   |
+---------------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
No planned update realised in the build in this repository.

Other updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                              |Priority / Bug Severity   |
+===================================================================================================================================+==========================+
|`registry-api-service#16`_ API server crashes with OutOfMemoryError if invalid query is used                                       |s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#17`_ error 500 on GET /collections/:lidvid:/products                                                         |s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#27`_ XML and PDS4+XML Response Formats are invalid                                                           |s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#43`_ As an API caller, I expect MD5s and file reference URLs to have real values and not the string "null"   |s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#51`_ blob is returned in product results if fields to return are not specified                               |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                   |Priority / Bug Severity   |
+========================================================================================================================================+==========================+
|`registry-api-service#10`_ As a SA, I want to deploy the API behind a proxy                                                             |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#13`_ As a developer, I want to utilize ElasticSearch performance robustness for API response time requirements.   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#14`_ As a node operators, I want to deploy the Registry API Service with the PDS Registry.                        |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`registry-api-service#47`_ As a user, I want to have a complete default fields (for now at least)                                       |unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

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


Planned Updates
~~~~~~~~~~~~~~~
- `validate#317`_ B12.0 Referential Integrity Improvements

+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                                                                                     |Level         |Priority / Bug Severity   |
+==========================================================================================================================================================================+==============+==========================+
|`validate#69`_ As a user, I want to validate that all context objects specified in observational products are referenced in the parent bundle/collection Reference_List   |requirement   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`validate#308`_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle                  |requirement   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`validate#358`_ Improve validate performance by removing unnecessary file IO                                                                                              |enhancement   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`validate#368`_ Product referential integrity check throws invalid WARNINGs                                                                                               |bug           |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`validate#372`_ Issues with logic for reading latest version of collections, and file read logging lost with v2.* of validate                                             |bug           |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+


- `validate#318`_ B12.0 Content Validation Improvements

+--------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|Issue                                                                                                                                 |Level         |Priority / Bug Severity   |
+======================================================================================================================================+==============+==========================+
|`validate#57`_ As a user, I want to be warned when there are alphanumeric characters between fields in Table_Character                |requirement   |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`validate#164`_ As a user, I want to validate PDF files are PDF/A                                                                     |requirement   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`validate#303`_ As a user, I want to the raise a WARNING if the object-defined size in the label does not match the file_size value   |requirement   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+
|`validate#314`_ Revert #9: Do not throw ERROR message when ASCII Numeric field consists of only white space                           |bug           |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------+--------------------------+


Other updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                             |Priority / Bug Severity   |
+==================================================================================================================================================================+==========================+
|`validate#310`_ Validate missing collections in bundle after CCB-282 updates                                                                                      |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#325`_ Validate Incorrectly Throws Error When Embedded Field_Character Contains <CR><LF>                                                                 |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#326`_ File-size check fails for large data files                                                                                                        |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#327`_ validate fails to process large data file                                                                                                         |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#357`_ Validate allows CRLF within a Table_Delimited field                                                                                               |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#360`_ validate does not parse colon in Windows path                                                                                                     |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#361`_ validate does not check Header of a File_Area_Ancillary nor does not provide a meaningful error message for an incorrect Table_Character offset   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#364`_ validate does not allow ".XML" as an extension for a label file                                                                                   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#366`_ validate should not check if file is PDF/A if --skip-content-validation is enabled                                                                |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#375`_ validate halts if label has name "collection" embedded                                                                                            |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#379`_ FileService:printStackTraceToFile:ERROR when validating a product with overlapping fields                                                         |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#380`_ stack trace being created during successful validate execution                                                                                    |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#381`_ validate does not work correctly when the path name contains a space                                                                              |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#392`_ Validate throws incorrect overlap error when first Field_Bit has length 1                                                                         |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                |Priority / Bug Severity   |
+=====================================================================================+==========================+
|`validate#373`_ Update pds4 version mismatch warning message and problem type        |unknown                   |
+-------------------------------------------------------------------------------------+--------------------------+
|`validate#374`_ Refactor PDF/A check handling to match with similar product checks   |unknown                   |
+-------------------------------------------------------------------------------------+--------------------------+

Liens
=====

+---------------------------------------------------------------------+---------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Issue                                                                |Title                                                    |Rationale                                                                                                                                                                                                                                                                                                           |
+=====================================================================+=========================================================+====================================================================================================================================================================================================================================================================================================================+
|pds-swg_11_ [CR] B12.0 Add Information Model Tasks to Release Plan   |[CR] B12.0 Add Information Model Tasks to Release Plan   |The GEOM LDD split effort is fully underway and we have pretty much dug the hole too deep at this point. Pulling back on that effort is most likely a non-starter, so we have to pivot to support that. The "B12.0 Refactoring of IMTool" effort is not critical and should not impact LDDTool for the near-term.   |
+---------------------------------------------------------------------+---------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `software
release summary (B12.0)`_

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

.. _plan B12.0: https://nasa-pds.github.io/releases/12.0/plan.html
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
.. _pds4-information-model#164: https://github.com/NASA-PDS/pds4-information-model/issues/164
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
.. _pds4-information-model#403: https://github.com/NASA-PDS/pds4-information-model/issues/403
.. _archive-analytics#2: https://github.com/NASA-PDS/archive-analytics/issues/2
.. _archive-analytics#7: https://github.com/NASA-PDS/archive-analytics/issues/7
.. _archive-analytics#16: https://github.com/NASA-PDS/archive-analytics/issues/16
.. _harvest#60: https://github.com/NASA-PDS/harvest/issues/60
.. _harvest#55: https://github.com/NASA-PDS/harvest/issues/55
.. _harvest#58: https://github.com/NASA-PDS/harvest/issues/58
.. _pds-api#24: https://github.com/NASA-PDS/pds-api/issues/24
.. _pds-api#67: https://github.com/NASA-PDS/pds-api/issues/67
.. _pds-api#76: https://github.com/NASA-PDS/pds-api/issues/76
.. _pds-api#80: https://github.com/NASA-PDS/pds-api/issues/80
.. _pds-api#75: https://github.com/NASA-PDS/pds-api/issues/75
.. _pds-api#91: https://github.com/NASA-PDS/pds-api/issues/91
.. _pds-api#101: https://github.com/NASA-PDS/pds-api/issues/101
.. _pds-api#105: https://github.com/NASA-PDS/pds-api/issues/105
.. _pds-api#77: https://github.com/NASA-PDS/pds-api/issues/77
.. _pds-api#56: https://github.com/NASA-PDS/pds-api/issues/56
.. _pds-api#59: https://github.com/NASA-PDS/pds-api/issues/59
.. _pds-api#60: https://github.com/NASA-PDS/pds-api/issues/60
.. _pds-api#61: https://github.com/NASA-PDS/pds-api/issues/61
.. _pds-api#62: https://github.com/NASA-PDS/pds-api/issues/62
.. _pds-api#79: https://github.com/NASA-PDS/pds-api/issues/79
.. _pds-api#81: https://github.com/NASA-PDS/pds-api/issues/81
.. _pds-api#74: https://github.com/NASA-PDS/pds-api/issues/74
.. _pds-api#83: https://github.com/NASA-PDS/pds-api/issues/83
.. _pds-api#84: https://github.com/NASA-PDS/pds-api/issues/84
.. _pds-api#99: https://github.com/NASA-PDS/pds-api/issues/99
.. _pds-api#73: https://github.com/NASA-PDS/pds-api/issues/73
.. _pds-api#96: https://github.com/NASA-PDS/pds-api/issues/96
.. _pds-api#107: https://github.com/NASA-PDS/pds-api/issues/107
.. _pds-api-client#6: https://github.com/NASA-PDS/pds-api-client/issues/6
.. _pds-deep-archive#105: https://github.com/NASA-PDS/pds-deep-archive/issues/105
.. _pds-deep-archive#7: https://github.com/NASA-PDS/pds-deep-archive/issues/7
.. _pds-deep-archive#106: https://github.com/NASA-PDS/pds-deep-archive/issues/106
.. _pds-deep-archive#115: https://github.com/NASA-PDS/pds-deep-archive/issues/115
.. _pds-deep-archive#116: https://github.com/NASA-PDS/pds-deep-archive/issues/116
.. _pds-doi-service#86: https://github.com/NASA-PDS/pds-doi-service/issues/86
.. _pds-doi-service#90: https://github.com/NASA-PDS/pds-doi-service/issues/90
.. _pds-doi-service#145: https://github.com/NASA-PDS/pds-doi-service/issues/145
.. _pds-doi-service#187: https://github.com/NASA-PDS/pds-doi-service/issues/187
.. _pds-doi-service#178: https://github.com/NASA-PDS/pds-doi-service/issues/178
.. _pds-doi-service#163: https://github.com/NASA-PDS/pds-doi-service/issues/163
.. _pds-doi-service#180: https://github.com/NASA-PDS/pds-doi-service/issues/180
.. _pds-doi-service#188: https://github.com/NASA-PDS/pds-doi-service/issues/188
.. _pds-doi-service#179: https://github.com/NASA-PDS/pds-doi-service/issues/179
.. _pds-doi-service#203: https://github.com/NASA-PDS/pds-doi-service/issues/203
.. _pds-doi-service#191: https://github.com/NASA-PDS/pds-doi-service/issues/191
.. _pds-doi-service#220: https://github.com/NASA-PDS/pds-doi-service/issues/220
.. _pds-doi-service#171: https://github.com/NASA-PDS/pds-doi-service/issues/171
.. _pds-doi-service#172: https://github.com/NASA-PDS/pds-doi-service/issues/172
.. _pds-doi-service#174: https://github.com/NASA-PDS/pds-doi-service/issues/174
.. _pds-doi-service#175: https://github.com/NASA-PDS/pds-doi-service/issues/175
.. _pds-doi-service#198: https://github.com/NASA-PDS/pds-doi-service/issues/198
.. _pds-doi-service#228: https://github.com/NASA-PDS/pds-doi-service/issues/228
.. _pds-doi-service#162: https://github.com/NASA-PDS/pds-doi-service/issues/162
.. _pds-doi-service#165: https://github.com/NASA-PDS/pds-doi-service/issues/165
.. _pds-doi-service#227: https://github.com/NASA-PDS/pds-doi-service/issues/227
.. _pds-doi-service#229: https://github.com/NASA-PDS/pds-doi-service/issues/229
.. _pds-doi-ui#60: https://github.com/NASA-PDS/pds-doi-ui/issues/60
.. _pds-doi-ui#22: https://github.com/NASA-PDS/pds-doi-ui/issues/22
.. _pds-doi-ui#35: https://github.com/NASA-PDS/pds-doi-ui/issues/35
.. _pds-doi-ui#70: https://github.com/NASA-PDS/pds-doi-ui/issues/70
.. _pds-doi-ui#25: https://github.com/NASA-PDS/pds-doi-ui/issues/25
.. _pds-doi-ui#34: https://github.com/NASA-PDS/pds-doi-ui/issues/34
.. _pds-doi-ui#41: https://github.com/NASA-PDS/pds-doi-ui/issues/41
.. _pds-doi-ui#42: https://github.com/NASA-PDS/pds-doi-ui/issues/42
.. _pds-doi-ui#65: https://github.com/NASA-PDS/pds-doi-ui/issues/65
.. _pds-doi-ui#71: https://github.com/NASA-PDS/pds-doi-ui/issues/71
.. _pds-doi-ui#1: https://github.com/NASA-PDS/pds-doi-ui/issues/1
.. _pds-doi-ui#9: https://github.com/NASA-PDS/pds-doi-ui/issues/9
.. _pds-doi-ui#10: https://github.com/NASA-PDS/pds-doi-ui/issues/10
.. _pds-doi-ui#48: https://github.com/NASA-PDS/pds-doi-ui/issues/48
.. _pds-doi-ui#49: https://github.com/NASA-PDS/pds-doi-ui/issues/49
.. _pds-doi-ui#50: https://github.com/NASA-PDS/pds-doi-ui/issues/50
.. _pds-doi-ui#54: https://github.com/NASA-PDS/pds-doi-ui/issues/54
.. _pds-doi-ui#75: https://github.com/NASA-PDS/pds-doi-ui/issues/75
.. _pds-doi-ui#79: https://github.com/NASA-PDS/pds-doi-ui/issues/79
.. _pds-doi-ui#82: https://github.com/NASA-PDS/pds-doi-ui/issues/82
.. _pds-registry-app#26: https://github.com/NASA-PDS/pds-registry-app/issues/26
.. _pds-registry-app#152: https://github.com/NASA-PDS/pds-registry-app/issues/152
.. _pds-registry-app#155: https://github.com/NASA-PDS/pds-registry-app/issues/155
.. _pds-registry-app#153: https://github.com/NASA-PDS/pds-registry-app/issues/153
.. _pds-registry-app#154: https://github.com/NASA-PDS/pds-registry-app/issues/154
.. _pds-registry-app#163: https://github.com/NASA-PDS/pds-registry-app/issues/163
.. _pds-registry-app#12: https://github.com/NASA-PDS/pds-registry-app/issues/12
.. _pds-registry-app#130: https://github.com/NASA-PDS/pds-registry-app/issues/130
.. _pds-registry-app#147: https://github.com/NASA-PDS/pds-registry-app/issues/147
.. _pds-registry-app#122: https://github.com/NASA-PDS/pds-registry-app/issues/122
.. _pds-registry-app#150: https://github.com/NASA-PDS/pds-registry-app/issues/150
.. _pds-registry-app#165: https://github.com/NASA-PDS/pds-registry-app/issues/165
.. _pds-wds-web#25: https://github.com/NASA-PDS/pds-wds-web/issues/25
.. _PDS.nasa.gov-Search#33: https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/33
.. _PDS.nasa.gov-UX#74: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/74
.. _PDS.nasa.gov-UX#73: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/73
.. _PDS.nasa.gov-UX#75: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/75
.. _PDS.nasa.gov-UX#79: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/79
.. _PDS.nasa.gov-UX#81: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/81
.. _PDS.nasa.gov-UX#86: https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/86
.. _pds4-information-model#306: https://github.com/NASA-PDS/pds4-information-model/issues/306
.. _pds4-information-model#349: https://github.com/NASA-PDS/pds4-information-model/issues/349
.. _pds4-information-model#347: https://github.com/NASA-PDS/pds4-information-model/issues/347
.. _pds4-information-model#348: https://github.com/NASA-PDS/pds4-information-model/issues/348
.. _pds4-information-model#326: https://github.com/NASA-PDS/pds4-information-model/issues/326
.. _pds4-information-model#240: https://github.com/NASA-PDS/pds4-information-model/issues/240
.. _pds4-information-model#330: https://github.com/NASA-PDS/pds4-information-model/issues/330
.. _pds4-information-model#338: https://github.com/NASA-PDS/pds4-information-model/issues/338
.. _pds4-information-model#346: https://github.com/NASA-PDS/pds4-information-model/issues/346
.. _pds4-information-model#350: https://github.com/NASA-PDS/pds4-information-model/issues/350
.. _pds4-information-model#356: https://github.com/NASA-PDS/pds4-information-model/issues/356
.. _pds4-information-model#357: https://github.com/NASA-PDS/pds4-information-model/issues/357
.. _pds4-information-model#358: https://github.com/NASA-PDS/pds4-information-model/issues/358
.. _pds4-information-model#359: https://github.com/NASA-PDS/pds4-information-model/issues/359
.. _pds4-information-model#368: https://github.com/NASA-PDS/pds4-information-model/issues/368
.. _pds4-information-model#324: https://github.com/NASA-PDS/pds4-information-model/issues/324
.. _pds4-information-model#369: https://github.com/NASA-PDS/pds4-information-model/issues/369
.. _pds4-information-model#391: https://github.com/NASA-PDS/pds4-information-model/issues/391
.. _pds4-information-model#397: https://github.com/NASA-PDS/pds4-information-model/issues/397
.. _pds4-jparser#40: https://github.com/NASA-PDS/pds4-jparser/issues/40
.. _PLAID#21: https://github.com/NASA-PDS/PLAID/issues/21
.. _PLAID#25: https://github.com/NASA-PDS/PLAID/issues/25
.. _PLAID#15: https://github.com/NASA-PDS/PLAID/issues/15
.. _registry-api-service#16: https://github.com/NASA-PDS/registry-api-service/issues/16
.. _registry-api-service#17: https://github.com/NASA-PDS/registry-api-service/issues/17
.. _registry-api-service#27: https://github.com/NASA-PDS/registry-api-service/issues/27
.. _registry-api-service#43: https://github.com/NASA-PDS/registry-api-service/issues/43
.. _registry-api-service#51: https://github.com/NASA-PDS/registry-api-service/issues/51
.. _registry-api-service#10: https://github.com/NASA-PDS/registry-api-service/issues/10
.. _registry-api-service#13: https://github.com/NASA-PDS/registry-api-service/issues/13
.. _registry-api-service#14: https://github.com/NASA-PDS/registry-api-service/issues/14
.. _registry-api-service#47: https://github.com/NASA-PDS/registry-api-service/issues/47
.. _validate#317: https://github.com/NASA-PDS/validate/issues/317
.. _validate#69: https://github.com/NASA-PDS/validate/issues/69
.. _validate#308: https://github.com/NASA-PDS/validate/issues/308
.. _validate#358: https://github.com/NASA-PDS/validate/issues/358
.. _validate#368: https://github.com/NASA-PDS/validate/issues/368
.. _validate#372: https://github.com/NASA-PDS/validate/issues/372
.. _validate#318: https://github.com/NASA-PDS/validate/issues/318
.. _validate#57: https://github.com/NASA-PDS/validate/issues/57
.. _validate#164: https://github.com/NASA-PDS/validate/issues/164
.. _validate#303: https://github.com/NASA-PDS/validate/issues/303
.. _validate#314: https://github.com/NASA-PDS/validate/issues/314
.. _validate#319: https://github.com/NASA-PDS/validate/issues/319
.. _validate#310: https://github.com/NASA-PDS/validate/issues/310
.. _validate#325: https://github.com/NASA-PDS/validate/issues/325
.. _validate#326: https://github.com/NASA-PDS/validate/issues/326
.. _validate#327: https://github.com/NASA-PDS/validate/issues/327
.. _validate#357: https://github.com/NASA-PDS/validate/issues/357
.. _validate#360: https://github.com/NASA-PDS/validate/issues/360
.. _validate#361: https://github.com/NASA-PDS/validate/issues/361
.. _validate#364: https://github.com/NASA-PDS/validate/issues/364
.. _validate#366: https://github.com/NASA-PDS/validate/issues/366
.. _validate#375: https://github.com/NASA-PDS/validate/issues/375
.. _validate#379: https://github.com/NASA-PDS/validate/issues/379
.. _validate#380: https://github.com/NASA-PDS/validate/issues/380
.. _validate#381: https://github.com/NASA-PDS/validate/issues/381
.. _validate#392: https://github.com/NASA-PDS/validate/issues/392
.. _validate#373: https://github.com/NASA-PDS/validate/issues/373
.. _validate#374: https://github.com/NASA-PDS/validate/issues/374
.. _pds-swg_11: https://github.com/NASA-PDS/pds-swg/issues/11
.. _software release summary (B12.0): https://nasa-pds.github.io/releases/B12.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Sotware Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
