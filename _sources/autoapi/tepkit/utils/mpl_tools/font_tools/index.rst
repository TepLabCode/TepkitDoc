tepkit.utils.mpl_tools.font_tools
=================================

.. py:module:: tepkit.utils.mpl_tools.font_tools


Attributes
----------

.. autoapisummary::

   tepkit.utils.mpl_tools.font_tools.RECOMMENDED_SERIF_FONTS
   tepkit.utils.mpl_tools.font_tools.RECOMMENDED_SANS_FONTS
   tepkit.utils.mpl_tools.font_tools.RECOMMENDED_MONO_FONTS
   tepkit.utils.mpl_tools.font_tools.RECOMMENDED_SERIF_FONTS_HANS
   tepkit.utils.mpl_tools.font_tools.RECOMMENDED_SANS_FONTS_HANS
   tepkit.utils.mpl_tools.font_tools.STYLE_TO_RECOMMENDED_FONTS
   tepkit.utils.mpl_tools.font_tools.result


Functions
---------

.. autoapisummary::

   tepkit.utils.mpl_tools.font_tools.is_font_avalible
   tepkit.utils.mpl_tools.font_tools.get_avalible_font_by_names
   tepkit.utils.mpl_tools.font_tools.get_recommended_font


Module Contents
---------------

.. py:data:: RECOMMENDED_SERIF_FONTS
   :no-index:
   :value: ['Times New Roman', 'FreeSerif', 'DejaVu Serif']


.. py:data:: RECOMMENDED_SANS_FONTS
   :no-index:
   :value: ['Helvetica', 'Arial', 'FreeSans', 'DejaVu Sans']


.. py:data:: RECOMMENDED_MONO_FONTS
   :no-index:
   :value: ['Consolas', 'FreeMono', 'DejaVu Sans Mono']


.. py:data:: RECOMMENDED_SERIF_FONTS_HANS
   :no-index:
   :value: ['Source Han Serif SC', 'Source Han Serif CN', 'SimSun']


.. py:data:: RECOMMENDED_SANS_FONTS_HANS
   :no-index:
   :value: ['Source Han Sans SC', 'Source Han Sans CN', 'Microsoft YaHei']


.. py:data:: STYLE_TO_RECOMMENDED_FONTS
   :no-index:


.. py:function:: is_font_avalible(font_name: str) -> bool

.. py:function:: get_avalible_font_by_names(font_names: list[str], fallback: bool = False) -> str

   Return the first available font name from a list of font names.

   :param font_names: A list of possible font names.
   :param fallback: Whether to return a fallback font ("DejaVu Sans") if no available font in the list.
   :raises ValueError: If no available font in the list and ``fallback`` is ``False``.


.. py:function:: get_recommended_font(style: str) -> str

   Get the first available font name by specify the font style.

   :param style: One of the "Serif", "Sans", "Mono", "Serif-Hans", or "Sans-Hans".


.. py:data:: result
   :no-index:


