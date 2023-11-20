======================================
Software Catalog (Build 14.0-SNAPSHOT)
======================================
The software provided for the PDS System Build 14.0-SNAPSHOT are listed below and organized by category:

- `Standalone Tools`_

- `Libraries and Clients`_

- `Core Services`_


Standalone Tools
================
PDS Tools for Discipline Nodes, Data Providers and Community Users.

+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|tool                               |version           |last updated   |description                                                                                                                                                                         |l |manual|                                 |l |changelog|                                 |l |requirements|                       |l |download|                                 |l |license|                                 |l |feedback|                                 |
+===================================+==================+===============+====================================================================================================================================================================================+===========================================+==============================================+=======================================+=============================================+============================================+=============================================+
|PDS API Client                     |None              |N/A            |Python library and API for accessing the online PDS Search API.                                                                                                                     ||NASA-PDS/pds-api-client_manual|           ||NASA-PDS/pds-api-client_changelog|           |                                       ||NASA-PDS/pds-api-client_download|           ||NASA-PDS/pds-api-client_license|           ||NASA-PDS/pds-api-client_feedback|           |
+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|PDS Deep Archive                   |v1.2.0-dev        |2023-04-27     |PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators                              ||NASA-PDS/deep-archive_manual|             |                                              ||NASA-PDS/deep-archive_requirements|   ||NASA-PDS/deep-archive_download|             ||NASA-PDS/deep-archive_license|             ||NASA-PDS/deep-archive_feedback|             |
+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|Validate                           |v3.3.0-SNAPSHOT   |2023-05-31     |Validates PDS4 product labels, data and PDS3 Volumes                                                                                                                                ||NASA-PDS/validate_manual|                 |                                              |                                       ||NASA-PDS/validate_download|                 ||NASA-PDS/validate_license|                 ||NASA-PDS/validate_feedback|                 |
+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|PDS4 Information Model & LDDTool   |None              |N/A            |The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.                                                    ||NASA-PDS/pds4-information-model_manual|   ||NASA-PDS/pds4-information-model_changelog|   |                                       ||NASA-PDS/pds4-information-model_download|   ||NASA-PDS/pds4-information-model_license|   ||NASA-PDS/pds4-information-model_feedback|   |
+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|Transform                          |None              |N/A            |Transforms PDS3 and PDS4 product labels and data into various formats.                                                                                                              ||NASA-PDS/transform_manual|                ||NASA-PDS/transform_changelog|                |                                       ||NASA-PDS/transform_download|                ||NASA-PDS/transform_license|                ||NASA-PDS/transform_feedback|                |
+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|MILabel                            |v1.3.0-SNAPSHOT   |2022-12-19     |Metadata Injector for PDS Labels (MILabel) provides a command-line interface for generating PDS4 Labels using a user provided PDS4 XML template and input (source) data products.   ||NASA-PDS/mi-label_manual|                 ||NASA-PDS/mi-label_changelog|                 |                                       ||NASA-PDS/mi-label_download|                 ||NASA-PDS/mi-label_license|                 ||NASA-PDS/mi-label_feedback|                 |
+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|PLAID                              |None              |N/A            |APPS PDS Label Assistant for Interactive Design (PLAID). See an overview of the software on YouTube. https://www.youtube.com/watch?v=WCo8erW_rL8                                    ||NASA-PDS/PLAID_manual|                    ||NASA-PDS/PLAID_changelog|                    |                                       ||NASA-PDS/PLAID_download|                    ||NASA-PDS/PLAID_license|                    ||NASA-PDS/PLAID_feedback|                    |
+-----------------------------------+------------------+---------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+---------------------------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+

Libraries and Clients
=====================
Libraries and Clients for programing interfaces to PDS services and data.

+---------------+------------------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+----------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|tool           |version           |last updated   |description                                                                                                                                                                      |l |manual|                       |l |changelog|   |l |requirements|   |l |download|                       |l |license|                       |l |feedback|                       |
+===============+==================+===============+=================================================================================================================================================================================+=================================+================+===================+===================================+==================================+===================================+
|PDS4 JParser   |v2.6.0-SNAPSHOT   |2023-05-26     |Java Library providing APIs for parsing and exporting information on PDS4 products, including table and image objects to various formats including CSV, PNG, VICAR, FITs, etc.   ||NASA-PDS/pds4-jparser_manual|   |                |                   ||NASA-PDS/pds4-jparser_download|   ||NASA-PDS/pds4-jparser_license|   ||NASA-PDS/pds4-jparser_feedback|   |
+---------------+------------------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+----------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+

Core Services
=========================
Tools and Services centrally deployed by PDS Engineering Node to support the integration and interoperability of all PDS nodes.

+-------------------------+------------------+---------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+------------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|tool                     |version           |last updated   |description                                                                                                                                                                                                |l |manual|                       |l |changelog|                       |l |requirements|   |l |download|                       |l |license|                       |l |feedback|                       |
+=========================+==================+===============+===========================================================================================================================================================================================================+=================================+====================================+===================+===================================+==================================+===================================+
|PDS DOI Service          |None              |N/A            |Service and tools for generating DOIs for PDS bundles, collections, and data sets                                                                                                                          ||NASA-PDS/doi-service_manual|    ||NASA-PDS/doi-service_changelog|    |                   ||NASA-PDS/doi-service_download|    ||NASA-PDS/doi-service_license|    ||NASA-PDS/doi-service_feedback|    |
+-------------------------+------------------+---------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+------------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|PDS DOI User Interface   |None              |N/A            |The web interface for the PDS DOI Service providing the ability management PDS archive DOIs. See the DOI Service for more details on the available capabilities. https://nasa-pds.github.io/doi-service/   ||NASA-PDS/doi-ui_manual|         ||NASA-PDS/doi-ui_changelog|         |                   ||NASA-PDS/doi-ui_download|         ||NASA-PDS/doi-ui_license|         ||NASA-PDS/doi-ui_feedback|         |
+-------------------------+------------------+---------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+------------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|Harvest                  |v3.8.0-SNAPSHOT   |2023-05-11     |Standalone Harvest client application providing the functionality for capturing and indexing product metadata into the PDS Registry system (https://github.com/nasa-pds/registry).                         ||NASA-PDS/harvest_manual|        |                                    |                   ||NASA-PDS/harvest_download|        ||NASA-PDS/harvest_license|        ||NASA-PDS/harvest_feedback|        |
+-------------------------+------------------+---------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+------------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|Registry Manager         |None              |N/A            |Standalone Registry Manager application responsible for managing the PDS Registry (https://github.com/NASA-PDS/registry) schemas and indexes.                                                              ||NASA-PDS/registry-mgr_manual|   ||NASA-PDS/registry-mgr_changelog|   |                   ||NASA-PDS/registry-mgr_download|   ||NASA-PDS/registry-mgr_license|   ||NASA-PDS/registry-mgr_feedback|   |
+-------------------------+------------------+---------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+------------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+

.. |NASA-PDS/doi-service_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds-doi-service/
.. |NASA-PDS/doi-service_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/doi-service_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/doi-service_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds-doi-service/releases/tag/None
.. |NASA-PDS/doi-service_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds-doi-service/main/LICENSE.md
.. |NASA-PDS/doi-service_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds-doi-service/issues/new/choose
.. |NASA-PDS/doi-ui_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds-doi-ui/
.. |NASA-PDS/doi-ui_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/doi-ui_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/doi-ui_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds-doi-ui/releases/tag/None
.. |NASA-PDS/doi-ui_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds-doi-ui/main/LICENSE.md
.. |NASA-PDS/doi-ui_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds-doi-ui/issues/new/choose
.. |NASA-PDS/pds-api-client_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds-api-client/
.. |NASA-PDS/pds-api-client_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/pds-api-client_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/pds-api-client_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds-api-client/releases/tag/None
.. |NASA-PDS/pds-api-client_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds-api-client/main/LICENSE.md
.. |NASA-PDS/pds-api-client_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds-api-client/issues/new/choose
.. |NASA-PDS/deep-archive_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds-deep-archive/
.. |NASA-PDS/deep-archive_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: None
.. |NASA-PDS/deep-archive_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: https://github.com/NASA-PDS/pds-deep-archive/blob/main/docs/requirements/v1.2.0-dev/REQUIREMENTS.md
.. |NASA-PDS/deep-archive_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds-deep-archive/releases/tag/v1.2.0-dev
.. |NASA-PDS/deep-archive_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds-deep-archive/main/LICENSE.md
.. |NASA-PDS/deep-archive_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds-deep-archive/issues/new/choose
.. |NASA-PDS/validate_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/validate/
.. |NASA-PDS/validate_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: None
.. |NASA-PDS/validate_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/validate_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/validate/releases/tag/v3.3.0-SNAPSHOT
.. |NASA-PDS/validate_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/validate/main/LICENSE.md
.. |NASA-PDS/validate_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/validate/issues/new/choose
.. |NASA-PDS/pds4-information-model_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds4-information-model/
.. |NASA-PDS/pds4-information-model_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/pds4-information-model_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/pds4-information-model_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds4-information-model/releases/tag/None
.. |NASA-PDS/pds4-information-model_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds4-information-model/main/LICENSE.md
.. |NASA-PDS/pds4-information-model_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds4-information-model/issues/new/choose
.. |NASA-PDS/harvest_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/harvest/
.. |NASA-PDS/harvest_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: None
.. |NASA-PDS/harvest_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/harvest_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/harvest/releases/tag/v3.8.0-SNAPSHOT
.. |NASA-PDS/harvest_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/harvest/main/LICENSE.md
.. |NASA-PDS/harvest_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/harvest/issues/new/choose
.. |NASA-PDS/registry-mgr_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds-registry-mgr-elastic/
.. |NASA-PDS/registry-mgr_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/registry-mgr_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/registry-mgr_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds-registry-mgr-elastic/releases/tag/None
.. |NASA-PDS/registry-mgr_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds-registry-mgr-elastic/main/LICENSE.md
.. |NASA-PDS/registry-mgr_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds-registry-mgr-elastic/issues/new/choose
.. |NASA-PDS/transform_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/transform/
.. |NASA-PDS/transform_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/transform_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/transform_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/transform/releases/tag/None
.. |NASA-PDS/transform_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/transform/main/LICENSE.md
.. |NASA-PDS/transform_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/transform/issues/new/choose
.. |NASA-PDS/pds4-jparser_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds4-jparser/
.. |NASA-PDS/pds4-jparser_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: None
.. |NASA-PDS/pds4-jparser_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/pds4-jparser_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds4-jparser/releases/tag/v2.6.0-SNAPSHOT
.. |NASA-PDS/pds4-jparser_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds4-jparser/main/LICENSE.md
.. |NASA-PDS/pds4-jparser_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds4-jparser/issues/new/choose
.. |NASA-PDS/mi-label_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/mi-label/
.. |NASA-PDS/mi-label_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/mi-label/blob/main/CHANGELOG.md#v130-snapshot-2022-11-17
.. |NASA-PDS/mi-label_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/mi-label_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/mi-label/releases/tag/v1.3.0-SNAPSHOT
.. |NASA-PDS/mi-label_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/mi-label/main/LICENSE.md
.. |NASA-PDS/mi-label_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/mi-label/issues/new/choose
.. |NASA-PDS/PLAID_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://github.com/NASA-PDS/PLAID
.. |NASA-PDS/PLAID_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/PLAID_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/PLAID_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/PLAID/releases/tag/None
.. |NASA-PDS/PLAID_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/PLAID/main/LICENSE.md
.. |NASA-PDS/PLAID_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/PLAID/issues/new/choose
.. |manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual_text.png
   :alt: manual
.. |changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog_text.png
   :alt: changelog
.. |requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements_text.png
   :alt: requirements
.. |download| image:: https://nasa-pds.github.io/pdsen-corral/images/download_text.png
   :alt: download
.. |license| image:: https://nasa-pds.github.io/pdsen-corral/images/license_text.png
   :alt: license
.. |feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback_text.png
   :alt: feedback
