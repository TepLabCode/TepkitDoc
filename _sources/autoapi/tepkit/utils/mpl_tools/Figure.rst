tepkit.utils.mpl_tools.Figure
=============================

.. py:class:: tepkit.utils.mpl_tools.Figure(width: float = 1.0, height: float = 0.9, dpi: float = None, font_size=None, style='tepkit_basic', projection=None)



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``width``", "``None``", "| The ratio to the recommended width (3.334 inch = 1000 px at 300 dpi ≈ 8.47 cm),
   | default set to 1.0."
   "``height``", "``None``", "| The ratio to the recommended height (3.334 inch = 1000 px at 300 dpi ≈ 8.47 cm),
   | default set to 0.9."
   "``fig``", "``None``", ""
   "``ax``", "``None``", ""
   "``legend``", "``None``", "The latest legend added by ``.add_legend()``."
   "``colorbar``", "``None``", "The latest colorbar added by ``.add_colorbar()``."






Methods
-------

.. autoapisummary::

   tepkit.utils.mpl_tools.Figure.add_legend
   tepkit.utils.mpl_tools.Figure.add_colorbar
   tepkit.utils.mpl_tools.Figure.adjust_margin
   tepkit.utils.mpl_tools.Figure.set_locator
   tepkit.utils.mpl_tools.Figure.set_formatter
   tepkit.utils.mpl_tools.Figure.save
   tepkit.utils.mpl_tools.Figure.show




All Members
-----------


.. py:attribute:: width
   :no-index:
   :type:  int | float


   | The ratio to the recommended width (3.334 inch = 1000 px at 300 dpi ≈ 8.47 cm),
   | default set to 1.0.



.. py:attribute:: height
   :no-index:
   :type:  int | float


   | The ratio to the recommended height (3.334 inch = 1000 px at 300 dpi ≈ 8.47 cm),
   | default set to 0.9.



.. py:attribute:: fig
   :no-index:



.. py:attribute:: ax
   :no-index:



.. py:attribute:: legend
   :no-index:
   :value: None


   The latest legend added by ``.add_legend()``.



.. py:attribute:: colorbar
   :no-index:
   :value: None


   The latest colorbar added by ``.add_colorbar()``.



.. py:method:: add_legend(*args, border_width: int | float | None = None, **kwargs)
   :no-index:


   A wrapper of ``matplotlib.pyplot.legend()``.

   :return: ``matplotlib.legend.Legend``

   Features
   ========
   - Add parameter aliases:
       - ``font_size``: ``fontsize``
   - Add automatic behaviors:
       - Sync the border width of the legend to the left axis.
   - Add new parameters:
       - ``border_width``: Set the border width of the legend.



.. py:method:: add_colorbar(*args, width: int | float = 1, height: int | float = 1, border_width: int | float | None = None, **kwargs)
   :no-index:


   A wrapper of ``matplotlib.pyplot.colorbar()``.

   :return: ``matplotlib.colorbar.Colorbar``

   Features
   ========
   - Add automatic behaviors:
       - Sync the border width of the colorbar to the left axis.
   - Add new parameters:
       - ``width`` and ``height``: Change the size of the colorbar.
       - ``border_width``: Set the border width of the colorbar.



.. py:method:: adjust_margin(*, top=None, right=None, bottom=None, left=None, wspace=None, hspace=None) -> None
   :no-index:
   :staticmethod:


   A wrapper of ``matplotlib.pyplot.subplots_adjust()``.

   Adjust the margin of the figure **in pixels**.



.. py:method:: set_locator(*args, **kwargs)
   :no-index:


   A wrapper of ``tepkit.utils.mpl_tools.ticker_tools.set_axes_ticker_locator()``.

   Set ``ax`` as ``self.ax``.



.. py:method:: set_formatter(*args, **kwargs)
   :no-index:


   A wrapper of ``tepkit.utils.mpl_tools.ticker_tools.set_axes_ticker_formatter()``.

   Set ``ax`` as ``self.ax``.



.. py:method:: save(path='tepkit.figure.png', **kwargs) -> None
   :no-index:


   A wrapper of ``matplotlib.figure.Figure.savefig()``.

   Features
   ========
   - Add parameter aliases:
       - ``path``: ``fname``
   - Add parameter default value:
       - ``path``: ``tepkit.figure.png``



.. py:method:: show(dpi=200)
   :no-index:


   A wrapper of ``matplotlib.pyplot.show()``.

   Features
   ========
   - Add new parameters:
       - ``dpi``: Change the dpi of the figure before show it to avoid covering too much of the screen.




