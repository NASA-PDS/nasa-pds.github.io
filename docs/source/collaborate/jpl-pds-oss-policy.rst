JPL-PDS Open Source Software Policy
===================================

..  toctree::
    :maxdepth: 3

    /collaborate/jpl-pds-oss-policy

--------------

Background
++++++++++
The following *Open Source Software Policy* has been approved as part of the JPL-PDS Node 2022-2027 Task Plan.

Applicability
+++++++++++++
This policy is applicable to the JPL-PDS Nodes:

* Engineering Node (EN)
* Navigational & Ancillary Information Facility (NAIF)
* Cartography and Imaging Sciences Sub-Node at JPL (IMG)

Open Source Software Policy
++++++++++++++++++++++++++++
Software funded and developed as part of the Jet Propulsion Laboratory’s Planetary Data System (PDS) Project shall be developed in the open from project initiation and made available to the public as Open Source Software (OSS). The OSS should be distributed under the Apache License, Version 2.0, or some other equivalent open license that is consistent with the definition of “Open Source” provided by the Open Source Initiative (https://opensource.org/osd) or meet the definition of “Free Software” provided by the Free Software Foundation (https://www.gnu.org/philosophy/free-sw.html). All OSS projects should be made publicly available and maintained in the NASA PDS GitHub (https://github.com/NASA-PDS) or an equivalent repository approved by the PDS Software Working Group. Each major release of the software must have a persistent identifier such as a Digital Object Identifier (DOI). The repository should include a code of conduct and a contributor’s guide for the project. For any activities covered in this Task Plan that are currently not open source, the applicable product owner shall develop an open source plan and timeline to complete transition to the NASA PDS GitHub/open source software framework.
 
Some software may be exempt from this policy for reasons such as export control, security, or proprietary concerns. Software that would be exempt from this policy should be identified as part of the Task Plan along with the justification for the exception along with any steps being taken to mitigate the exemption. Software developed later that may be exempt should be reviewed with program officer. All exemptions will be documented on the NASA-PDS Github website (https://nasa-pds.github.io/collaborate/jpl-pds-oss-policy.html#exemptions) and, at minimum, reviewed as part of next task plan renewal.
 
This policy is subject to change based upon future guidance from NASA Science Mission Directorate per open sourcing, archiving, and indexing of software.

This policy complies with the Open Source Policy at JPL, and has been approved by JPL’s Office of Technology Transfer and Software Release Authority.

Exemptions
++++++++++

Exemption from Apache 2.0 license or other license for the SPICE Toolkit.
---------------------------------------------------------------------
*Rationale:* The SPICE Toolkit source code is provided as open source via their website [1] with an open source license that limits redistribution [2]. The license was already agreed upon due to concerns over the security, backwards-compatibility, and quality of the software. This exemption will be reviewed at the next major release of the software.
 
Exemption from Open Development and GitHub requirement for the SPICE Toolkit.
-----------------------------------------------------------------------------
*Rationale:* The SPICE Toolkit source code is provided as open source via their website [1].  The previously agreed upon open source license [2] limits open development and redistribution, and it is cost prohibitive to migrate to an open development framework and GitHub. This exemption will be reviewed at the next major release of the software.

[1] https://naif.jpl.nasa.gov/naif/toolkit.html

[2] https://naif.jpl.nasa.gov/naif/rules.html
