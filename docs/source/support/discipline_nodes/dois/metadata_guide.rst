DOI Metadata Guidelines
=======================

..  note::
    This page is under constructions. Contributions, comments, and improvements welcome
    in our `Github Issues <https://github.com/NASA-PDS/nasa-pds.github.io/issues>`_

..  toctree::

    /support/discipline_nodes/dois/metadata_guide


*ROOT*

This is the root of the submission file document, and thus required.

Note that the content of the *<resource>* element is defined under an
*xs:all* group, so that the immediate child nodes can appear in any
order. The order here reflects the order in which they are listed in the
schema.

.. _section_1:

*REQUIRED*

This is the assigned DOI identifier and must begin with the DataCite
prefix "10."

   Required attribute: *identifierType*. This *must* have a value of
   **DOI**. For example:

::

        <identifier identifierType="DOI">10.12345/abcde</identifier>

.. _section_2:

*REQUIRED*

This is the author list or equivalent. Creators should appear in
priority order. Both individuals and institutions/organizations can be
credited as creators.

+----------------------------------------------------------------------+
| If the only list we have is a list of editors, then it goes here,    |
| but also indicate in the *<contributors>* section that each person   |
| in the list is a *contributor* with the role of **Editor**. This is  |
| not an optimal solution, but it will do for now.                     |
+----------------------------------------------------------------------+

.. _section_3:

*REQUIRED, repeatable*

This class contains the identifying information for one creator. It is
repeated for each creator. Note that the metadata schema does not
distinguish between "authors" and "editors". If some of the creators
listed are editors rather than authors, repeat their creator information
in the *<contributors>* section and indicate a role of "Editor".

+----------------------------------------------------------------------+
| Fill out as much of this class as possible with information that was |
| apropos at the time of the publication. So, if you know given name,  |
| include it; if you know the institutional affiliation, include it;   |
| if you can find and confirm the correct ORCID, include it; etc. This |
| all helps in linking the data set into the literature and the        |
| author's network.                                                    |
+----------------------------------------------------------------------+

.. _section_4:

*REQUIRED*

The string representing the name as it should appear in citations. For
personal names, the format is "*Family*, *Given*" (all one string). Full
first names are preferred for the metadata, in order to help identify
authors unambiguously. (It is also relatively easy to turn a complete
name into an initial.) For organizational names, use the full, formal
name of the organization.

This tag has one optional XML attribute, *nameType*, which takes one of
these values:

      **Organizational**
      **Personal**

Best practice is to always include this attribute for *creatorName*.

.. _section_5:

*OPTIONAL*

For personal names, this should contain the string corresponding to the
given name in the *<creatorName>* element. This should not be present
for organizational names (but that is not enforced by the DataCite
schema).

.. _section_6:

*OPTIONAL*

For personal names, this should contain the string corresponding to the
family name (surname, patronymic, etc.). This should not be present for
organizational names (but that is not enforced by the DataCite schema).

+----------------------------------------------------------------------+
| **Note:** For PDS purposes, at least, we should consider where to    |
| associate suffixes (Jr., Sr., III, etc.). If DataCite, ADS, or the   |
| AAS journals have a convention, we should follow that.               |
+----------------------------------------------------------------------+

.. _section_7:

*OPTIONAL, repeatable*

This attribute provides a formal identifier for an individual or
organization - for example, an author's ORCID, or an organizational DOI.
Only public identifiers should appear here, of course. If there is more
than one applicable identifier, this element may be repeated.

   Required attribute: *nameIdentifierScheme*. The value should be the
   common name or acronym for the identifier given (like "ORCID").
   Optional attribute: *schemeURI*. The value should be the URI of the
   defining organization or schema ("http://orcid.org", e.g.).

Where it can be obtained directly from the creator, or where we can be
certain about a creator's ORCID, we should add it to the metadata.

.. _section_8:

*OPTIONAL, repeatable*

This attribute provides an organizational affiliation (as free-format
text) for the creator. It may be repeated. Organizational "creators" may
also have affiliations, if that makes sense.

   Optional attribute: *affiliationIdentifier*. The value should be a
   formal, permanent, unique identifier for the affiliated organization,
   beyond the name that is the value of the *<affiliation>* element. For
   example, a Research Organization Registry (ROR) ID would be ideal
   here.

   Optional attribute: *affiliationIdentifierScheme*. The
   (human-recognizable) name of the identifier system (e.g., "ROR" would
   be sufficient in the above case.

   Optional attribute: *schemeURI*. The URI of the identifier scheme,
   typically a URL.

.. _section_9:

*REQUIRED*

This class lists names or titles for the resource being identified. At
least one title *must* be provided. This is the title that will be used
to format citations, and it is also the title that users will see
returned by various search interfaces. It needs to make sense in a
general, non-PDS search context, so avoid acronyms and assuming that
users will know that, for example, "Deep Impact" is also the name of a
spacecraft and NASA mission.

+----------------------------------------------------------------------+
| Remember the primary title has to make sense in the context of an    |
| ADS-type search. Users may not know that data sets are included in   |
| their result set. The title we put here will be used to formulate    |
| citations of the data set as well as helping users to identify data  |
| of potential interest. So avoid acronyms (no matter how obvious they |
| seem now) unless they include the full name. For example, "DIF" is   |
| not good on its own, but "Deep Impact Flyby (DIF) Spacecraft" is     |
| very good - explicit and contains the acronym that knowledgeable     |
| users might search on as well.                                       |
+----------------------------------------------------------------------+

===

.. raw:: html

   <title>

===

*REQUIRED, repeatable*

This element contains a single title. It may be repeated for alternate
titles where appropriate.

   Optional attribute: *titleType*. This must have one of the following
   values:
   :\* AlternativeTitle

   :\* Subtitle

   :\* TranslatedTitle

   :\* Other

For PDS purposes, the formal title should *always* be listed first
without a *titleType* attribute, and additional titles should probably
always be either alternatives or translations and identified accordingly
through the *titleType* attribute.

   Optional attribute: *xml:lang*. This should contain one of the
   standard ISO 2- or 3-letter codes (but this is not validated). Note
   that this indicates only the language of the associated title string,
   *not* the language of the resource.

PDS documents are required to be in English, so we should have no use
for this. Our IPDA partners, however, might. In that sort of context, it
would be prudent to include the *xml:lang* attribute for all *<title>*
elements, not just the one identified as the *TranslatedTitle*.

.. _section_10:

*REQUIRED*

This attribute identifies the publisher/distributor/curator of the
resource. It is used in creating citations.

+----------------------------------------------------------------------+
| For PDS4 data sets that have LIDs that begin with *urn:nasa:pds*,    |
| this should always be **NASA Planetary Data System**. If we are      |
| assigning DOIs for other publishers (like ESA), we should first      |
| determine what their publisher title should be, *and* we should      |
| probably be using a DOI prefix that can be unique to that publishing |
| archive.                                                             |
|                                                                      |
| If we are assigning a DOI and also serving the data for a non-PDS    |
| publisher, then we should list our node and facility in the          |
| *<contributors>* section, with a role of *DataCurator*. (The first   |
| time this comes up we should think about this again, just in case.)  |
+----------------------------------------------------------------------+

   Optional attribute: *xml:lang*. This attribute is used to indicate
   the language (using the standard ISO codes) of the publisher name.
   Unless otherwise specified, this is assumed to be in English.

.. _section_11:

*REQUIRED*

The year the resource was made available to the public. This is used in
creating citations.

+----------------------------------------------------------------------+
| For PDS data sets, this **must** be the four-digit year in which the |
| data were publicly posted *in the format and version associated with |
| this DOI*. This may or may not be the same year as listed in the     |
| CITATION_DESC field for legacy data sets. When in doubt, assume the  |
| DATA_SET_RELEASE_DATE is correct unless you have documentation that  |
| proves it is not - and then use the date in that documentation and   |
| note the discrepancy and resolution in an additional *<description>* |
| field (following) with a *descriptionType* of **Other**.             |
|                                                                      |
| This date **must** agree with the **Available** date (see below)     |
| provided for ADS processing.                                         |
|                                                                      |
| There are other date fields in which significant dates can be        |
| indicated if needed or desired.                                      |
+----------------------------------------------------------------------+

.. _section_12:

*REQUIRED*

This element takes a free-format text description of the type of
resource associated with the DOI.

   Required attribute: *resourceTypeGeneral*. This must have one of the
   following values:

      {\| cellpadding="10"

\|- \| valign="top" \|

-  Audiovisual
-  **[New in Schema 4.4]** Book
-  **[New in Schema 4.4]** BookChapter
-  Collection
-  **[New in Schema 4.4]** ComputationalNotebook
-  **[New in Schema 4.4]** ConferencePaper
-  **[New in Schema 4.4]** ConferenceProceeding

\| valign="top" \|

-  DataPaper
-  Dataset
-  **[New in Schema 4.4]** Dissertation
-  Event
-  Image
-  InteractiveResource
-  **[New in Schema 4.4]** Journal

\| valign="top" \|

-  **[New in Schema 4.4]** JournalArticle
-  Model
-  **[New in Schema 4.4]** OutputmanagementPlan
-  **[New in Schema 4.4]** PeerReview
-  PhysicalObject
-  **[New in Schema 4.4]** Preprint
-  **[New in Schema 4.4]** Report

\| valign="top" \|

-  Service
-  Software
-  Sound
-  **[New in Schema 4.4]** Standard
-  Text
-  Workflow
-  Other

\|}

Best/recommended practice is to consider the *resourceTypeGeneral* as
the broader term which is then modified by the value string, so that a
classification can be formed by concatenating the two with '/'. So, for
example:

::

       <resourceType resourceTypeGeneral="Dataset">PDS4 Refereed Data Collection</resourceType>

would read as "Dataset/PDS4 Refereed Data Collection".

**[New in Schema 4.4]** The value "Text" is deprecated except as a last
resort before going with *Other*. Wherever possible, please use a more
specific reference to a type of textual publication (i.e.,
*JournalArticle* or *Dissertation*).

Here are the values to use for non-text SBN cases:

+----------------------+-----------------------+----------------------+
| DOI target           | * resourceTypeGeneral*| *resourceType*       |
|                      |  |                    |
+======================+=======================+======================+
| PDS3 archived data   | **Dataset**           | **PDS3 Refereed Data |
| set                  |                       | Set**                |
+----------------------+-----------------------+----------------------+
| PDS4 archived data   | **Dataset**           | **PDS4 Refereed Data |
| product              |                       | Product**            |
+----------------------+-----------------------+----------------------+
| PDS4 archived        | **Dataset**           | **PDS4 Refereed Data |
| collection product   |                       | Collection**         |
+----------------------+-----------------------+----------------------+
| PDS4 archived bundle | **Dataset**           | **PDS4 Refereed Data |
| product, collections |                       | Bundle**             |
| do not have DOIs     |                       |                      |
+----------------------+-----------------------+----------------------+
| PDS4 archived bundle | **Collection**        | **PDS4 Bundle**      |
| product, collections |                       |                      |
| have their own DOIs  |                       |                      |
+----------------------+-----------------------+----------------------+
| PDS3 safed data set  | **Dataset**           | **PDS3 Save-the-bits |
|                      |                       | Data Set**           |
+----------------------+-----------------------+----------------------+

In general, we should aim to be consistent with Dublin Core usage for
these terms, but decisions here will have consequences elsewhere in the
database. Consistency across PDS would be highly desirable here.

.. _section_13:

*OPTIONAL*

This element lists keyword-type classifications as are commonly
associated with journal articles.

.. _section_14:

*OPTIONAL*

This element provides a string that corresponds to a keyword or similar
classifier for the resource. It may be repeated as desired. Each
occurrence should contain only a single taxonomic-type entry, and the
taxonomy should be indicated via the optional attributes as far as
possible.

   Optional attribute: *subjectScheme*. This should be the name of the
   taxonomy or authority. There is no controlled value list.
   Optional attribute: *schemeURI*. This should be a reference to the
   taxonomy definition or reference site.
   Optional attribute: *valueURI*. If there is a URL, for example, for
   the definition of the specific term being used, include it here.
   Optional attribute: *xml:lang*. Use this attribute to provide the
   standard ISO abbreviation for the language of the term.
   **[4.4 addition]** Optional attribute: *classificationCode*. Use this
   to provide the code within a system that does not have individual
   **valueURI**\ s but does have an internal code for each concept. (SBN
   data sets should use the UAT which does have **valueURI**\ s, so this
   attribute should not be used.)

For PDS and SBN data sets, subject keywords should be from the *Unified
Astronomy Thesaurus*, which does provide **valueURIs**. Here's a sample
** referencing the UAT:

``<subject subjectScheme="UAT" schemeURI="http://astrothesaurus.org" valueURI="https://astrothesaurus.org/uat/280">Comets</subject>``

If you cannot find an appropriate value in the UAT, please let SBN know
and we'll suggest an update.

.. _section_15:

*OPTIONAL*

This element provides a means for identifying people and organizations,
other than the previously identified *<creator>*, who contributed to the
creation, management, curation, distribution, etc., of the resource
being described.

.. _section_16:

*OPTIONAL*

This element identifies a person or organization who made or makes some
contribution to the resource. There is a required attribute to define
the type of contribution. The element may be repeated as needed.

   Required attribute: *contributorType*. This must have one of the
   following values:

      {\| cellpadding="10"

\|- \| valign="top" \|

-  ContactPerson
-  DataCollector
-  DataCurator
-  DataManager
-  Distributor
-  Editor
-  HostingInstitution

\| valign="top" \|

-  Producer
-  ProjectLeader
-  ProjectManager
-  ProjectMember
-  RegistrationAgency
-  RegistrationAuthority
-  RelatedPerson

\| valign="top" \|

-  Researcher
-  ResearchGroup
-  RightsHolder
-  Sponsor
-  Supervisor
-  WorkPackageLeader
-  Other

\|}

   These are all defined in the appendix to the DataCite schema
   description document, but interpreting them into a PDS context should
   be done with care.

   Here are some suggestions:

   {\| class="wikitable" style="background-color:lime"

! *Contributor Role* !! *Use for* \|- \| **Data Collector** \|\| People
involved in collection or compiling the data object but not otherwise
involved in generating labels or archive support information, and are
not otherwise credited as authors or editors. \|- \| **Data Curator**
\|\| The PDS Node/Subnode where the primary copy of the data physically
reside. \|- \| **Editor** \|\| Someone who formatted or otherwise
altered the content of data product files or archive labels created by
someone else. \|- \| **Producer** \|\| Someone who is involved in
designing and creating the PDS4 archive labels and support files, who is
not otherwise credited. \|- \| colspan="2" \| Other contributor roles
may be used if appropriate, but generic roles should be avoided and no
role should be used gratuitously. Do not use the *ContactPerson*, or
*RelatedPerson* roles in particular, as these do not age well in an
archive and will not be maintained - at least not by me. \|}

.. _section_17:

*REQUIRED*

The name of a single person or organization contributing. As in the case
of *<creator>*, this should be in the format "*Family, Given*" for
personal names, and the formal name for organizations.

   Optional attribute: *nameType*. It must have one of these two values:
   :\* Personal

   :\* Organizational

Best practice is to use the optional attribute.

.. _section_18:

*OPTIONAL*

The given name of a personal name, analogous to the same field for
*<creatorName>*.

.. _section_19:

*OPTIONAL*

The surname or patronymic of a personal name, analogous to the same
field for *<creatorName>*.

.. _section_20:

*OPTIONAL*

A formal identifier for a person or organization, such as a personal
ORCID or an organizational DOI. It may be repeated if there is more than
one applicable identifier.

   Required attribute: *nameIdentifierScheme*. This is the type of the
   identifier ("ORCID" or "DOI", e.g.).
   Optional attribute: *schemeURI*. This is a URI reference to the
   identifier definition or defining organization.

.. _section_21:

*OPTIONAL*

This element contains the name of an organization or institution with
which the named contributor is affiliated. It is a free-format text
field. It should be repeated for each unique affiliation when there is
more than one.

+----------------------------------------------------------------------+
| In the archiving case, this *must* be interpreted as "affiliation at |
| the time of publication of the product(s)" - in other words,         |
| affiliation on the date given for ''<publicationYear>.               |
+----------------------------------------------------------------------+

   Optional attribute: *affiliationIdentifier*. The value should be a
   formal, permanent, unique identifier for the affiliated organization,
   beyond the name that is the value of the *<affiliation>* element. For
   example, a Research Organization Registry (ROR) ID would be ideal
   here.

   Optional attribute: *affiliationIdentifierScheme*. The
   (human-recognizable) name of the identifier system (e.g., "ROR" would
   be sufficient in the above case.

   Optional attribute: *schemeURI*. The URI of the identifier scheme,
   typically a URL.

.. _section_22:

*OPTIONAL*

This element provides a way to include various significant dates in the
DOI database record.

.. _section_23:

*OPTIONAL*

One significant date for the resource. Dates should be in ISO 8601
format and can be to any precision (but this is not schematically
enforced). This element may be repeated as needed for each date.

   Required attribute: *dateType*. This indicates the significance of
   the date and must be one of the following values:

      {\| cellpadding="10"

\|- \| valign="top" \|

-  Accepted
-  Available
-  Collected
-  Copyrighted
-  Created
-  Issued

\| valign="top" \|

-  Other
-  Submitted
-  Updated
-  Valid
-  Withdrawn

\|}

   These are defined in the DOI Schema description document.

   Optional attribute: *dateInformation*. This should be a *very* brief
   clarification of the *dateType*, where necessary.

+----------------------------------------------------------------------+
| Wherever it is possible to do so, SBN must include an *<Available>*  |
| date that is the year and month of publication - so the year *must*  |
| agree with the previously listed *<publicationYear>* value. This     |
| date is the date ADS will use in generating statistics over various  |
| periods, so it is important that at least the month be present       |
| whenever it is known. As with *<publicationYear>*, the PDS3          |
| DATA_SET_RELEASE date should usually be considered authoritative.    |
+----------------------------------------------------------------------+

.. _section_24:

*OPTIONAL*

The natural language of the resource. This is defined as being of type
*xs:language*, which provides syntax validation but does not actually
fully enforce that values come from the "IETF BCP 47, ISO 639-1 language
code," as specified in the description.

+----------------------------------------------------------------------+
| For most purposes, "English" is assumed and there is no need to      |
| attempt to distinguish between American, Canadian, British, or any   |
| other sub-categories of modern English. If you're a completionist,   |
| though, feel free to include *<language>en</language>* in your DOI   |
| metadata.                                                            |
+----------------------------------------------------------------------+

.. _section_25:

*OPTIONAL*

This element lists alternate identifiers for the same instance of the
resource (as opposed to physically distinct, duplicate copies with their
own identifiers). The identifiers should be unique and controlled within
some context which should be specified.

In the DOI metadata context, PDS3 Data Set IDs and PDS4 LIDVIDs are
"alternate identifiers". Typically we would want the DSID or LIDVID to
be included in a citation, so we need to pay particular attention to
content here to make sure it is consistent and thus programmatically
retrievable. PDS4 LIDs without the version ID are not identifiers in the
context of DOIs, because the thing they point to is not permanently
fixed (a LID alone refers to the "latest available version", which may
change).

+--------------------------------------------------+------------------+
| For PDS Product:                                 | Use:             |
+==================================================+==================+
| PDS3 Product                                     | DSID:PRODUCT_ID  |
+--------------------------------------------------+------------------+
| PDS3 Data Set                                    | DATA_SET_ID      |
+--------------------------------------------------+------------------+
| PDS4 Product                                     | Product LIDVID   |
+--------------------------------------------------+------------------+
| PDS4 Collection                                  | Collection LDVID |
+--------------------------------------------------+------------------+
| PDS4 Bundle                                      | Bundle LIDVID\*  |
+--------------------------------------------------+------------------+
| \*Note that a Bundle that does not change its    |                  |
| own version ID every time a collection it        |                  |
| contains changes its version ID *should not have |                  |
| its own DOI*. The DOI needs to be associated     |                  |
| with an unchanging entity. If the bundle doesn't |                  |
| change when any of its collections changes, then |                  |
| it is *not* an "unchanging entity".              |                  |
+--------------------------------------------------+------------------+

.. _section_26:

*OPTIONAL*

This element provides one instance of an alternate identifier for the
resource. It may be repeated as desired.

   Required attribute: *alternateIdentifierType*. This string must
   describe the source or context of the identifier.

   {\| class="wikitable" style="background-color: lime"

! For PDS Identifier: !! Use *alternateIdentifierType*: \|- \| PDS3
DSID:PRODUCT_ID \|\| **PDS3 Product ID** \|- \| PDS3 DSID \|\| **PDS3
Dataset ID** \|- \| PDS4 Product LIDVID \|\| **PDS4 Product ID** \|- \|
PDS4 Collection LIDVID \|\| **PDS4 Collection ID** \|- \| PDS4 Bundle
LIDVID \|\| **PDS4 Bundle ID** \|}

.. _section_27:

*OPTIONAL*

This element lists identifiers for other resources related to this
resource in some specific way. **This is an important attribute to
include in our DOI metadata.** This is where we tie into the published
literature, so some effort should be put into getting this right. It's
also where we can related different versions of the same PDS product
(each of which will have its own DOI).

*Citation Considerations*

This is where we indicate which papers and other data sets are cited by
the data set getting the DOI. This is **not** a "reading list". When in
doubt, consider the data set/product as if it were being prepared for
publication in a refereed journal. If the citation would be appropriate
in that context, then it is likely appropriate in this one.

--------------

.. _citing_conventions:

Citing Conventions
^^^^^^^^^^^^^^^^^^

Here are some draft guidelines developed at SBN/UMD during a discussion
among the node personnel for where to look for citations to include in
DOI metadata as *relatedIdentifier*\ s of the type **Cites** or
**isCitedBy**:

   **Raw and Calibrated Data**

   -  *Cites* any inline citation in the text of the overview and/or
      intro document
   -  *Cites* any published papers describing the mission and/or
      relevant instrumentation referenced by the archive
   -  Calibrated data *Cites* raw data and calibration data; raw and
      calibration data *isCitedBy* calibrated data

   **High-level Data**

   -  *Cites* immediate precursor products (e.g., mosaic *Cites*
      calibrated images; resampled data *Cites* full-resolution data);
      precursor data *isCitedBy* high-level data
   -  *Cites* published paper describing the derivation/processing, if
      any.

   **Calibration Data**

   -  *Cites* mission and hardware papers, as appropriate.

--------------

*Other Relationships*

The next most important relationship to note here is that between older
and newer versions. Where both things have DOIs, the metadata should be
updated in both cases to provide bi-directional pointing. This can also
be used to indicate predecessors even when there are multiple
predecessors that were combined, or one that was split.

Other relationships should be documented if that makes sense both in the
context of the DOI metadata as well as the PDS archive. Some of the
likely ones to occur are listed following.

.. _section_28:

*OPTIONAL*

This element is a single related identifier. It can be repeated as
needed for additional identifiers. Note that it has half a dozen
attributes, only two of which are required, to help in defining the
relationship. Standard values are defined in the DataCite schema
documentation.

   Required attribute: *relatedIdentifierType*. The value must come from
   the following list:

      {\| cellpadding="10"

\|- \| valign="top" \|

-  ARK
-  arXiv
-  bibcode
-  DOI
-  EAN13
-  EISSN

\| valign="top" \|

-  Handle
-  IGSN
-  ISBN
-  ISSN
-  ISTC
-  LISSN

\| valign="top" \|

-  LSID
-  PMID
-  PURL
-  UPC
-  URL
-  URN
-  w3id

\|}

   Do not include more than one *<relatedIdentifier>* for the same
   publication/work to be cited or related.
   For general use, **DOI** is the preferred identifier for all
   relationship types. For citation, **bibcode** is acceptable, but
   should only be used if there is no DOI available. When both exist,
   ADS (who issue *bibcodes*) have specifically requested that we only
   use the DOI in this list to cite the other work. **ISBN** and
   **arXiv** might also be available and could be used in cases where
   this is no DOI.

   Required attribute: *relationType*. The value must come from the
   following list:

      {\| cellpadding="10"

\|- \| valign="top" \|

-  IsCitedBy
-  Cites
-  IsSupplementTo
-  IsSupplementedBy
-  IsContinuedBy
-  Continues
-  IsNewVersionOf
-  IsPreviousVersionOf
-  IsPartOf
-  HasPart
-  **[New in Schema 4.4]** IsPublishedIn

\| valign="top" \|

-  IsReferencedBy
-  References
-  IsDocumentedBy
-  Documents
-  IsCompiledBy
-  Compiles
-  IsVariantFormOf
-  IsOriginalFormOf
-  IsIdenticalTo
-  HasMetadata
-  IsMetadataFor

\| valign="top" \|

-  Reviews
-  IsReviewedBy
-  IsDerivedFrom
-  IsSourceOf
-  Describes
-  IsDescribedBy
-  HasVersion
-  IsVersionOf
-  Requires
-  IsRequiredby
-  Obsoletes
-  IsObsoletedBy

\|}

   Following is a summary of the relationships most likely to be useful
   in our context.

   {\| class="wikitable" style="background-color:lime"

! *relationType* !! Use for: \|- \| Cites/IsCitedBy \|\| Standard
citation of previous/subsequent work \|- \| IsVariantFormOf \|\| PDS4
versions of PDS3 data sets, where the PDS3 data set has a DOI and *no
substantive changes* (i.e., an external peer review was *not* required
for the PDS4 version) have been made in migrating the data from PDS3 to
PDS4. This should be included in the DOI metadata for both the PDS3 and
PDS4 versions. \|- \| IsNewVersionOf/IsPreviousVersionOf \|\| Datasets
that are new/previous versions (that is, same ID but different version
number) of datasets that also have DOIs; in this case both DOIs should
have their metadata updated. Also, if a PDS3-to-PDS4 migration *did*
require substantive changes to the data file, then this is the
appropriate relationship between the two. \|- \| Obsoletes/IsObsoletedBy
\|\| When a dataset supersedes a dataset with a *different* ID (in the
same ID system), use this relationship. \|- \| IsSupplementTo \|\| Data
that is the basis of or direct result of a journal article, but that was
*not* published as part of the article - especially where the data set
is mentioned in that publication \|- \| IsReferencedBy/References \|\|
Bibliographic references (as opposed to citations) \|- \|
IsDerivedFrom/IsSourceOf \|\| Raw-Calibrated relationships; high-order
products and the contributing source products \|- \| IsPartOf/HasPart
\|\| Bundles and their constituent collections when both have DOIs.
*IsPartOf* can also be used when a data product comprises one or more
tables that were published (in their entirety) as part of a journal
article or book. \|- \| colspan="2" \| Other relationships can and
should be used where they seem useful. \|}

   Optional attribute: *resourceTypeGeneral*. This attribute is
   identical to the one of the same name in
   *<*\ `resourceType <#.3CresourceType.3E>`__\ *>*, above.

   These optional attributes should only be used when the value of the
   *relationType* attribute is either **IsMetadataFor** or
   **HasMetadata** (this is not validated):

      Optional attribute: *relatedMetadataScheme*. This indicates the ID
      or name of a metadata definition standard.
      Optional attribute: *schemeURI*. This should be the URI of the
      named metadata standard.
      Optional attribute: *schemeType*. The DataCite definition is not
      clear, but this looks like a specific file format type for the
      referenced metadata standard (such as "XSD").

.. _new_in_schema_4.4:

**[New in Schema 4.4]** 
-----------------------

*OPTIONAL*

This element is used for two purposes:

1. To provide reference information for a traditional publication that
has no DOI; and 2. To provide additional information about the
publication context of a reference that does have a DOI (for example, to
document the book that contains a chapter in the citation list).

SBN will generally be using this element for the first purpose. Note
that *no verification* is done by DataCite for the publication
information in this class even when a DOI is present, so type carefully
and check it twice.

.. _section_29:

*OPTIONAL*

A single instance of "related item" information. Like
*<relatedIdentifier>*, this element has several attributes.

   Required Attribute: *relatedItemType*. This must have a value from
   the same list as the *resourceTypeGeneral* attribute of the
   `<resourceType> <#.3CresourceType.3E>`__ element above.

   Required Attribute: *relationType*. This must have a value from the
   same list as the *relationType* attribute of the
   `<relatedIdentifier> <#.3CrelatedIdentifier.3E>`__ element above.

.. _section_30:

*OPTIONAL*

If the related item has a digital identifier, it should be specified
here in the same manner as would be used for
`<relatedIdentifier> <#.3CrelatedIdentifier.3E>`__, above.

   Optional Attribute: *relatedItemIdentifierType*. This must have a
   value from the same list as
   `relatedIdentifier <#.3CrelatedIdentifier.3E>`__, above. Unlike
   *<relatedIdentifier>*, however, this attribute is optional.

   Optional Attributes: *relatedMetadataScheme*, *schemeURI*, and
   *schemeType*. These are used in the same circumstances and in the
   same way as for `<relatedIdentifier> <#.3CrelatedIdentifier.3E>`__,
   above. For SBN data sets, these are very unlikely to be relevant.

.. _section_31:

*OPTIONAL*

This is a grouping element for the creator list of the related item.

.. _section_32:

*OPTIONAL*

This element is similar to the *<creator>* element for the resource
itself, but does not allow specification of a *nameIdentifier* or
*affiliation*.

.. _section_33:

*REQUIRED*

As with the creators listed for the resource, the name should be given
in the format "*familyName, givenName*".

   Optional Attribute: *nameType*, which must be either
   **Organizational** or **Personal**.

   Optional Attribute: *xml:lang*, which can be used to indicate the
   language in which the name is expressed.

.. _section_34:

*OPTIONAL*

The given name of the creator.

.. _section_35:

*OPTIONAL*

The family name of the creator.

.. _section_36:

*OPTIONAL*

This container class is used to hold the title of the related item, and
any alternate titles for that item.

=====

.. raw:: html

   <title>

=====

*OPTIONAL*

This element holds the title of the related item, if it has one. It may
be repeated if that seems appropriate.

   Optional Attribute: *titleType*. If there is more than one title,
   then the secondary titles should have an associated *titleType* to
   explain their existence. The values come from the same list as used
   for the `title of the resource <#.3Ctitle.3E>`__, above.

Note there is **not** an enclosing *<titles>* class in this case.

.. _section_37:

*OPTIONAL*

If the related item has aassociated volume identifier (numeric or
otherwise), here's where it goes.

.. _section_38:

*OPTIONAL*

If the related item has an associated issue identifier (numeric or
otherwise), it goes here.

.. _section_39:

*OPTIONAL*

This element is for an associated sequence number, or similar (possibly
non-numeric) identifier.

   Optional Attribute: *numberType*. Use the attribute to indicate what
   kind of number (corresponding to common prefixes in reference list
   formats) the element contains. It must have one of these values:

      {\| cellpadding="10"

\|- \| valign="top" \|

-  Article
-  Chapter
-  Report
-  Other

\|}

.. _section_40:

*OPTIONAL*

This and the following element are for specifying a start and end page
for the item within the enclosing volume, issue, etc. If only one page
is known, assume it is the starting page and use *<firstPage>* without
*<lastPage>*.

.. _section_41:

*OPTIONAL*

This is for specifying the end of the page range of the related item
within its containing publication. If only one page is known, assume it
is the starting page and use *<firstPage>* without *<lastPage>*.

.. _section_42:

*OPTIONAL*

This element indicates the publisher of the related item, *not* the
resource receiving the DOI.

.. _section_43:

*OPTIONAL*

The year in which the related item was made publicly available. As with
the *<publicationYear>* of the resource, this must be in the range
[0..9999].

.. _section_44:

*OPTIONAL*

This element is used to provide an edition or version number for the
related item.

.. _section_45:

*OPTIONAL*

This is an enclosing element to hold a list of contributors to the
related item.

.. _section_46:

*OPTIONAL*

This element identifies a single contributor.

   Required Attribute: *contributorType*. This indicates the role the
   named *contributor* filled. This must come from the same
   controlled-value list as listed above for the
   `contributors <#.3Ccontributor.3E>`__ to the resource.

.. _section_47:

*REQUIRED*

As with the contributors listed for the resource, the name should be
given in the format "*familyName, givenName*".

   Optional Attribute: *nameType*, which must be either
   **Organizational** or **Personal**.

   Optional Attribute: *xml:lang*, which can be used to indicate the
   language in which the name is expressed.

.. _section_48:

*OPTIONAL*

The given name of the contributor.

.. _section_49:

*OPTIONAL*

The family name of the contributor.

.. _section_50:

*OPTIONAL*

This element provides unstructured size information. In other words, it
is not required to be numeric and there are no syntax constraints on the
content.

.. _section_51:

*OPTIONAL*

A single size specification string, like "18GB" or "Three volumes". This
element may be repeated as needed or desired.

+----------------------------------------------+
| Some Examples                                |
+==============================================+
| <size>55GB</size>                            |
+----------------------------------------------+
| <size>3250 tables<size>                      |
+----------------------------------------------+
| <size>235 FITS images<size>                  |
+----------------------------------------------+
| <size>24 documents in multiple formats<size> |
+----------------------------------------------+

.. _section_52:

*OPTIONAL*

This class indicates the physical/digital format(s) of the resource.

.. _section_53:

*OPTIONAL*

This element contains a text description of the format. It is not
constrained and may be repeated as appropriate.

Best practice is to use a file extension or MIME type string as the
value.

+----------------------------------------------------------------------+
| PDS should be more formal about the content here. We also need to    |
| think about possible mixed-format products, like single documents    |
| that comprise multiple files, some of which are text and some        |
| images/graphics, and the best way to describe *format* for           |
| collections (if at all).                                             |
+----------------------------------------------------------------------+

+--------------------------------------------+
| Some Examples                              |
+============================================+
| <format>text/plain</format>                |
+--------------------------------------------+
| <format>text/plain;charset=utf-8</format>  |
+--------------------------------------------+
| <format>text/csv</format>                  |
+--------------------------------------------+
| <format>text/tab-separated-values</format> |
+--------------------------------------------+
| <format>text/vnd.ascii-art</format>        |
+--------------------------------------------+
| <format>application/pdf</format>           |
+--------------------------------------------+
| <format>application/msword</format>        |
+--------------------------------------------+
| <format>text/xml</format>                  |
+--------------------------------------------+
| <format>image/fits</format>                |
+--------------------------------------------+
| <format>application/fits</format>          |
+--------------------------------------------+

Other media types (MIME types) may be found by referencing the list
provided by the Internet Assigned Number Authority (IANA) at
https://www.iana.org/assignments/media-types/media-types.xhtml. There is
no media type corresponding to PDS3 *.img* images, or plain raster
images (as far as I can tell).

.. _section_54:

*OPTIONAL*

A version number associated with the resource.

Best practice is to obtain a new DOI for a major version change of
something that already has a DOI.

+----------------------------------------------------------------------+
| Because of the traceability and reproducability concerns involved in |
| research data, PDS should never use this element for archival data.  |
| New versions of PDS products with DOIs should get their own DOIs.    |
| The *<*\ `relatedIdentifier <#.3CrelatedIdentifier.3E>`__\ *>*       |
| element can be used to link the two versions in the DOI database.    |
+----------------------------------------------------------------------+

.. _section_55:

*OPTIONAL*

This element typically contains only a single *<rights>* member to
indicate the rights management for the resource, although it may contain
multiple *<rights>* elements in complex cases.

.. _section_56:

*OPTIONAL*

A single rights license with management information (e.g., "Creative
Commons", or "GNU General Public License"). This should be as explicit
as possible, with a complete management statement where appropriate.
Embargo information should also be recorded here.

   Optional attribute: *rightsURI*. This should be the URI to the full
   text of the license.
   Optional attribute: *rightsIdentifier*. A short, standardized license
   name. Best practice is to use one of the identifiers on the SPDX
   list: https://spdx.org/licenses/
   Optional attribute: *rightsIdentifierScheme*. The name of the scheme
   for the identifier, immediately preceding. If the identifier same
   from the SPDX list, for example, then this attribute should have the
   value **SPDX**.
   Optional attribute: *schemeURI*. The URI corresponding to the
   definition of whatever is in *rightsIdentifierScheme*. In general,
   those two attributes should be used together.
   Optional attribute: *xml:lang*. This indicates the language of the
   license.

+----------------------------------------------------------------------+
| PDS data is in the public domain for some values of "public domain", |
| but this is not a well-defined term. Also, in order to be considered |
| FAIR, PDS data must have an explicit statement of license. "U.S.     |
| Government Work" might be correct, but this is typically applied to  |
| documents. Repeated requests to PDS and NASA for direction have gone |
| nowhere.                                                             |
+----------------------------------------------------------------------+

.. _section_57:

*OPTIONAL*

This element provides a place for additional information that does not
fit into other categories.

.. _section_58:

*OPTIONAL*

A single, free-format description of the specified (via attribute) type.
This field may be repeated as needed.

It looks like formatting is not preserved for this text, but you may use
the *<br/>* tag to insert a paragraph break.

Best practice is to provide at least one description of some type. It is
probably not a good idea to provide multiple *<description>* elements
with the same *descriptionType* value, but this is not validated.

   Required attribute: *descriptionType*. This indicates the category of
   information being provided. It must have one of these values:
   :\* Abstract

   :\* Methods

   :\* SeriesInformation

   :\* TableOfContents

   :\* TechnicalInfo

   :\* Other

+----------------------------------------------------------------------+
| All PDS DOIs *must* have at least one *<description>* field with a   |
| *descriptionType* of **Abstract**. Note that if you create a DOI     |
| through the *Fabrica* interface, the description you enter there is  |
| *not* tagged as an abstract. If other description types seem         |
| appropriate, add them.                                               |
+----------------------------------------------------------------------+

   Optional attribute: *xml:lang*. This indicates the language of the
   description being provided, not of the resource.

.. _section_59:

*OPTIONAL*

This element is used to define relationships (either on the creation or
application side) between the resource and a defined patch on the
surface of the Earth. I don't see a way to apply it as it currently
exists to celestial coordinates, and that might seriously confuse
applications that process this sort of metadata harvested from DOI
databases. It's included here for completeness.

.. _section_60:

*OPTIONAL*

This element defines one specific patch of Earth where the data were
taken or on which the resource is focused. It may be repeated as
desired.

.. _section_61:

*OPTIONAL*

A name for the location being defined.

Note that the text provided in the schema that describes the points
comprising the following elements as having values which are "a single
latitude-longitude pair, separated by whitespace". This is not true. In
all cases there are tags specifically defining latitude and longitude as
separate and distinct elements.

It is also possible to define any single *<geoLocation>* as being
simultaneously a single point, a single box, *and* any number of
polygons. This seems irrational, yet it appears to be deliberate.

.. _section_62:

*OPTIONAL*

This element specifies a single point on the globe.

.. _section_63:

*REQUIRED*

Longitude in degrees in the range +/- 180.

.. _section_64:

*REQUIRED*

Latitude in degrees in the range +/- 90.

.. _section_65:

*OPTIONAL*

A box is defined by its four sides - east and west longtude, and north
and south latitude.

.. _section_66:

*REQUIRED*

Westward bounding longitude in degrees in the range +/- 180.

.. _section_67:

*REQUIRED*

Eastward bounding longitude in degrees in the range +/- 180.

.. _section_68:

*REQUIRED*

Southward bounding latitude in degrees in the range +/- 90.

.. _section_69:

*REQUIRED*

Northward bounding latitude in degrees in the range +/- 90.

.. _section_70:

*OPTIONAL*

This element defines an arbitrary polygon as a sequence of points around
the perimeter in which the last point must have the same definition as
the first point (though this is not validated, nor is the nature of the
path). There must be at least 4 points provided.

Oddly, the schema allows this element to be repeated.

.. _section_71:

*REQUIRED*

Longitude and latitude of one point on the perimeter of the polygon.

.. _section_72:

*REQUIRED*

Longitude in degrees in the range +/- 180.

.. _section_73:

*REQUIRED*

Latitude in degrees in the range +/- 90.

.. _section_74:

*OPTIONAL*

If you are intending to define an area that is larger than half the
total surface of the Earth, then you *must* use this element to define a
point somewhere inside the area of interest. Otherwise the smaller
enclosed area is assumed to be the area of interest. The actual point
can be random, as long as it is inside the intended area.

.. _section_75:

*REQUIRED*

Longitude in degrees in the range +/- 180.

.. _section_76:

*REQUIRED*

Latitude in degrees in the range +/- 90.

.. _section_77:

*OPTIONAL*

This element identifies sources of funding related to creating or
maintaining the resource.

+----------------------------------------------------------------------+
| This is not information that PDS has traditionally collected, but as |
| it is used to trace results back to funding in the literature        |
| databases, we probably should. In the case of ROSES data preparers,  |
| I'd make that "definitely should".                                   |
+----------------------------------------------------------------------+

.. _section_78:

*OPTIONAL*

This element identifies a single source of funding. It may be repeated
as needed.

.. _section_79:

*REQUIRED*

Name of the funding source. This should be the formal name.

.. _section_80:

*OPTIONAL*

This is a string that uniquely identifies a funding source under some
public scheme, like "Crossref Funder" or ISNI.

   Required attribute: *funderIdentifierType*. This string is the source
   of the corresponding identifier. It must have one of these values:
   :\* ISNI

   :\* GRID

   :\* Crossref Funder ID

   :\* ROR

   :\* Other

   NASA's Crossref Funder ID is *10.13039/100000104*.

.. _section_81:

*OPTIONAL*

Grant number or similar code assigned by the funding organization.

   Optional attribute: *awardURI*. This attribute can be used to provide
   a link to a page at the funding organization website that describes
   the award/grant program.

.. _section_82:

*OPTIONAL*

The title on the grant/award - that is, the title of the proposal that
was submitted and funded.
