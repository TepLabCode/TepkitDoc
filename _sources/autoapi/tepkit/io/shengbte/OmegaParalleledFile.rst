tepkit.io.shengbte.OmegaParalleledFile
======================================

.. py:class:: tepkit.io.shengbte.OmegaParalleledFile

   Bases: :py:obj:`tepkit.io.TableTextFile`



   由 频率 和 数值 两列数据组成的数据文件。
   @shape: (n_qpoints * n_modes, 2)
   ---
   Supported Files:
   - ``BTE.w*``
   - ``T*K/``

       - ``BTE.WP3*``
       - ``BTE.WP4*``
       - ``BTE.w*``



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``column_indices``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.OmegaParalleledFile.reshape_to




All Members
-----------


.. py:attribute:: column_indices
   :no-index:



.. py:method:: reshape_to(shape)
   :no-index:




