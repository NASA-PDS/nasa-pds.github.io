==========================================
Release Description Document (Build B14.1)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B14.1`_

The following sections can be found in this document:

.. toctree::
   :glob: 
   :maxdepth: 3

   rdd.rst

PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

No PDS4 Standards Updates

Software Changes
================
For each software repository, the changes are listed in 2 categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B14.1`_).

The 'Other Updates' occurs during the build cycle without being planned or attached to a theme. They are organized by
types (bug, enhancements, requirements, tasks). Any updates that require a de-scope of planned tasks are reviewed by the
PDS Software Working Group.

The deliveries are validated by the development team and go through an additional Integration & Test process, as
applicable, as indicated by the ```Testing Status``` column in the tables below. There are 3 possible statuses for
testing:

- |:blue_circle:| Skip Testing - Testing is not needed for this ticket. These are determined at the discretion of the team based upon the technical or operational nature of the closed task.
- |:yellow_circle:| Testing Needed
- |:green_circle:| Testing Complete - Initial testing complete, and test cases/results documented.

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

+-------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================+====================+==========================+
|`deep-archive#151`_ Installation instructions don't work on Windows 11   ||:yellow_circle:|   |s.medium                  |
+-------------------------------------------------------------------------+--------------------+--------------------------+

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

+------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                   |I&T Status          |Priority / Bug Severity   |
+========================================================================+====================+==========================+
|`ds-view#14`_ Memory leak in Solr connections leading to Tomcat crash   ||:yellow_circle:|   |s.critical                |
+------------------------------------------------------------------------+--------------------+--------------------------+
|`ds-view#12`_ v2.14.2 does not work for resource links                  ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                     |I&T Status          |Priority / Bug Severity   |
+==========================================================================================+====================+==========================+
|`ds-view#8`_ Upgrade to latest Solr 9.3.x                                                 ||:blue_circle:|     |unknown                   |
+------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`ds-view#3`_ Upgrade Dataset View and dependencies to support Harvest/Registry upgrades   ||:yellow_circle:|   |p.must-have               |
+------------------------------------------------------------------------------------------+--------------------+--------------------------+

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
Bugs
++++

+-------------------------------------------------+--------------------+--------------------------+
|Issue                                            |I&T Status          |Priority / Bug Severity   |
+=================================================+====================+==========================+
|`registry-common#40`_ Fix code scanning alerts   ||:yellow_circle:|   |s.high                    |
+-------------------------------------------------+--------------------+--------------------------+

--------

Registry-harvest-legacy
-----------------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-harvest-legacy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-harvest-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-harvest-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-harvest-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-harvest-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-harvest-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                  |I&T Status          |Priority / Bug Severity   |
+=======================================================================================================+====================+==========================+
|`registry-harvest-legacy#8`_ As a user, I want to ingest Product_External products into the Registry   ||:yellow_circle:|   |p.must-have               |
+-------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Registry-mgr-legacy
-------------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-mgr-legacy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-mgr-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-mgr-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-mgr-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-mgr-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-mgr-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+---------------------------------------------------------+------------------+--------------------------+
|Issue                                                    |I&T Status        |Priority / Bug Severity   |
+=========================================================+==================+==========================+
|`registry-mgr-legacy#17`_ Upgrade to latest Solr 9.3.x   ||:blue_circle:|   |unknown                   |
+---------------------------------------------------------+------------------+--------------------------+

--------

Registry-pds3-catalog
---------------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-pds3-catalog#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-pds3-catalog>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-pds3-catalog/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-pds3-catalog/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-pds3-catalog/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-pds3-catalog/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                   |I&T Status          |Priority / Bug Severity   |
+========================================================================================================+====================+==========================+
|`registry-pds3-catalog#6`_ Upgrade to latest Solr 9.3.x                                                 ||:blue_circle:|     |unknown                   |
+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-pds3-catalog#4`_ Upgrade Catalog Tool and dependencies to support Harvest/Registry upgrades   ||:yellow_circle:|   |p.must-have               |
+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Search-ui-legacy
----------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/search-ui-legacy#readme>`_
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
Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                |I&T Status          |Priority / Bug Severity   |
+=====================================================================================================+====================+==========================+
|`search-ui-legacy#1`_ Upgrade Keyword Search and dependencies to support Harvest/Registry upgrades   ||:yellow_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Transform
---------
*Transforms PDS3 and PDS4 product labels and data into various formats.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/transform/>`_
     - `Github Repo <https://github.com/NASA-PDS/transform>`_
     - `Issue Tracking <https://github.com/NASA-PDS/transform/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/transform/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/transform/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/transform/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================================================+====================+==========================+
|`transform#30`_ [SECURITY] Upgrade to log4j-core/log4j-api                            ||:yellow_circle:|   |s.low                     |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|`transform#46`_ NoClassDefFoundError exception when transforming XML to PDS3 label    ||:yellow_circle:|   |s.medium                  |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|`transform#45`_ Broken download link and Windows JAVA settings in installation docs   ||:yellow_circle:|   |s.medium                  |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================+====================+==========================+
|`validate#475`_ Validate crashes on invalid # of records, and spurious file left behind    ||:yellow_circle:|   |p.wont-have               |
+-------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#681`_ Validate incorrectly throws precision mismatch error for Table_Delimited   ||:yellow_circle:|   |s.medium                  |
+-------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#723`_ Installation instructions need updates for Windows                         ||:yellow_circle:|   |unknown                   |
+-------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#698`_ Investigate and Fix code scanning alert for potential improvements         ||:blue_circle:|     |s.medium                  |
+-------------------------------------------------------------------------------------------+--------------------+--------------------------+

Liens
=====

+--------+--------+------------+
|Issue   |Title   |Rationale   |
+========+========+============+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B14.1)`_

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

.. _plan B14.1: https://nasa-pds.github.io/releases/14.1/plan.html
.. _deep-archive#151: https://github.com/NASA-PDS/deep-archive/issues/151
.. _ds-view#14: https://github.com/NASA-PDS/ds-view/issues/14
.. _ds-view#12: https://github.com/NASA-PDS/ds-view/issues/12
.. _ds-view#8: https://github.com/NASA-PDS/ds-view/issues/8
.. _ds-view#3: https://github.com/NASA-PDS/ds-view/issues/3
.. _registry-common#40: https://github.com/NASA-PDS/registry-common/issues/40
.. _registry-harvest-legacy#8: https://github.com/NASA-PDS/registry-harvest-legacy/issues/8
.. _registry-mgr-legacy#17: https://github.com/NASA-PDS/registry-mgr-legacy/issues/17
.. _registry-pds3-catalog#6: https://github.com/NASA-PDS/registry-pds3-catalog/issues/6
.. _registry-pds3-catalog#4: https://github.com/NASA-PDS/registry-pds3-catalog/issues/4
.. _search-ui-legacy#1: https://github.com/NASA-PDS/search-ui-legacy/issues/1
.. _transform#30: https://github.com/NASA-PDS/transform/issues/30
.. _transform#46: https://github.com/NASA-PDS/transform/issues/46
.. _transform#45: https://github.com/NASA-PDS/transform/issues/45
.. _validate#475: https://github.com/NASA-PDS/validate/issues/475
.. _validate#681: https://github.com/NASA-PDS/validate/issues/681
.. _validate#723: https://github.com/NASA-PDS/validate/issues/723
.. _validate#698: https://github.com/NASA-PDS/validate/issues/698
.. _Software Release Summary (B14.1): https://nasa-pds.github.io/releases/14.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
