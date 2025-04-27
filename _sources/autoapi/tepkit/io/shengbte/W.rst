tepkit.io.shengbte.W
====================

.. py:class:: tepkit.io.shengbte.W(omega: Omega = None)

   Bases: :py:obj:`tepkit.io.shengbte.OmegaParalleledFile`, :py:obj:`tepkit.io.shengbte.SubdirFile`



   For ShengBTE output files ``BTE.w`` and ``BTE.w_*`` (Scattering rate).

   Table Strcture
   ==============

   .. list-table::
      :widths: 10 10 10
      :header-rows: 2
      :stub-columns: 1

      * - Quantity
        - Angular Frequency
        - Scattering Rate
      * - Unit
        - rad/ps
        - 1/ps
      * - Line 0
        - *float*
        - *float*
      * - ...
        - ...
        - ...

   Supported Files
   ==================================

   Root-dir Files
   ----------------------------------
   - ``BTE.w_boundary``
   - ``BTE.w_isotopic``

   Temperature-dependent-subdir Files
   ----------------------------------
   - ``BTE.w``
   - ``BTE.w_anharmonic``
   - ``BTE.w_anharmonic_plus``
   - ``BTE.w_anharmonic_minus``
   - ``BTE.w_final``




Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'BTE.w_final'``", "The default name of file when use ``from_dir()`` ."
   "``column_indices``", "``None``", ""
   "``omega``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.W.plot




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'BTE.w_final'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: column_indices
   :no-index:
   :type:  dict



.. py:attribute:: omega
   :no-index:



.. py:method:: plot(ax, direction, x_unit='rad/ps', colors=None, group='111n')
   :no-index:




