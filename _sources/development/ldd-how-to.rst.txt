LDD How-To Guides
===================

..  toctree::
    :maxdepth: 3

    /development/ldd-how-to


Trigger LDD Build
+++++++++++++++++

For this example we will be using the `IMG Discipline LDD <https://github.com/pds-data-dictionaries/ldd-img>`_ repo. For your repo, just replace the `ldd-img` or references to `IMG` with your appropriate discipline dictionary.

1. `Create a new branch for your updates <https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/managing-branches>`_ (if you have not already created one).
2. Update your IngestLDD file (e.g. PDS4_IMG_IngestLDD.xml).
3. `Commit your changes <https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/committing-and-reviewing-changes-to-your-project>`_.
4. `Push your branch to Github <https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/pushing-changes-to-github>`_
5. Watch the magic happen on your Github Actions page: https://github.com/pds-data-dictionaries/ldd-img/actions
6. After the action has completed successfully (hopefully), `update your local branch <https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/syncing-your-branch>`_ to get the generated dictionaries from Github.com


Generate a Discipline LDD
+++++++++++++++++++++++++

To generate a Discipline LDD versus a Mission LDD, you must specify this information within the IngestLDD, for example::

        <name>Imaging Discipline Dictionary</name>
        <ldd_version_id>1.0.0.0</ldd_version_id>
        <dictionary_type>Discipline</dictionary_type>

See the `Imaging Discipline LDD <https://github.com/pds-data-dictionaries/ldd-img/blob/master/src/PDS4_IMG_IngestLDD.xml>`_ for a more detailed example.

Then execute LDDTool to generate the appropriate dictionary::

    lddtool -lp <my_ingest_ldd>


Generate a Mission LDD
++++++++++++++++++++++

To generate a Mission LDD versus a Discipline LDD, you must specify this information within the IngestLDD, for example::

        <name>Mars 2020 Mission</name>
        <ldd_version_id>1.0.0.0</ldd_version_id>
        <dictionary_type>Mission</dictionary_type>

See the `Mars 2020 Mission LDD <https://github.com/pds-data-dictionaries/ldd-m2020/blob/master/src/PDS4_M2020_IngestLDD.xml>`_ for a more detailed example.

Then execute LDDTool to generate the appropriate dictionary::

    lddtool -lp <my_ingest_ldd>


Generate a LDD with a specific PDS4 Version
+++++++++++++++++++++++++++++++++++++++++++

LDDTool is a reflection of the PDS4 Information Model (IM), and in turn, has a major build in sync with the `PDS4 Build Schedule <https://pds.nasa.gov/datastandards/about/>`_ (every 6 months).

By default, LDDTool builds with the latest version of the IM. As of LDDTool v12.0.0, it can now generate LDDs for older versions of the IM using the -V flag::

      -V, --IM Version - E.g., -V 1D00


Specify Enumerated Values for Attributes within Inherited Classes
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Classes from the PDS common dictionary (or discipline LDDs) are often inherited and used within Discipline and Mission LDDs (e.g. ``Internal_Reference.reference_type``, etc.). When inherited within the specific Discipline or Mission, you may want to provide a specific set of values applicable for that particular context. In this case you would want to use the `DD_Associate_External_Class <https://pds.nasa.gov/datastandards/documents/im/current/index_1E00.html#18.9%C2%A0%C2%A0class_pds_dd_associate_external_class>`_. For example:::

    <DD_Associate_External_Class>
      <namespace_id>pds</namespace_id>
      <class_name>Local_Internal_Reference</class_name>
      <minimum_occurrences>0</minimum_occurrences>
      <maximum_occurrences>1</maximum_occurrences>
      <DD_Context_Value_List>
         <attribute_name>local_reference_type</attribute_name>
         <attribute_relative_xpath>local_reference_type</attribute_relative_xpath>
         <DD_Permissible_Value>
             <value>spectral_characteristics_to_array_object</value>
             <value_meaning>
               The spectral parameters describe the array associated
               with the given 'local_identifier'.
             </value_meaning>
         </DD_Permissible_Value>
         <DD_Permissible_Value>
             <value>spectral_characteristics_to_table_object</value>
             <value_meaning>
               The spectral parameters describe the table or specific
               fields in the table associated with the given 
               'local_identifier'.
             </value_meaning>
         </DD_Permissible_Value>
      </DD_Context_Value_List>
    </DD_Associate_External_Class>


Schematron (DD_Rule) Help
+++++++++++++++++++++++++

Specify Enumerated Values for Inherited Attributes 
--------------------------------------------------

Attributes from the PDS common dictionary (or discipline LDDs) are often inherited and used within Discipline and Mission LDDs (e.g. ``pds:name``, etc.). When inherited within the specific Discipline or Mission, you may want to provide a specific set of values applicable for that particular context. In this case you will need to specify a DD_Rule to provide the enumerated value list. For example:::

    <DD_Rule>
        <local_identifier>color_filter_array_state_check</local_identifier>
        <rule_context>//img:Color_Filter_Array</rule_context>
        <DD_Rule_Statement>
          <rule_type>Assert</rule_type>
          <rule_test>img:color_filter_array_state = ('Encoded', 'Decoded', 'No CFA')</rule_test>
          <rule_message>IMG:error:img:color_filter_array_state_check: img:color_filter_array_state must be equal to one of the following values: 
            'Encoded', 'Decoded', 'No CFA'.
          </rule_message>
        </DD_Rule_Statement>
    </DD_Rule>


Using Schematron ``value-of`` functionality
++++++++++++++++++++++++++++++++++++++++++++

To use the ``sch:value-of`` in your ``DD_Rule`` descriptions, you simply need to escape the XML entities. For example::

    <sch:rule context="msn:mission_phase_name">
        <sch:let name="num_colons" value="string-length(.) - string-length(translate(., ':', ''))"/>
        <sch:let name="required_colons" value="4"/>
        <sch:assert test="$num_colons eq $required_colons">
            In Product_Collection, the number of colons found:
            (&lt;sch:value-of select="$num_colons"/&gt;)
            is inconsistent with the number expected:
            (&lt;sch:value-of select="$required_colons"/&gt;).
        </sch:assert>
        </sch:rule>
    </sch:pattern>

Note the ``&lt;``` and ``&gt;`` used to replace the ``<`` and ``>``


Mission LDD Namespace Formation Guidelines
++++++++++++++++++++++++++++++++++++++++++++

.. note::
    The determination of LDD namespaces is ultimately up to the discussion amongst the Mission Data Archive Working Group (DAWG). This is simply a guide to enable consistency wherever possible.

For **mission namespaces**, use the *mission acronym or shortened name*. For example:

* bc for BepiColombo
* m2020 for Mars2020
* insight for InSight
* orex for OSIRIS-REx

for **instrument-specific namespaces**, use the formation rule *mission_host_instrument*. For example:

* bc_mtm_mcam for the MCAM instrument on the Mercury Transfer Module (MTM) instrument host of the BepiColombo mission



TBD
+++
Feel free to add some of your own or create a ticket in the `PDS4 LDD Issue Repo <https://github.com/pds-data-dictionaries/PDS4-LDD-Issue-Repo/issues>`_ so we can start to build up this documentation.