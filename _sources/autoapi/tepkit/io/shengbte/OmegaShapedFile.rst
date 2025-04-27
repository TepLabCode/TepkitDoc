tepkit.io.shengbte.OmegaShapedFile
==================================

.. py:class:: tepkit.io.shengbte.OmegaShapedFile(omega=None)

   Bases: :py:obj:`tepkit.io.TableTextFile`



   与 BTE.omega 的数据形状相同的数据文件。
   @shape: (n_qpoints, n_modes)
   ---
   Supported Files:
   - ``BTE.gruneisen``
   - ``BTE.omega``
   - ``BTE.P3*``
   - ``BTE.P4*``



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``omega``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.OmegaShapedFile.set_mode_names
   tepkit.io.shengbte.OmegaShapedFile.plot




All Members
-----------


.. py:attribute:: omega
   :no-index:



.. py:method:: set_mode_names(names=None)
   :no-index:



.. py:method:: plot(ax, x_unit='rad/ps', colors=None, group='111n')
   :no-index:




