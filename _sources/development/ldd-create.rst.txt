LDD Creation Process
====================

..  toctree::
    :maxdepth: 3

    /development/ldd-create

Proposing a New Discipline LDD
++++++++++++++++++++++++++++++

Creation of a new Discipline LDDs should be discussed and approved by the PDS LDD Change Control Board (TBD Email list or google group). During this process the following must be determined:

1. Is this LDD needed?
----------------------

Does a similar dictionary exist? If so, what is the rationale for creating a new one instead of adding to an existing one?

2. Who will be the LDD Steward(s)?
----------------------------------

One or more discipline node staff members must be appointed steward of the LDD.

3. Who will be on the LDD Change Control Board?
-----------------------------------------------

If this LDD is of interest to your Discipline Node, request of the newly appointed LDD Steward(s) to be added to the CCB.

----

Proposing a New Mission LDD
+++++++++++++++++++++++++++

Contact your Discipline Node to help you along this process. Many of the best practices and review rigor described below may not be necessary for Mission LDD development.

----

Requesting A New Namespace ID
+++++++++++++++++++++++++++++

Upon receiving approval to begin development on your new LDD, a namespace ID must be reserved.

Create a new "PDS Namespace Request" issue within the `PDS4 Information Model repo <https://github.com/NASA-PDS/pds4-information-model/issues/new/choose>`_ to get your namespace added to the `PDS4 Namespace Registry <https://pds.nasa.gov/datastandards/schema/pds-namespace-registry.pdf>`_.

----

Kick-off Team and Repo Creation
+++++++++++++++++++++++++++++++

Contact the `PDS Team <https://github.com/orgs/pds-data-dictionaries/teams/pds-dictionary-steward-admins/members>`_ to assist you with creating the appropriate Github Teams and LDD Repository as laid out below. These actions all require Github Admin access. Please provide them with the following information:

* namespace_id
* Brief description of the LDD. spell out namespace_id if it is an acronym.
* LDD Steward Github username

----

Creating New LDD Repository (Admin Only)
++++++++++++++++++++++++++++++++++++++++

Once you have your `Namespace ID <#Requesting-A-New-Namespace-ID>`_, you are ready to create the new Github repo for maintaining the LDD.

.. note::
    Responsible Party: Member of `PDS Dictionary Stewards Admin Team <https://github.com/orgs/pds-data-dictionaries/teams/pds-dictionary-steward-admins/members>`_

.. note::
    This can probably be scripted someday using GithubAPI or within a Github Action.


1. Create new repo from ldd-template
------------------------------------

a. `Create new repo <https://github.com/pds-data-dictionaries/ldd-template/generate>`_

b. Set the following parameters:
    * ``Owner``: ``pds-data-dictionaries``
    * ``Repository Name``: should follow the naming scheme ``ldd-<namespace_id>``.
    * ``Description``: enter description sent by LDD Steward
    * Set visibility to ``Public``
    * Check the box ``Include all branches``


2. Update Repo Settings
-----------------------

We need to setup the teams and ``master`` branch protections.

a. Go to ``Settings``

b. Disable issues being created on this repo (they will be created in the PDS4 LDD Issue Repo).

c. Add appropriate teams with access to repo
    * Go to ``Manage Access``
    * Click on ``Invite teams or people``
    * Add the LDD Steward with Admin access
    * Add the LDD CCB Team with Write access

d. Set branches protections
    * Go to ``Branches``
    * Under **Branch protection rules**, click ``Add rule``
    * Enter **Branch name pattern:** ``master``
    * Select ``Require pull request reviews before merging``
    * Select ``Require review from Code Owners``
    * Select ``Restrict who can push to matching branches``


3. Create new issue template in PDS4 LDD Issue Repo
----------------------------------------------------

a. `Create a new label <https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/labels>`_ in the PDS4 LDD Issue Repo for the new repo (ldd-<namespace_id>)

b. Clone the `PDS4 LDD Issue Repo <https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/>`_

c. Execute the `generate-issue-template.sh bash script <https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/blob/master/bin/generate-issue-template.sh>`_. This will automatically generate an issue template from the `LDD Issue Template <https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/blob/master/templates/ldd-issue-template.md>`_ and push to the repo::

        $ bin/generate-issue-template.sh cart Cartography thareUSGS
        New issue template created: /Users/jpadams/Documents/proj/pds/pdsen/workspace/pds4-ldd-issue-repo/bin/../.github/ISSUE_TEMPLATE/-ldd-cart--ldd-update-request.md
        [master 950bedb] Add cart issue template
         1 file changed, 33 insertions(+)
         create mode 100644 .github/ISSUE_TEMPLATE/-ldd-cart--ldd-update-request.md
        Enumerating objects: 8, done.
        Counting objects: 100% (8/8), done.
        Delta compression using up to 16 threads
        Compressing objects: 100% (4/4), done.
        Writing objects: 100% (5/5), 1.07 KiB | 1.07 MiB/s, done.
        Total 5 (delta 2), reused 0 (delta 0)
        remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
        remote: This repository moved. Please use the new location:
        remote:   git@github.com:pds-data-dictionaries/PDS4-LDD-Issue-Repo.git
        To github.com:pds-data-dictionaries/pds4-ldd-issue-repo.git
           b0abee5..950bedb  master -> master

d. You should now see a `new issue template created <https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/issues/new/choose>`_


4. Notify LDD Steward
---------------------

Notify the LDD Steward the new repo is ready.


----

Retrofit Existing LDD Repository (Admin / Stewards Only)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++

1. Clone the ldd-template repo and the LDD repo to be retrofitted. For this example, we will be retrofitting the ``ldd-img`` repo::

    git clone git@github.com:pds-data-dictionaries/ldd-template.git
    git clone git@github.com:pds-data-dictionaries/ldd-img.git

2. From the ``ldd-img`` repo, rsync the various files from the ``ldd-template`` repo::

    cd ldd-img
    rsync -av ../ldd-template/.gitignore ../ldd-template/.github ../ldd-template/build ../ldd-template/src ../ldd-template/test ./

3. Rename or remove test files and example IngestLDD so they don't get picked up in the regression tests (files can't end in .xml)::

    mv test/test1_FAIL.xml test/test1_FAIL.xml_example
    mv test/test1_VALID.xml test/test1_VALID.xml_example
    rm src/PDS4_EXAMPLE_IngestLDD.xml

4. Re-arrange directories to match that of the ``ldd-template`` repo. Specifically note the ``build/development`` and ``build/release`` directories.

5. Create a branch and pull request, and verify the Github Action executes successfully. e.g. https://github.com/pds-data-dictionaries/ldd-img/actions/

6. Remove local repo github issues, update permissions on the repository, and add branch protections per :doc:`Update Repo Settings above <ldd-create#update-repo-settings>`

7. Update README as appropriate to direct people to Contribute and Get Support. See the `ldd-template README <https://github.com/pds-data-dictionaries/ldd-template/blob/master/README.md>`_ for more details.
