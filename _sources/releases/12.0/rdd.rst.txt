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
|`validate#368`_ Product referential integrity check throws invalid WARNINGs                                                                                       |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#372`_ Issues with logic for reading latest version of collections, and file read logging lost with v2.* of validate                                     |s.medium                  |
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

enhancement
~~~~~~~~~~~

+-------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                |Priority / Bug Severity   |
+=====================================================================================+==========================+
|`validate#373`_ Update pds4 version mismatch warning message and problem type        |unknown                   |
+-------------------------------------------------------------------------------------+--------------------------+
|`validate#374`_ Refactor PDF/A check handling to match with similar product checks   |unknown                   |
+-------------------------------------------------------------------------------------+--------------------------+

requirement
~~~~~~~~~~~

+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                                     |Priority / Bug Severity   |
+==========================================================================================================================================================================+==========================+
|`validate#57`_ As a user, I want to be warned when there are alphanumeric characters between fields in Table_Character                                                    |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#69`_ As a user, I want to validate that all context objects specified in observational products are referenced in the parent bundle/collection Reference_List   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#164`_ As a user, I want to validate PDF files are PDF/A                                                                                                         |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#303`_ As a user, I want to the raise a WARNING if the object-defined size in the label does not match the file_size value                                       |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|`validate#308`_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle                  |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

theme
~~~~~

+--------------------------------------------------------+--------------------------+
|Issue                                                   |Priority / Bug Severity   |
+========================================================+==========================+
|`validate#318`_ B12.0 Content Validation Improvements   |unknown                   |
+--------------------------------------------------------+--------------------------+

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
.. _validate#310: https://github.com/NASA-PDS/validate/issues/310
.. _validate#325: https://github.com/NASA-PDS/validate/issues/325
.. _validate#326: https://github.com/NASA-PDS/validate/issues/326
.. _validate#327: https://github.com/NASA-PDS/validate/issues/327
.. _validate#357: https://github.com/NASA-PDS/validate/issues/357
.. _validate#360: https://github.com/NASA-PDS/validate/issues/360
.. _validate#361: https://github.com/NASA-PDS/validate/issues/361
.. _validate#364: https://github.com/NASA-PDS/validate/issues/364
.. _validate#366: https://github.com/NASA-PDS/validate/issues/366
.. _validate#368: https://github.com/NASA-PDS/validate/issues/368
.. _validate#372: https://github.com/NASA-PDS/validate/issues/372
.. _validate#375: https://github.com/NASA-PDS/validate/issues/375
.. _validate#379: https://github.com/NASA-PDS/validate/issues/379
.. _validate#380: https://github.com/NASA-PDS/validate/issues/380
.. _validate#381: https://github.com/NASA-PDS/validate/issues/381
.. _validate#392: https://github.com/NASA-PDS/validate/issues/392
.. _validate#373: https://github.com/NASA-PDS/validate/issues/373
.. _validate#374: https://github.com/NASA-PDS/validate/issues/374
.. _validate#57: https://github.com/NASA-PDS/validate/issues/57
.. _validate#69: https://github.com/NASA-PDS/validate/issues/69
.. _validate#164: https://github.com/NASA-PDS/validate/issues/164
.. _validate#303: https://github.com/NASA-PDS/validate/issues/303
.. _validate#308: https://github.com/NASA-PDS/validate/issues/308
.. _validate#318: https://github.com/NASA-PDS/validate/issues/318
.. _pds-swg_11: https://github.com/NASA-PDS/pds-swg/issues/11
.. _software release summary (B12.0): https://nasa-pds.github.io/releases/B12.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Sotware Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
