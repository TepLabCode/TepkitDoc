tepkit.io.shengbte.Omega
========================

.. py:class:: tepkit.io.shengbte.Omega(omega=None)

   Bases: :py:obj:`tepkit.io.shengbte.OmegaShapedFile`



   For ShengBTE output file ``BTE.omega`` (Angular frequency).

   Table Strcture
   ==============

   .. list-table::
      :widths: 10 10 10 10
      :header-rows: 3
      :stub-columns: 1

      * - Quantity
        - Angular Frequency
        - —
        - ...
      * - Unit
        - rad/ps
        - —
        - ...
      * - Phonon Band Index
        - 1
        - 2
        - ...
      * - *q* point 0
        - *float*
        - *float*
        - ...
      * - ...
        - ...
        - ...
        - ...

   Supported Files
   ==================================
   - ``BTE.omega``




Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'BTE.omega'``", "The default name of file when use ``from_dir()`` ."
   "``column_indices``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.Omega.get_values
   tepkit.io.shengbte.Omega.plot_with




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'BTE.omega'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: column_indices
   :no-index:



.. py:method:: get_values(unit='rad/ps')
   :no-index:



.. py:method:: plot_with(ax, y_table, x_unit='rad/ps', colors=None, group='111n')
   :no-index:




