LDD Regression Testing
=======================

..  toctree::
    :maxdepth: 3

    /development/ldd-test

Overview
++++++++

Local Data Dictionary (LDD) stewards are expected to provide example labels that can be used for regression testing LDDs delivered for release. The number and complexity of examples developed are dependent upon the dictionary steward and what is determined to be a high-priority or is thought to be something that are critical to the dictionary. The following page describes some examples of regression tests as well as where/how these files should be provided to PDS Engineering Node to complete that testing.


Regression Test Data
++++++++++++++++++++++++++++++

Regression tests should be made up of PDS4 example products that either successfully or unsuccessfully validate using the `PDS Validate Tool <https://nasa-pds.github.io/validate/>`_.

For simple examples of generating simple regression test cases, see the `LDD Template repository <https://github.com/pds-data-dictionaries/ldd-template>`_.


Regression Test Data Rules
++++++++++++++++++++++++++

In order for your regression test data to be autonomously tested during the automated LDD Generation process, you must follow the following rules when posting your test data to Github:

1. **No schematrons** - do not include schematron references in the labels. the pipeline will automatically add the newly generated schematrons to the validation.
2. **No schemaLocations** - do not include schemaLocation references in the labels. the pipeline will automatically add the newly generated schematrons to the validation.
3. **Include ``[IM_VERSION]`` for information_model_version** - use ``[IM_VERSION]`` value for ``information_model_version`` attribute so it can be dynamically replaced by the pipeline


Test Data Directory Layout
++++++++++++++++++++++++++++++

Regression test products should be maintained within the ``test/`` directory of your LDD Repo::

    ldd-test/
    ├── ...
    ├── test
    │   ├── No.Data
    │   ├── test1_FAIL.xml
    │   └── test1_VALID.xml

where:

* ``PDS4_SP_1100_1000_test`` - this top level directory should be named using the format ``PDS4_<namespace_id>_<IM_version>_<LDD_version>_test``
* ``*FAIL*`` - all PDS4 XML labels that will fail validation against delivered dictionaries. Output from Validate Tool should go into ``*FAIL*.log`` files in order to compare output from EN Validate execution.
* ``*VALID*`` - all PDS4 XML labels that will complete successful validation against delivered dictionaries.

