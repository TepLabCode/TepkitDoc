tepkit.utils.mpl_tools.ticker_tools
===================================

.. py:module:: tepkit.utils.mpl_tools.ticker_tools

.. autoapi-nested-parse::

   Ref: https://matplotlib.org/stable/api/ticker_api.html



Attributes
----------

.. autoapisummary::

   tepkit.utils.mpl_tools.ticker_tools.ticker_locators
   tepkit.utils.mpl_tools.ticker_tools.ticker_formatters


Functions
---------

.. autoapisummary::

   tepkit.utils.mpl_tools.ticker_tools.set_axis_ticker_locator
   tepkit.utils.mpl_tools.ticker_tools.set_axes_ticker_locator
   tepkit.utils.mpl_tools.ticker_tools.set_ticker_locator
   tepkit.utils.mpl_tools.ticker_tools.set_axis_ticker_formatter
   tepkit.utils.mpl_tools.ticker_tools.set_axes_ticker_formatter
   tepkit.utils.mpl_tools.ticker_tools.set_ticker_formatter
   tepkit.utils.mpl_tools.ticker_tools.test


Module Contents
---------------

.. py:data:: ticker_locators
   :no-index:


.. py:function:: set_axis_ticker_locator(axis: matplotlib.axis.Axis, locator: str, arg: Any = None, minor: bool = False)

   Set the ticker locator of the given axis (ax.xaxis or ax.yaxis).


.. py:function:: set_axes_ticker_locator(ax: matplotlib.axes.Axes, direction: str, locator: str, arg: Any = None, minor: bool = False)

   Set the ticker locator of the given axes (ax).
   Usage:
   >>> set_axes_ticker_locator(ax, "x", "auto")
   >>> set_axes_ticker_locator(ax, "x", "gap", 10)
   >>> set_axes_ticker_locator(ax, "y", "log", {"base": 10})


.. py:function:: set_ticker_locator(target: matplotlib.axis.Axis | matplotlib.axes.Axes, locator: str, arg: Any = None, minor: bool = False, direction: str = None)

   Set the ticker locator of the given axis (ax.xaxis or ax.yaxis) or axes (ax).


.. py:data:: ticker_formatters
   :no-index:


.. py:function:: set_axis_ticker_formatter(axis: matplotlib.axis.Axis, formatter: str, arg: Any = None, minor: bool = False)

   Set the ticker formatter of the given axis (ax.xaxis or ax.yaxis).


.. py:function:: set_axes_ticker_formatter(ax: matplotlib.axes.Axes, direction: str, formatter: str, arg: Any = None, minor: bool = False)

   Set the ticker formatter of the given axes (ax).
   Usage:
   >>> set_axes_ticker_formatter(ax, "x", "null")
   >>> set_axes_ticker_formatter(ax, "y", "log", {"base": 10})


.. py:function:: set_ticker_formatter(target: matplotlib.axis.Axis | matplotlib.axes.Axes, formatter: str, direction: str = None, arg: Any = None, minor: bool = False)

   Set the ticker formatter of the given axis (ax.xaxis or ax.yaxis) or axes (ax).


.. py:function:: test()

