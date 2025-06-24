tepkit.utils.mpl_tools
======================

.. py:module:: tepkit.utils.mpl_tools


Submodules
----------

.. toctree::
   :maxdepth: 1

   /autoapi/tepkit/utils/mpl_tools/color_tools/index
   /autoapi/tepkit/utils/mpl_tools/font_tools/index
   /autoapi/tepkit/utils/mpl_tools/formatters/index
   /autoapi/tepkit/utils/mpl_tools/plotters/index
   /autoapi/tepkit/utils/mpl_tools/ticker_tools/index


Attributes
----------

.. autoapisummary::

   tepkit.utils.mpl_tools.package_root
   tepkit.utils.mpl_tools.style_dir
   tepkit.utils.mpl_tools.style_path


Classes
-------

.. toctree::
   :hidden:

   /autoapi/tepkit/utils/mpl_tools/Figure

.. autoapisummary::

   tepkit.utils.mpl_tools.Figure


Functions
---------

.. autoapisummary::

   tepkit.utils.mpl_tools.set_axes_ticker_formatter
   tepkit.utils.mpl_tools.set_axes_ticker_locator
   tepkit.utils.mpl_tools.adjust_legend_linewidth


Package Contents
----------------

.. py:data:: package_root
   :no-index:


.. py:function:: set_axes_ticker_formatter(ax: matplotlib.axes.Axes, direction: str, formatter: str, arg: Any = None, minor: bool = False)

   Set the ticker formatter of the given axes (ax).
   Usage:
   >>> set_axes_ticker_formatter(ax, "x", "null")
   >>> set_axes_ticker_formatter(ax, "y", "log", {"base": 10})


.. py:function:: set_axes_ticker_locator(ax: matplotlib.axes.Axes, direction: str, locator: str, arg: Any = None, minor: bool = False)

   Set the ticker locator of the given axes (ax).
   Usage:
   >>> set_axes_ticker_locator(ax, "x", "auto")
   >>> set_axes_ticker_locator(ax, "x", "gap", 10)
   >>> set_axes_ticker_locator(ax, "y", "log", {"base": 10})


.. py:data:: style_dir
   :no-index:


.. py:data:: style_path
   :no-index:


.. py:function:: adjust_legend_linewidth(ax, linewidth: float = None)

