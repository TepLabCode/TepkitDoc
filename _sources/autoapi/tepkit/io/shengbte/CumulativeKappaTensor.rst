tepkit.io.shengbte.CumulativeKappaTensor
========================================

.. py:class:: tepkit.io.shengbte.CumulativeKappaTensor

   Bases: :py:obj:`tepkit.io.shengbte.NticksLengthFile`, :py:obj:`tepkit.io.shengbte.SubdirFile`, :py:obj:`KappaEtcMixin`



   For ShengBTE output file ``BTE.cumulative_kappa_tensor`` .

   Supported Files
   ===============
   - BTE.cumulative_kappa_tensor



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'BTE.cumulative_kappa_tensor'``", "The default name of file when use ``from_dir()`` ."
   "``column_indices``", "``None``", ""
   "``fit_func``", "``None``", ""
   "``x0``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.CumulativeKappaTensor.get_fit_func
   tepkit.io.shengbte.CumulativeKappaTensor.calculate_fitted_kappal
   tepkit.io.shengbte.CumulativeKappaTensor.plot




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'BTE.cumulative_kappa_tensor'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: column_indices
   :no-index:



.. py:attribute:: fit_func
   :no-index:



.. py:attribute:: x0
   :no-index:



.. py:method:: get_fit_func(direction) -> Callable
   :no-index:



.. py:method:: calculate_fitted_kappal(direction)
   :no-index:



.. py:method:: plot(ax, direction, fit=False, x0=False, color='blue')
   :no-index:




