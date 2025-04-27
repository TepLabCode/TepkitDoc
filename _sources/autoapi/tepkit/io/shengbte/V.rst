tepkit.io.shengbte.V
====================

.. py:class:: tepkit.io.shengbte.V(omega: Omega = None)

   Bases: :py:obj:`tepkit.io.shengbte.OmegaLengthFile`



   For ShengBTE output file ``BTE.v`` (Group velocity).

   Table Strcture
   ==============

   .. list-table::
      :widths: 10 10 10 10
      :header-rows: 3
      :stub-columns: 1

      * - Quantity
        - Group Velocity
        - —
        - —
      * - Unit
        - km/s
        - —
        - —
      * - Direction
        - x
        - y
        - z
      * - Line 0
        - *float*
        - *float*
        - *float*
      * - ...
        - ...
        - ...
        - ...

   Supported Files
   ===============
   - ``BTE.v``




Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'BTE.v'``", "The default name of file when use ``from_dir()`` ."
   "``column_indices``", "``None``", ""
   "``omega``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.V.calculate_speed
   tepkit.io.shengbte.V.plot




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'BTE.v'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: column_indices
   :no-index:



.. py:attribute:: omega
   :no-index:



.. py:method:: calculate_speed()
   :no-index:


   增加 ("Frequency", "THz") 列



.. py:method:: plot(ax, direction, x_unit='rad/ps', colors=None, group='111n')
   :no-index:




