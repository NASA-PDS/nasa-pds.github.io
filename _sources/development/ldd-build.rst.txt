LDD Build Process
=================

Operational Release
++++++++++++++++++++

By default, all Discipline LDDs will be built at the time of PDS4 IM Release. See the `PDS4 Build Schedule <https://pds.jpl.nasa.gov/datastandards/about/>`_ for more details on the timing of those builds.


Point Build Release
-------------------

Create a Point Build Request issue (link TBD) to request EN to trigger a point build of your LDD.

----

Development Release
+++++++++++++++++++

By default, as long as your Discipline LDD is using the ldd-template repository (TBD link), all Discipline LDD schemas, schematrons, and other default LDDTool outputs are generated whenever a Pull Request is created with a change to an IngestLDD.

The new schemas/schematrons are posted to the TBD directory in your repository. See :doc:`LDD Update and Build Tutorial </support/tutorials>` for an example generating these schemas/schematrons.


For more details on how the dictionaries are generated, see `LDD Github Actions`.


----

LDD Github Actions
+++++++++++++++++++

TBD