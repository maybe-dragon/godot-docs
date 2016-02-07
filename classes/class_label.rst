.. _class_Label:

Label
=====

**Inherits:** :ref:`Control<class_control>` **<** :ref:`CanvasItem<class_canvasitem>` **<** :ref:`Node<class_node>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

Control that displays formatted text.

Member Functions
----------------

+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_align<class_Label_set_align>`  **(** :ref:`int<class_int>` align  **)**                                   |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_align<class_Label_get_align>`  **(** **)** const                                                          |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_valign<class_Label_set_valign>`  **(** :ref:`int<class_int>` valign  **)**                                |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_valign<class_Label_get_valign>`  **(** **)** const                                                        |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_text<class_Label_set_text>`  **(** :ref:`String<class_string>` text  **)**                                |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_string>`  | :ref:`get_text<class_Label_get_text>`  **(** **)** const                                                            |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_autowrap<class_Label_set_autowrap>`  **(** :ref:`bool<class_bool>` enable  **)**                          |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`      | :ref:`has_autowrap<class_Label_has_autowrap>`  **(** **)** const                                                    |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_clip_text<class_Label_set_clip_text>`  **(** :ref:`bool<class_bool>` enable  **)**                        |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`      | :ref:`is_clipping_text<class_Label_is_clipping_text>`  **(** **)** const                                            |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_uppercase<class_Label_set_uppercase>`  **(** :ref:`bool<class_bool>` enable  **)**                        |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`      | :ref:`is_uppercase<class_Label_is_uppercase>`  **(** **)** const                                                    |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_line_height<class_Label_get_line_height>`  **(** **)** const                                              |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_line_count<class_Label_get_line_count>`  **(** **)** const                                                |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_total_character_count<class_Label_get_total_character_count>`  **(** **)** const                          |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_visible_characters<class_Label_set_visible_characters>`  **(** :ref:`int<class_int>` amount  **)**        |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_visible_characters<class_Label_get_visible_characters>`  **(** **)** const                                |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_percent_visible<class_Label_set_percent_visible>`  **(** :ref:`float<class_float>` percent_visible  **)** |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`    | :ref:`get_percent_visible<class_Label_get_percent_visible>`  **(** **)** const                                      |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_lines_skipped<class_Label_set_lines_skipped>`  **(** :ref:`int<class_int>` lines_skipped  **)**           |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_lines_skipped<class_Label_get_lines_skipped>`  **(** **)** const                                          |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| void                         | :ref:`set_max_lines_visible<class_Label_set_max_lines_visible>`  **(** :ref:`int<class_int>` lines_visible  **)**   |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`        | :ref:`get_max_lines_visible<class_Label_get_max_lines_visible>`  **(** **)** const                                  |
+------------------------------+---------------------------------------------------------------------------------------------------------------------+

Numeric Constants
-----------------

- **ALIGN_LEFT** = **0** --- Align rows to the left (default).
- **ALIGN_CENTER** = **1** --- Align rows centered.
- **ALIGN_RIGHT** = **2** --- Align rows to the right (default).
- **ALIGN_FILL** = **3** --- Expand row whitespaces to fit the width.
- **VALIGN_TOP** = **0** --- Align the whole text to the top.
- **VALIGN_CENTER** = **1** --- Align the whole text to the center.
- **VALIGN_BOTTOM** = **2** --- Align the whole text to the bottom.
- **VALIGN_FILL** = **3** --- Align the whole text by spreading the rows.

Description
-----------

Label is a control that displays formatted text, optionally autowrapping it to the :ref:`Control<class_control>` area. It inherits from range to be able to scroll wrapped text vertically.

Member Function Description
---------------------------

.. _class_Label_set_align:

- void  **set_align**  **(** :ref:`int<class_int>` align  **)**

Sets the alignment mode to any of the ALIGN\_\* enumeration values.

.. _class_Label_get_align:

- :ref:`int<class_int>`  **get_align**  **(** **)** const

Return the alignment mode (any of the ALIGN\_\* enumeration values).

.. _class_Label_set_valign:

- void  **set_valign**  **(** :ref:`int<class_int>` valign  **)**

Sets the vertical alignment mode to any of the VALIGN\_\* enumeration values.

.. _class_Label_get_valign:

- :ref:`int<class_int>`  **get_valign**  **(** **)** const

Return the vertical alignment mode (any of the VALIGN\_\* enumeration values).

.. _class_Label_set_text:

- void  **set_text**  **(** :ref:`String<class_string>` text  **)**

Set the label text. Text can contain newlines.

.. _class_Label_get_text:

- :ref:`String<class_string>`  **get_text**  **(** **)** const

Return the label text. Text can contain newlines.

.. _class_Label_set_autowrap:

- void  **set_autowrap**  **(** :ref:`bool<class_bool>` enable  **)**

Set *autowrap* mode. When enabled, autowrap will fit text to the control width, breaking sentences when they exceed the available horizontal space. When disabled, the label minimum width becomes the width of the longest row, and the minimum height large enough to fit all rows.

.. _class_Label_has_autowrap:

- :ref:`bool<class_bool>`  **has_autowrap**  **(** **)** const

Return the state of the *autowrap* mode (see :ref:`set_autowrap<class_Label_set_autowrap>`).

.. _class_Label_set_clip_text:

- void  **set_clip_text**  **(** :ref:`bool<class_bool>` enable  **)**

Cuts off the rest of the text if it is too wide.

.. _class_Label_is_clipping_text:

- :ref:`bool<class_bool>`  **is_clipping_text**  **(** **)** const

Return true if text would be cut off if it is too wide.

.. _class_Label_set_uppercase:

- void  **set_uppercase**  **(** :ref:`bool<class_bool>` enable  **)**

Display text in all capitals.

.. _class_Label_is_uppercase:

- :ref:`bool<class_bool>`  **is_uppercase**  **(** **)** const

Return true if text is displayed in all capitals.

.. _class_Label_get_line_height:

- :ref:`int<class_int>`  **get_line_height**  **(** **)** const

Return the height of a line.

.. _class_Label_get_line_count:

- :ref:`int<class_int>`  **get_line_count**  **(** **)** const

Return the amount of lines.

.. _class_Label_get_total_character_count:

- :ref:`int<class_int>`  **get_total_character_count**  **(** **)** const

Return the total length of the text.

.. _class_Label_set_visible_characters:

- void  **set_visible_characters**  **(** :ref:`int<class_int>` amount  **)**

Restricts the number of characters to display. Set to -1 to disable.

.. _class_Label_get_visible_characters:

- :ref:`int<class_int>`  **get_visible_characters**  **(** **)** const

Return the restricted number of characters to display. Returns -1 if unrestricted.

.. _class_Label_set_percent_visible:

- void  **set_percent_visible**  **(** :ref:`float<class_float>` percent_visible  **)**

Restricts the number of characters to display (as a percentage of the total text).

.. _class_Label_get_percent_visible:

- :ref:`float<class_float>`  **get_percent_visible**  **(** **)** const

Return the restricted number of characters to display (as a percentage of the total text).

.. _class_Label_set_lines_skipped:

- void  **set_lines_skipped**  **(** :ref:`int<class_int>` lines_skipped  **)**

Sets the number of lines to skip before displaying. Useful for scrolling text.

.. _class_Label_get_lines_skipped:

- :ref:`int<class_int>`  **get_lines_skipped**  **(** **)** const

Return the the number of lines to skipped before displaying.

.. _class_Label_set_max_lines_visible:

- void  **set_max_lines_visible**  **(** :ref:`int<class_int>` lines_visible  **)**

Restricts the number of lines to display. Set to -1 to disable.

.. _class_Label_get_max_lines_visible:

- :ref:`int<class_int>`  **get_max_lines_visible**  **(** **)** const

Return the restricted number of lines to display. Returns -1 if unrestricted.

