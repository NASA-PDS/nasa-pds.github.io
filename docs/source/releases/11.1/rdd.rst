=========================================
Release Description Document (build 11.1)
=========================================
validate
--------
bug
~~~

+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                                                     |Priority / Bug Severity   |
+==========================================================================================================================================================+==========================+
|validate_5_ Improve file base name check according to Standards Reference                                                                                 |s.low                     |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_6_ Improve pds4.bundle unlabeled files check to handle files without a file suffix                                                               |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_11_  Update allowable field_format values per Standards Reference definition regarding [+\-] characters                                          |s.low                     |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_153_ Update validate to throw error when a file has a space in the filename                                                                      |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_189_ Validate error reading tables > 2GiB                                                                                                        |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_240_ Unexpected error for data collection in a sub-directory                                                                                     |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_256_ validate should only do integrity checking on latest version of a collection when referenced by LID                                         |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_257_ Product with incorrect table binary definition pass validation                                                                              |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_260_ Missing documentation about deprecated flags                                                                                                |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_271_ validate 1.25.0-SNAPSHOT raises an exception when validating a product                                                                      |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_273_ Bug performing bundle validation with nested directories                                                                                    |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_278_ Registered context products file does not retain older versions of context products                                                         |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_281_ Validate fails to report error in   File.file_size                                                                                          |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_291_ When validating a product with a bad schematron definition, bundle validation also fails indicating the associated product does not exist   |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_294_ Content validation incorrectly reports error for floating-point values out of specified min/max range                                       |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_297_ Content validation of ASCII_Integer field does not accept value with leading zeroes                                                         |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_298_ validate misses double quotes within a delimited table                                                                                      |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_299_ Validate tool does not PASS a bundle with a single-character filename                                                                       |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_300_ validate -u flag reports an error on Windows                                                                                                |unk                       |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_301_ unclear error message for field count matching                                                                                              |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_310_ Validate missing collections in bundle after CCB-282 updates                                                                                |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------------+

enhancement
~~~~~~~~~~~

+---------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                          |Priority / Bug Severity   |
+===============================================================================================================+==========================+
|validate_17_ Validate schematron references and throw fatal error if invalid URI specified                     |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_24_ Update context check to retrieve and use latest context products from EN Registry                 |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_51_ Provide the capability to specify multiple locations for pds4.bundle validation                   |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_81_ Validate and throw error when duplicate LIDs are found in Bundle                                  |p.should-have             |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_230_ Update validate per SR requirements for collection inventories                                   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_238_ validate does not perform full bundle validation when using a specific bundle.xml                |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_246_ Add output directory flag to validate-bundle tool                                                |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_249_ Improvements for validating accumulating bundles / collections                                   |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_252_ Implement initial behavioral testing framework with cucumber                                     |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_254_ validate does not perform expediently when doing bundle-level validation against large bundles   |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_264_ Update installation documentation to include 64-bit Java as system requirement                   |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_290_ Migrate subset of existing regression tests to cucumber behavioral testing                       |unk                       |
+---------------------------------------------------------------------------------------------------------------+--------------------------+

requirement
~~~~~~~~~~~

+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                                         |Priority / Bug Severity   |
+==============================================================================================================================+==========================+
|validate_188_ As a user, I want to validate a bundle that uses multiple versions of the Information Model / Discipline LDDs   |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_210_ As a user, I want validate to raise a WARNING when differing versions of IM are used within a bundle            |p.could-have              |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_292_ CCB-264: Make the Line Feed (LF) character an allowed record delimiter                                          |unk                       |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_322_ Update installation documentation to require Java 1.9+                                                          |unk                       |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+
|validate_323_ Upgrade to Java 9+                                                                                              |unk                       |
+------------------------------------------------------------------------------------------------------------------------------+--------------------------+

theme
~~~~~

+-----------------------------------------------------------------------------------------------------------+--------------------------+
|Issue                                                                                                      |Priority / Bug Severity   |
+===========================================================================================================+==========================+
|validate_250_ Improvements to meet updated Standards Reference since initial requirements implementation   |unk                       |
+-----------------------------------------------------------------------------------------------------------+--------------------------+

.. _validate_5: https://github.com/NASA-PDS/validate/issues/5
.. _validate_6: https://github.com/NASA-PDS/validate/issues/6
.. _validate_11: https://github.com/NASA-PDS/validate/issues/11
.. _validate_153: https://github.com/NASA-PDS/validate/issues/153
.. _validate_189: https://github.com/NASA-PDS/validate/issues/189
.. _validate_240: https://github.com/NASA-PDS/validate/issues/240
.. _validate_256: https://github.com/NASA-PDS/validate/issues/256
.. _validate_257: https://github.com/NASA-PDS/validate/issues/257
.. _validate_260: https://github.com/NASA-PDS/validate/issues/260
.. _validate_271: https://github.com/NASA-PDS/validate/issues/271
.. _validate_273: https://github.com/NASA-PDS/validate/issues/273
.. _validate_278: https://github.com/NASA-PDS/validate/issues/278
.. _validate_281: https://github.com/NASA-PDS/validate/issues/281
.. _validate_291: https://github.com/NASA-PDS/validate/issues/291
.. _validate_294: https://github.com/NASA-PDS/validate/issues/294
.. _validate_297: https://github.com/NASA-PDS/validate/issues/297
.. _validate_298: https://github.com/NASA-PDS/validate/issues/298
.. _validate_299: https://github.com/NASA-PDS/validate/issues/299
.. _validate_300: https://github.com/NASA-PDS/validate/issues/300
.. _validate_301: https://github.com/NASA-PDS/validate/issues/301
.. _validate_310: https://github.com/NASA-PDS/validate/issues/310
.. _validate_17: https://github.com/NASA-PDS/validate/issues/17
.. _validate_24: https://github.com/NASA-PDS/validate/issues/24
.. _validate_51: https://github.com/NASA-PDS/validate/issues/51
.. _validate_81: https://github.com/NASA-PDS/validate/issues/81
.. _validate_230: https://github.com/NASA-PDS/validate/issues/230
.. _validate_238: https://github.com/NASA-PDS/validate/issues/238
.. _validate_246: https://github.com/NASA-PDS/validate/issues/246
.. _validate_249: https://github.com/NASA-PDS/validate/issues/249
.. _validate_252: https://github.com/NASA-PDS/validate/issues/252
.. _validate_254: https://github.com/NASA-PDS/validate/issues/254
.. _validate_264: https://github.com/NASA-PDS/validate/issues/264
.. _validate_290: https://github.com/NASA-PDS/validate/issues/290
.. _validate_188: https://github.com/NASA-PDS/validate/issues/188
.. _validate_210: https://github.com/NASA-PDS/validate/issues/210
.. _validate_292: https://github.com/NASA-PDS/validate/issues/292
.. _validate_322: https://github.com/NASA-PDS/validate/issues/322
.. _validate_323: https://github.com/NASA-PDS/validate/issues/323
.. _validate_250: https://github.com/NASA-PDS/validate/issues/250
