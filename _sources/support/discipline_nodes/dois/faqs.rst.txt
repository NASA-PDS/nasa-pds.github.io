FAQs
++++

This section includes FAQs for creating and updating DOIs for PDS3 data sets; and for PDS4 Bundles, Collections, and Document Products. If you require additional support, please contact the `PDS Operator <mailto:pds-operator@jpl.nasa.gov>`__ for assistance.

..  toctree::

    /support/discipline_nodes/dois/faqs

----


How do I know whether I should reserve or release a DOI?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The short answer:

* If the data is not yet publicly available -> Reserve
* If the data is publicly available -> Release

The longer answer:

* To “reserve” a DOI, is to acquire a DOI from our DOI Provider associated for the future release of a PDS3 data set; or a PDS4 Bundle, Collection, or Document Product. This is the ideal start for acquiring DOIs so the DOI metadata is available and can be included in the Product label metadata prior to release.  

Notes:
   (1) The "reserved" DOI metadata is temporary / transitory and will be "overwritten" once the DOI is "released".  
   (2) A DOI is not "searchable" until the DOI is "released".

* To “release” a DOI is to make the ``https://doi.org/<my_doi>`` URL active / live (which means the DOI becomes "searchable". This requires that the data is registered at EN, available online, and the landing pages are also active / live (automated by EN Registry).

How can I specify multiple authors in the DOI reserve spreadsheet?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Currently, only 1 author can be specified / referenced in the XLS spreadsheet. The most signficiant metadata in in the XLS spreadsheet is the **LIDVID** (i.e., The LIDVID is what ties the DOI to the registered Product. Multiple authors may be specified / referenced when the DOI as part of the "release" process.

The DOI reserve spreadsheet seems very terse, can I provide more information?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The “Reserve DOI” step is really just a placeholder to request a DOI from our DOI Provider. The only information that is really critical at this step is the LIDVID. Everything else will be modified / updated when you submit a request to “release” the DOI.

What PDS4 products should we be assigning DOIs to?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Per the PDS DOI Policy, PDS4 Bundles are the “default” product to receive a DOI, but it is up to the Discipline Node if you would like DOIs additionally for PDS3 data sets or PDS4 Collections or Document Products.

What does it mean to have data registered?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In order for the DOI to be "registered", there must be a corresponding DOI Landing Page. The DOI Landing Page is generated when the Products are registered with PDS Engineering Node.

How do I register my PDS4 product with Engineering Node?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Contact the `PDS Operator <mailto:pds-operator@jpl.nasa.gov>`__ with the URL(s) to the applicable PDS4 product(s) you would like registered.

How do I get a DOIs for PDS3 data sets and documents?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The PDS has gone through the exercise with each Discipline Node to mint DOIs for most PDS3 Data Sets. If we missed one or there is a newer version available, please complete the following:

Send an email with the DS.CAT for all applicable PDS3 Data Sets to `PDS Operator <mailto:pds-operator@jpl.nasa.gov>`_ and `Ron
Joyner <mailto:ronald.joyner@jpl.nasa.gov>`_ with subject ``Release DOI for PDS3 Data Set: some identifying info``. 
Be sure to indicate whether:
  (1) The data set is new to the system; no DOI exists; but the data set has been "registered" with the PDS Engineering Node
  (2) The DS.cat been updated, the data set has already been registered at PDS Engineering Node, and the DOI for the data set is: ``<doi>10.17189/xxxxxx</doi>``
