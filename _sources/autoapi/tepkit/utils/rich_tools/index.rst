tepkit.utils.rich_tools
=======================

.. py:module:: tepkit.utils.rich_tools


Attributes
----------

.. autoapisummary::

   tepkit.utils.rich_tools.PANEL_PRESETS


Classes
-------

.. toctree::
   :hidden:

   /autoapi/tepkit/utils/rich_tools/TablePrinter

.. autoapisummary::

   tepkit.utils.rich_tools.TablePrinter


Functions
---------

.. autoapisummary::

   tepkit.utils.rich_tools.print_panel
   tepkit.utils.rich_tools.print_table
   tepkit.utils.rich_tools.print_args


Module Contents
---------------

.. py:data:: PANEL_PRESETS
   :no-index:


.. py:function:: print_panel(content: str, preset: str = None, **kwargs) -> rich.panel.Panel

.. py:function:: print_table(dictionary: dict, title: str = '', key: str = 'Keys', value: str = 'Values', table_options: dict = None, key_options: dict = None, value_options: dict = None) -> rich.table.Table

   A function to easily print a dict as a Rich table.

   :param dictionary:
   :param title:
   :param key:
   :param value:
   :param table_options:
   :param key_options:
   :param value_options:
   :return:


.. py:function:: print_args(args) -> rich.table.Table

