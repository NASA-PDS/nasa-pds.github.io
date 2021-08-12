=========================================
Release Description Document (build 11.1)
=========================================
This release of the PDS4 System is intended as an operational release of
the system components to date. The following sections can be found in
this document:
The original plan for this release can be found here: `plan B11.1`_

.. toctree::
   :glob: 
   :maxdepth: 2

   rdd.rst

PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information
Model approved by the PDS4 Change Control Board and implemented by the
PDS within the latest build period.

+--------------------------------+----------------------------------------------------------------------------------------------------+
|Ref                             |Title                                                                                               |
+================================+====================================================================================================+
|`pds4-information-model#166`_   |CCB-285:  GeoTIFF format as operational PDS4 image                                                  |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#270`_   |CCB-323: Fix schema formation rule for lidvid_reference (Part II)                                   |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#250`_   |CCB-315: "PDS3" is an allowed parsing standard for Bundle documentation file                        |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#252`_   |CCB-304: Cleanup unused Vector classes in IM before 2.0.0.0                                         |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#253`_   |CCB-313: Definition of <external_source_product_identifier> refers to non-existent documentation    |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#254`_   |CCB-305: Missing validation constraint on <specified_unit_id>                                       |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#255`_   |CCB-300: Apparently deprecated units of measure are not actually deprecated                         |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#256`_   |CCB-312: <ldd_version_id> does not appear to be constrained the way LDDTool expects                 |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#257`_   |CCB-302: No <reference_type> values defined in DD_Attribute or DD_Class contexts                    |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#273`_   |CCB-317: Add FITS 4.0 to parsing_standard_id enumerated values for Header object                    |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#275`_   |CCB-313: Definition of <external_source_product_identifier> refers to non-existent documentation.   |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#288`_   |CCB-321: Add MPEG-4 as an encoding_standard_id for Product_Native                                   |
+--------------------------------+----------------------------------------------------------------------------------------------------+
|`pds4-information-model#339`_   |CCB-328 : Inconsistency in <title> type definition                                                  |
+--------------------------------+----------------------------------------------------------------------------------------------------+

Software changes
================
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

+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                   |Priority / Bug Severity   |
+========================================================================================================================================================+==========================+
|`pds4-information-model#175`_ LDDTool: Displaying invalid Imaging Discipline Classes                                                                    |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#188`_ LDDTool: requires one class with (element_flag = true), even when no classes defined                                      |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#266`_ Throw WARNING message when enumeration_flag = false but enumerations are specified                                        |s.low                     |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#271`_ LDDTool forces use of LDD versions based upon config                                                                      |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#277`_ LDD versionId list in the Data Dictionary Document introduction does not contain valid versionIds                         |s.low                     |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#280`_ CSV files fail to escape double quotes.                                                                                   |s.low                     |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#283`_ LDDTool generated LIDs for XML Schema Label Products  do not contain IM or LDD Version Ids                                |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#302`_ LDDTool does not allow the bundle to be specified for generated dictionaries                                              |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#304`_ LDDTool does not include the PSA namespace                                                                                |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#312`_ LDDTool does not generate the complete "All LDD" version of the  WebHelp PDS4 Data Dictionary Document                    |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#316`_ The 1F00 directory is missing from the Data directory for the 1G00 development release.                                   |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#322`_ LDDTool generates a 1C00 file when -V 1B00 is specified                                                                   |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#327`_ Repo tests fail when trying to run back-to-back maven steps                                                               |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#328`_ LDDTool outputs invalid schema with v13.0.0                                                                               |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#331`_ Invalid output schema when trying to set an Internal_Reference reference_type value set                                   |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#339`_ CCB-328 : Inconsistency in <title> type definition                                                                        |s.low                     |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#342`_ Version flag does not return the latest information for the tool                                                          |s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#367`_ LDDTool does not generate valid xpath for schematron rules for classes defined using associate_external_class             |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#371`_ The Version Id of the Product_XML_Schema label is not being set to the proper value.                                      |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#378`_ IMTool/LDDTool still attempts to process dLDD ingested into Protege                                                       |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#391`_ Issue with DD_Associate_External_Class when trying to reference pds:Internal_Reference and pds:Local_Internal_Reference   |s.high                    |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                |Priority / Bug Severity   |
+=====================================================================================================================================================+==========================+
|`pds4-information-model#167`_ LDDTool: Use sch:value-of to display a variable in Schematron validation                                               |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#238`_ Continuing refactoring of IMTool / LDDTool                                                                             |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#241`_ Improvements from Build 11.0 testing                                                                                   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#242`_ DocBook HTML/WebHelp generation and conversion processes                                                               |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#293`_ Update JSON output to include dependencies in output                                                                   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#298`_ Add title to Rule Assertion to allow generation of regression tests.                                                   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#332`_ [namespace-registry] add new namespace "<clementine>"                                                                  |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#344`_ [namespace-registry] add new namespace "ctli"                                                                          |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#352`_ [namespace-registry] add new namespace "m2020"                                                                         |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#353`_ [namespace-registry] add new namespace "ml"                                                                            |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#369`_ Evolution of CCB-256: Need method for providing permissible value definitions for external namespaces in Ingest_LDD.   |unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#373`_ [namespace-registry] update path "<clementine>" in registry PDF (possibly shorten name)                                |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#374`_ [namespace-registry] add new namespace "clipper"                                                                       |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#386`_ [namespace-registry] add new namespace "Earth-Based Telescope Namespace"                                               |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                 |Priority / Bug Severity   |
+======================================================================================================================================+==========================+
|`pds4-information-model#330`_ As a user I want to know the output of the tool after it completes execution.                           |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#338`_ As a developer, I want to know the dLDD version from the output JSON data                               |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`pds4-information-model#361`_ As a developer I want to generate a query model that relates semantically similar permissible values.   |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

theme
~~~~~

+-----------------------------------------------------------------------------+--------------------------+
|Issue                                                                        |Priority / Bug Severity   |
+=============================================================================+==========================+
|`pds4-information-model#349`_ Establish LDD Management Teams and Processes   |unknown                   |
+-----------------------------------------------------------------------------+--------------------------+

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
|`validate#189`_ Validate error reading tables > 2GiB                                                                                                        |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#240`_ Unexpected error for data collection in a sub-directory                                                                                     |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#256`_ validate should only do integrity checking on latest version of a collection when referenced by LID                                         |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#257`_ Product with incorrect table binary definition pass validation                                                                              |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#260`_ Missing documentation about deprecated flags                                                                                                |s.low                     |
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
|`validate#297`_ Content validation of ASCII_Integer field does not accept value with leading zeroes                                                         |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#298`_ validate misses double quotes within a delimited table                                                                                      |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#299`_ Validate tool does not PASS a bundle with a single-character filename                                                                       |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#300`_ validate -u flag reports an error on Windows                                                                                                |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#301`_ unclear error message for field count matching                                                                                              |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#310`_ Validate missing collections in bundle after CCB-282 updates                                                                                |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#325`_ Validate Incorrectly Throws Error When Embedded Field_Character Contains <CR><LF>                                                           |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#326`_ File-size check fails for large data files                                                                                                  |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#327`_ validate fails to process large data file                                                                                                   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#356`_ validate labels error.sub_directory.unallowed_name as a warning                                                                             |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#357`_ Validate allows CRLF within a Table_Delimited field                                                                                         |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#360`_ validate does not parse colon in Windows path                                                                                               |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#364`_ validate does not allow ".XML" as an extension for a label file                                                                             |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#366`_ validate should not check if file is PDF/A if --skip-content-validation is enabled                                                          |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#378`_ validate raises an unexpected error with doi attribute in the Citation_information class                                                    |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#381`_ validate does not work correctly when the path name contains a space                                                                        |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                            |Priority / Bug Severity   |
+=================================================================================================================+==========================+
|`validate#17`_ Validate schematron references and throw fatal error if invalid URI specified                     |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#24`_ Update context check to retrieve and use latest context products from EN Registry                 |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#51`_ Provide the capability to specify multiple locations for pds4.bundle validation                   |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#81`_ Validate and throw error when duplicate LIDs are found in Bundle                                  |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#230`_ Update validate per SR requirements for collection inventories                                   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#238`_ validate does not perform full bundle validation when using a specific bundle.xml                |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#246`_ Add output directory flag to validate-bundle tool                                                |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#249`_ Improvements for validating accumulating bundles / collections                                   |unknown                   |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#252`_ Implement initial behavioral testing framework with cucumber                                     |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#254`_ validate does not perform expediently when doing bundle-level validation against large bundles   |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#264`_ Update installation documentation to include 64-bit Java as system requirement                   |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#290`_ Migrate subset of existing regression tests to cucumber behavioral testing                       |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#322`_ Update installation documentation to require Java 1.9+                                           |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#323`_ Upgrade to Java 9+                                                                               |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#355`_ Improve validate reporting when trying to read a null row                                        |unknown                   |
+-----------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                                     |Priority / Bug Severity   |
+==========================================================================================================================================================================+==========================+
|`validate#57`_ As a user, I want to be warned when there are alphanumeric characters between fields in Table_Character                                                    |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#69`_ As a user, I want to validate that all context objects specified in observational products are referenced in the parent bundle/collection Reference_List   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#149`_ As a user, I want validate to check number of records/fields specified in label matches the records in the actual data table                              |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#164`_ As a user, I want to validate PDF files are PDF/A                                                                                                         |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#188`_ As a user, I want to validate a bundle that uses multiple versions of the Information Model / Discipline LDDs                                             |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#210`_ As a user, I want validate to raise a WARNING when differing versions of IM are used within a bundle                                                      |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#292`_ CCB-264: Make the Line Feed (LF) character an allowed record delimiter                                                                                    |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#303`_ As a user, I want to the raise a WARNING if the object-defined size in the label does not match the file_size value                                       |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#308`_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle                  |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#343`_ As a user I want to see the name of a table/array in errors, if one is specified                                                                          |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

theme
~~~~~

+-------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                        |Priority / Bug Severity   |
+=============================================================================================================+==========================+
|`validate#250`_ Improvements to meet updated Standards Reference since initial requirements implementation   |unknown                   |
+-------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#318`_ B12.0 Content Validation Improvements                                                        |unknown                   |
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

.. _plan B11.1: https://nasa-pds.github.io/releases/B11.1/plan.html
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
.. _pds4-information-model#339: https://github.com/NASA-PDS/pds4-information-model/issues/339
.. _pds4-information-model#342: https://github.com/NASA-PDS/pds4-information-model/issues/342
.. _pds4-information-model#367: https://github.com/NASA-PDS/pds4-information-model/issues/367
.. _pds4-information-model#371: https://github.com/NASA-PDS/pds4-information-model/issues/371
.. _pds4-information-model#378: https://github.com/NASA-PDS/pds4-information-model/issues/378
.. _pds4-information-model#391: https://github.com/NASA-PDS/pds4-information-model/issues/391
.. _pds4-information-model#167: https://github.com/NASA-PDS/pds4-information-model/issues/167
.. _pds4-information-model#238: https://github.com/NASA-PDS/pds4-information-model/issues/238
.. _pds4-information-model#241: https://github.com/NASA-PDS/pds4-information-model/issues/241
.. _pds4-information-model#242: https://github.com/NASA-PDS/pds4-information-model/issues/242
.. _pds4-information-model#293: https://github.com/NASA-PDS/pds4-information-model/issues/293
.. _pds4-information-model#298: https://github.com/NASA-PDS/pds4-information-model/issues/298
.. _pds4-information-model#332: https://github.com/NASA-PDS/pds4-information-model/issues/332
.. _pds4-information-model#344: https://github.com/NASA-PDS/pds4-information-model/issues/344
.. _pds4-information-model#352: https://github.com/NASA-PDS/pds4-information-model/issues/352
.. _pds4-information-model#353: https://github.com/NASA-PDS/pds4-information-model/issues/353
.. _pds4-information-model#369: https://github.com/NASA-PDS/pds4-information-model/issues/369
.. _pds4-information-model#373: https://github.com/NASA-PDS/pds4-information-model/issues/373
.. _pds4-information-model#374: https://github.com/NASA-PDS/pds4-information-model/issues/374
.. _pds4-information-model#386: https://github.com/NASA-PDS/pds4-information-model/issues/386
.. _pds4-information-model#330: https://github.com/NASA-PDS/pds4-information-model/issues/330
.. _pds4-information-model#338: https://github.com/NASA-PDS/pds4-information-model/issues/338
.. _pds4-information-model#361: https://github.com/NASA-PDS/pds4-information-model/issues/361
.. _pds4-information-model#349: https://github.com/NASA-PDS/pds4-information-model/issues/349
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
.. _validate#356: https://github.com/NASA-PDS/validate/issues/356
.. _validate#357: https://github.com/NASA-PDS/validate/issues/357
.. _validate#360: https://github.com/NASA-PDS/validate/issues/360
.. _validate#364: https://github.com/NASA-PDS/validate/issues/364
.. _validate#366: https://github.com/NASA-PDS/validate/issues/366
.. _validate#378: https://github.com/NASA-PDS/validate/issues/378
.. _validate#381: https://github.com/NASA-PDS/validate/issues/381
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
.. _validate#355: https://github.com/NASA-PDS/validate/issues/355
.. _validate#57: https://github.com/NASA-PDS/validate/issues/57
.. _validate#69: https://github.com/NASA-PDS/validate/issues/69
.. _validate#149: https://github.com/NASA-PDS/validate/issues/149
.. _validate#164: https://github.com/NASA-PDS/validate/issues/164
.. _validate#188: https://github.com/NASA-PDS/validate/issues/188
.. _validate#210: https://github.com/NASA-PDS/validate/issues/210
.. _validate#292: https://github.com/NASA-PDS/validate/issues/292
.. _validate#303: https://github.com/NASA-PDS/validate/issues/303
.. _validate#308: https://github.com/NASA-PDS/validate/issues/308
.. _validate#343: https://github.com/NASA-PDS/validate/issues/343
.. _validate#250: https://github.com/NASA-PDS/validate/issues/250
.. _validate#318: https://github.com/NASA-PDS/validate/issues/318
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
