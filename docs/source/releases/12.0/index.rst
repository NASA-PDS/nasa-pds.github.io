=============================
Software Catalog (build 12.0)
=============================
The software provided for the build 12.0 are listed hereafter and
organized by category:

- `Standalone Tools and Libraries`_

- `Discipline Node Services`_

- `Libraries`_

- `Engineering Node Services`_

- `Other Tools and Libraries (dependencies)`_

Standalone Tools and Libraries
==============================
PDS tools for discipline nodes, data providers and users.

+-----------------------------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+-------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|tool                               |version   |last updated   |description                                                                                                                                              |l |manual|                                 |l |changelog|                                 |l |requirements|   |l |download|                                 |l |license|                                 |l |feedback|                                 |
+===================================+==========+===============+=========================================================================================================================================================+===========================================+==============================================+===================+=============================================+============================================+=============================================+
|PDS Deep Archive                   |v1.1.0    |2021-09-29     |PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators   ||NASA-PDS/deep-archive_manual|             ||NASA-PDS/deep-archive_changelog|             |                   ||NASA-PDS/deep-archive_download|             ||NASA-PDS/deep-archive_license|             ||NASA-PDS/deep-archive_feedback|             |
+-----------------------------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+-------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|Validate                           |v2.1.3    |2021-12-16     |Validates PDS4 product labels, data and PDS3 Volumes                                                                                                     ||NASA-PDS/validate_manual|                 ||NASA-PDS/validate_changelog|                 |                   ||NASA-PDS/validate_download|                 ||NASA-PDS/validate_license|                 ||NASA-PDS/validate_feedback|                 |
+-----------------------------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+-------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|PDS4 Information Model & LDDTool   |v13.1.0   |2021-10-05     |The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.                         ||NASA-PDS/pds4-information-model_manual|   ||NASA-PDS/pds4-information-model_changelog|   |                   ||NASA-PDS/pds4-information-model_download|   ||NASA-PDS/pds4-information-model_license|   ||NASA-PDS/pds4-information-model_feedback|   |
+-----------------------------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+-------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|Transform                          |v1.11.1   |2019-12-13     |Transforms PDS3 and PDS4 product labels and data into various formats.                                                                                   ||NASA-PDS/transform_manual|                ||NASA-PDS/transform_changelog|                |                   ||NASA-PDS/transform_download|                ||NASA-PDS/transform_license|                ||NASA-PDS/transform_feedback|                |
+-----------------------------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+-------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+
|MILabel                            |None      |N/A            |Metadata Injector for PDS Labels (MILabel), formerly known as Generate Tool                                                                              ||NASA-PDS/mi-label_manual|                 ||NASA-PDS/mi-label_changelog|                 |                   ||NASA-PDS/mi-label_download|                 ||NASA-PDS/mi-label_license|                 ||NASA-PDS/mi-label_feedback|                 |
+-----------------------------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------+----------------------------------------------+-------------------+---------------------------------------------+--------------------------------------------+---------------------------------------------+

Discipline Node Services
========================
PDS servers that Discipline Node should deploy to publish their archive
at PDS level

+-------------------+----------+---------------+-----------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------+----------------------------------------+-------------------------------------------+---------------------------------------+--------------------------------------+---------------------------------------+
|tool               |version   |last updated   |description                                                                                                                                          |l |manual|                           |l |changelog|                           |l |requirements|                           |l |download|                           |l |license|                           |l |feedback|                           |
+===================+==========+===============+=====================================================================================================================================================+=====================================+========================================+===========================================+=======================================+======================================+=======================================+
|PDS Registry App   |v1.0.2    |2021-12-10     |Registry application enabling a PDS node to register all its data products for long term preservation and sharing with the rest of the PDS system.   ||NASA-PDS/pds-registry-app_manual|   ||NASA-PDS/pds-registry-app_changelog|   ||NASA-PDS/pds-registry-app_requirements|   ||NASA-PDS/pds-registry-app_download|   ||NASA-PDS/pds-registry-app_license|   ||NASA-PDS/pds-registry-app_feedback|   |
+-------------------+----------+---------------+-----------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------+----------------------------------------+-------------------------------------------+---------------------------------------+--------------------------------------+---------------------------------------+

Libraries
=========
Libraries supported by PDS

+-----------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------------------+----------------+-------------------+-------------------------------------+------------------------------------+-------------------------------------+
|tool             |version   |last updated   |description                                                                                                                                                                      |l |manual|                         |l |changelog|   |l |requirements|   |l |download|                         |l |license|                         |l |feedback|                         |
+=================+==========+===============+=================================================================================================================================================================================+===================================+================+===================+=====================================+====================================+=====================================+
|PDS API Client   |v0.7.1    |2021-10-01     |PDS API Client                                                                                                                                                                   ||NASA-PDS/pds-api-client_manual|   |                |                   ||NASA-PDS/pds-api-client_download|   ||NASA-PDS/pds-api-client_license|   ||NASA-PDS/pds-api-client_feedback|   |
+-----------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------------------+----------------+-------------------+-------------------------------------+------------------------------------+-------------------------------------+
|PDS4 JParser     |v2.1.1    |2021-12-10     |Java Library providing APIs for parsing and exporting information on PDS4 products, including table and image objects to various formats including CSV, PNG, VICAR, FITs, etc.   ||NASA-PDS/pds4-jparser_manual|     |                |                   ||NASA-PDS/pds4-jparser_download|     ||NASA-PDS/pds4-jparser_license|     ||NASA-PDS/pds4-jparser_feedback|     |
+-----------------+----------+---------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------------------+----------------+-------------------+-------------------------------------+------------------------------------+-------------------------------------+

Engineering Node Services
=========================
PDS servers deployed by PDS Engineering Node at central level

+-------------------------------+----------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+-----------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|tool                           |version   |last updated   |description                                                                                                                                                                                                                                                        |l |manual|                       |l |changelog|                      |l |requirements|   |l |download|                       |l |license|                       |l |feedback|                       |
+===============================+==========+===============+===================================================================================================================================================================================================================================================================+=================================+===================================+===================+===================================+==================================+===================================+
|PDS DOI Service                |v2.1.1    |2021-12-07     |Service and tools for generating DOIs for PDS bundles, collections, and data sets                                                                                                                                                                                  ||NASA-PDS/doi-service_manual|    ||NASA-PDS/doi-service_changelog|   |                   ||NASA-PDS/doi-service_download|    ||NASA-PDS/doi-service_license|    ||NASA-PDS/doi-service_feedback|    |
+-------------------------------+----------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+-----------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|Harvest                        |v3.5.1    |2021-12-10     |Provides software provides functionality for capturing and indexing product metadata in PDS Registry. A sub-component of the PDS Registry App (https://github.com/NASA-PDS/pds-registry-app)                                                                       ||NASA-PDS/harvest_manual|        ||NASA-PDS/harvest_changelog|       |                   ||NASA-PDS/harvest_download|        ||NASA-PDS/harvest_license|        ||NASA-PDS/harvest_feedback|        |
+-------------------------------+----------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+-----------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+
|PDS Registry Manager Elastic   |v4.3.0    |2021-12-10     |Tool for managing the Elastic Search back-end Registry Service for tracking, searching, auditing, locating, and maintaining artifacts within the Planetary Data System. See new PDS Registry App for more details (https://github.com/NASA-PDS/pds-registry-app)   ||NASA-PDS/registry-mgr_manual|   |                                   |                   ||NASA-PDS/registry-mgr_download|   ||NASA-PDS/registry-mgr_license|   ||NASA-PDS/registry-mgr_feedback|   |
+-------------------------------+----------+---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+---------------------------------+-----------------------------------+-------------------+-----------------------------------+----------------------------------+-----------------------------------+

.. |NASA-PDS/doi-service_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/doi-service/
.. |NASA-PDS/doi-service_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/doi-service/blob/main/CHANGELOG.md#v211-2021-12-07
.. |NASA-PDS/doi-service_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/doi-service_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/doi-service/releases/tag/v2.1.1
.. |NASA-PDS/doi-service_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/doi-service/main/LICENSE.md
.. |NASA-PDS/doi-service_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/doi-service/issues/new/choose
.. |NASA-PDS/pds-registry-app_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds-registry-app/
.. |NASA-PDS/pds-registry-app_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/pds-registry-app/blob/main/CHANGELOG.md#v102-2021-12-10
.. |NASA-PDS/pds-registry-app_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: https://github.com/NASA-PDS/pds-registry-app/blob/main/docs/requirements/v1.0.2/REQUIREMENTS.md
.. |NASA-PDS/pds-registry-app_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds-registry-app/releases/tag/v1.0.2
.. |NASA-PDS/pds-registry-app_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds-registry-app/main/LICENSE.md
.. |NASA-PDS/pds-registry-app_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds-registry-app/issues/new/choose
.. |NASA-PDS/pds-api-client_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds-api-client/
.. |NASA-PDS/pds-api-client_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: None
.. |NASA-PDS/pds-api-client_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/pds-api-client_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds-api-client/releases/tag/v0.7.1
.. |NASA-PDS/pds-api-client_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds-api-client/main/LICENSE.md
.. |NASA-PDS/pds-api-client_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds-api-client/issues/new/choose
.. |NASA-PDS/deep-archive_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/deep-archive/
.. |NASA-PDS/deep-archive_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/deep-archive/blob/main/CHANGELOG.md#v110-2021-09-29
.. |NASA-PDS/deep-archive_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/deep-archive_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/deep-archive/releases/tag/v1.1.0
.. |NASA-PDS/deep-archive_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/deep-archive/main/LICENSE.md
.. |NASA-PDS/deep-archive_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/deep-archive/issues/new/choose
.. |NASA-PDS/validate_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/validate/
.. |NASA-PDS/validate_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/validate/blob/main/CHANGELOG.md#v213-2021-12-16
.. |NASA-PDS/validate_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/validate_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/validate/releases/tag/v2.1.3
.. |NASA-PDS/validate_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/validate/main/LICENSE.md
.. |NASA-PDS/validate_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/validate/issues/new/choose
.. |NASA-PDS/pds4-information-model_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/pds4-information-model/
.. |NASA-PDS/pds4-information-model_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/pds4-information-model/blob/main/CHANGELOG.md#v1310-2021-10-05
.. |NASA-PDS/pds4-information-model_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/pds4-information-model_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/pds4-information-model/releases/tag/v13.1.0
.. |NASA-PDS/pds4-information-model_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds4-information-model/main/LICENSE.md
.. |NASA-PDS/pds4-information-model_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds4-information-model/issues/new/choose
.. |NASA-PDS/harvest_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/harvest/
.. |NASA-PDS/harvest_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/harvest/blob/main/CHANGELOG.md#v351-2021-12-10
.. |NASA-PDS/harvest_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/harvest_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/harvest/releases/tag/v3.5.1
.. |NASA-PDS/harvest_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/harvest/main/LICENSE.md
.. |NASA-PDS/harvest_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/harvest/issues/new/choose
.. |NASA-PDS/registry-mgr_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/registry-mgr/
.. |NASA-PDS/registry-mgr_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: None
.. |NASA-PDS/registry-mgr_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/registry-mgr_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/registry-mgr/releases/tag/v4.3.0
.. |NASA-PDS/registry-mgr_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/registry-mgr/main/LICENSE.md
.. |NASA-PDS/registry-mgr_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/registry-mgr/issues/new/choose
.. |NASA-PDS/transform_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/transform/
.. |NASA-PDS/transform_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://github.com/NASA-PDS/transform/blob/main/CHANGELOG.md#v1111-2019-12-13
.. |NASA-PDS/transform_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/transform_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/transform/releases/tag/v1.11.1
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
   :target: https://github.com/NASA-PDS/pds4-jparser/releases/tag/v2.1.1
.. |NASA-PDS/pds4-jparser_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/pds4-jparser/main/LICENSE.md
.. |NASA-PDS/pds4-jparser_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/pds4-jparser/issues/new/choose
.. |NASA-PDS/mi-label_manual| image:: https://nasa-pds.github.io/pdsen-corral/images/manual.png
   :target: https://NASA-PDS.github.io/mi-label/
.. |NASA-PDS/mi-label_changelog| image:: https://nasa-pds.github.io/pdsen-corral/images/changelog.png
   :target: https://www.gnupg.org/gph/en/manual/r1943.html
.. |NASA-PDS/mi-label_requirements| image:: https://nasa-pds.github.io/pdsen-corral/images/requirements.png
   :target: None
.. |NASA-PDS/mi-label_download| image:: https://nasa-pds.github.io/pdsen-corral/images/download.png
   :target: https://github.com/NASA-PDS/mi-label/releases/tag/None
.. |NASA-PDS/mi-label_license| image:: https://nasa-pds.github.io/pdsen-corral/images/license.png
   :target: https://raw.githubusercontent.com/NASA-PDS/mi-label/main/LICENSE.md
.. |NASA-PDS/mi-label_feedback| image:: https://nasa-pds.github.io/pdsen-corral/images/feedback.png
   :target: https://github.com/NASA-PDS/mi-label/issues/new/choose
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
