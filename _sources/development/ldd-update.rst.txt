LDD Update Process
===================

..  toctree::
    :maxdepth: 3

    /development/ldd-update


The following are the necessary steps to propose and execute an update to a PDS4 Local Data Dictionary.

..  image:: /_static/images/LDD-mgmt-process.png
    :target: ../_static/images/LDD-mgmt-process.png

1. Change Request Proposed
+++++++++++++++++++++++++++

The process is initiated when a user requests an update to an LDD via the `PDS4 Github Issues Repo <https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/issues/new/choose>`_.


2. LDD Steward Initial Approval
+++++++++++++++++++++++++++++++

The update request is received by the LDD Steward, who makes an initial determination of whether or not the change is warranted.

    a. If no, the issue is brought to the :doc:`LDD Change Control Board </teams/ldd-ccb>` for discussion. The outcome of that User Group discussion will determine whether or not to proceed.


3. Update IngestLDD
+++++++++++++++++++

Once the LDD Steward approves the change, they will get the latest version of the LDD from Github, and complete the necessary updates to the IngestLDD file (TBD link).

The LDD Steward can download and use `LDDTool  <https://nasa-pds.github.io/pds4-information-model/model-lddtool/index.html>`_ for testing purposes, but only the IngestLDD will be needed for submission to Github.


4. Push Updates To Github
+++++++++++++++++++++++++++

Once the LDD Steward has completed the necessary changes to the IngestLDD, a Pull Request (PR) (TBD link) is then created in the applicable LDD repository. When creating the Pull Request, sufficient documentation and details need to be provided in order to sufficiently describe the change and the rationale for LDD Change Control Board (link TBD) review.

Additionally, by generating a PR on the IngestLDD updates, the system will automatically run LDDTool to generate the schemas, schematrons, and other default LDDTool outputs. See the :doc:`LDD Update and Build Tutorial </support/tutorials>`


5. LDD Change Control Board Approval
+++++++++++++++++++++++++++++++++++++

The LDD Change Control Board will be notified their review is needed by two mechanisms:
a. They will be assigned as reviewers on the Github Pull Request
b. The LDD Steward will notify the group of the review start by emailing the CCB Google Group

Discussions about the changes should as much as possible be done within the Github Pull Request. See `Github Documentation <https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request>`_ for more details.

See the :doc:`LDD Change Control Board web page </teams/ldd-ccb>` for details on the voting and approval process.


6. Approve and Merge Changes
++++++++++++++++++++++++++++

Once the LDD CCB has approved changes, the PDS DD Steward can then Merge the Pull Request (link TBD).


7. (optional) Contact EN for Point Build
++++++++++++++++++++++++++++++++++++++++

For critical bug fixes that require the LDD to be built and released against the current or a past IM, create a new ticket for a Point Build Request (link TBD)

