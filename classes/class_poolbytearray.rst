.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the PoolByteArray.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_PoolByteArray:

PoolByteArray
=============

**Category:** Built-In Types

Brief Description
-----------------

Raw byte array.

Member Functions
----------------

+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolByteArray<class_poolbytearray>`  | :ref:`PoolByteArray<class_PoolByteArray_PoolByteArray>` **(** :ref:`Array<class_array>` from **)**                                        |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`append<class_PoolByteArray_append>` **(** :ref:`int<class_int>` byte **)**                                                          |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`append_array<class_PoolByteArray_append_array>` **(** :ref:`PoolByteArray<class_poolbytearray>` array **)**                         |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolByteArray<class_poolbytearray>`  | :ref:`compress<class_PoolByteArray_compress>` **(** :ref:`int<class_int>` compression_mode=0 **)**                                        |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolByteArray<class_poolbytearray>`  | :ref:`decompress<class_PoolByteArray_decompress>` **(** :ref:`int<class_int>` buffer_size, :ref:`int<class_int>` compression_mode=0 **)** |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_string>`                | :ref:`get_string_from_ascii<class_PoolByteArray_get_string_from_ascii>` **(** **)**                                                       |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_string>`                | :ref:`get_string_from_utf8<class_PoolByteArray_get_string_from_utf8>` **(** **)**                                                         |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                      | :ref:`insert<class_PoolByteArray_insert>` **(** :ref:`int<class_int>` idx, :ref:`int<class_int>` byte **)**                               |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`invert<class_PoolByteArray_invert>` **(** **)**                                                                                     |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`push_back<class_PoolByteArray_push_back>` **(** :ref:`int<class_int>` byte **)**                                                    |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`remove<class_PoolByteArray_remove>` **(** :ref:`int<class_int>` idx **)**                                                           |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`resize<class_PoolByteArray_resize>` **(** :ref:`int<class_int>` idx **)**                                                           |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| void                                       | :ref:`set<class_PoolByteArray_set>` **(** :ref:`int<class_int>` idx, :ref:`int<class_int>` byte **)**                                     |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                      | :ref:`size<class_PoolByteArray_size>` **(** **)**                                                                                         |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PoolByteArray<class_poolbytearray>`  | :ref:`subarray<class_PoolByteArray_subarray>` **(** :ref:`int<class_int>` from, :ref:`int<class_int>` to **)**                            |
+--------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+

Description
-----------

Raw byte array. Contains bytes. Optimized for memory usage, can't fragment the memory.

Member Function Description
---------------------------

.. _class_PoolByteArray_PoolByteArray:

- :ref:`PoolByteArray<class_poolbytearray>` **PoolByteArray** **(** :ref:`Array<class_array>` from **)**

Create from a generic array.

.. _class_PoolByteArray_append:

- void **append** **(** :ref:`int<class_int>` byte **)**

Append an element at the end of the array (alias of :ref:`push_back<class_PoolByteArray_push_back>`).

.. _class_PoolByteArray_append_array:

- void **append_array** **(** :ref:`PoolByteArray<class_poolbytearray>` array **)**

Append a ``PoolByteArray`` at the end of this array.

.. _class_PoolByteArray_compress:

- :ref:`PoolByteArray<class_poolbytearray>` **compress** **(** :ref:`int<class_int>` compression_mode=0 **)**

Returns a new ``PoolByteArray`` with the data compressed. Set the compression mode using one of :ref:`File<class_file>`'s COMPRESS\_\* constants.

.. _class_PoolByteArray_decompress:

- :ref:`PoolByteArray<class_poolbytearray>` **decompress** **(** :ref:`int<class_int>` buffer_size, :ref:`int<class_int>` compression_mode=0 **)**

Returns a new ``PoolByteArray`` with the data decompressed. Set buffer_size to the size of the uncompressed data. Set the compression mode using one of :ref:`File<class_file>`'s COMPRESS\_\* constants.

.. _class_PoolByteArray_get_string_from_ascii:

- :ref:`String<class_string>` **get_string_from_ascii** **(** **)**

Returns a copy of the array's contents as :ref:`String<class_string>`. Fast alternative to :ref:`PoolByteArray.get_string_from_utf8<class_PoolByteArray_get_string_from_utf8>` if the content is ASCII-only. Unlike the UTF-8 function this function maps every byte to a character in the array. Multibyte sequences will not be interpreted correctly. For parsing user input always use :ref:`PoolByteArray.get_string_from_utf8<class_PoolByteArray_get_string_from_utf8>`.

.. _class_PoolByteArray_get_string_from_utf8:

- :ref:`String<class_string>` **get_string_from_utf8** **(** **)**

Returns a copy of the array's contents as :ref:`String<class_string>`. Slower than :ref:`PoolByteArray.get_string_from_ascii<class_PoolByteArray_get_string_from_ascii>` but supports UTF-8 encoded data. Use this function if you are unsure about the source of the data. For user input this function should always be preferred.

.. _class_PoolByteArray_insert:

- :ref:`int<class_int>` **insert** **(** :ref:`int<class_int>` idx, :ref:`int<class_int>` byte **)**

Insert a new element at a given position in the array. The position must be valid, or at the end of the array (pos==size()).

.. _class_PoolByteArray_invert:

- void **invert** **(** **)**

Reverse the order of the elements in the array (so first element will now be the last).

.. _class_PoolByteArray_push_back:

- void **push_back** **(** :ref:`int<class_int>` byte **)**

Append an element at the end of the array.

.. _class_PoolByteArray_remove:

- void **remove** **(** :ref:`int<class_int>` idx **)**

Remove an element from the array by index.

.. _class_PoolByteArray_resize:

- void **resize** **(** :ref:`int<class_int>` idx **)**

Set the size of the array. If the array is grown reserve elements at the end of the array. If the array is shrunk truncate the array to the new size.

.. _class_PoolByteArray_set:

- void **set** **(** :ref:`int<class_int>` idx, :ref:`int<class_int>` byte **)**

Change the byte at the given index.

.. _class_PoolByteArray_size:

- :ref:`int<class_int>` **size** **(** **)**

Return the size of the array.

.. _class_PoolByteArray_subarray:

- :ref:`PoolByteArray<class_poolbytearray>` **subarray** **(** :ref:`int<class_int>` from, :ref:`int<class_int>` to **)**

Returns the slice of the ``PoolByteArray`` between indices (inclusive) as a new ``PoolByteArray``.  Any negative index is considered to be from the end of the array.


