tepkit.io.shengbte.SubdirFile
=============================

.. py:class:: tepkit.io.shengbte.SubdirFile

   Bases: :py:obj:`tepkit.io.File`



   ShengBTE 温度子文件夹中文件的文件类。



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``t``", "``None``", "The temperature (K) of the subdir."






Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.SubdirFile.from_dir




All Members
-----------


.. py:attribute:: t
   :no-index:
   :type:  int
   :value: None


   The temperature (K) of the subdir. 



.. py:method:: from_dir(path: tepkit.utils.typing_tools.PathLike = None, file_name: str = None, t: int = None) -> Self
   :no-index:
   :classmethod:


   @override File.from_dir()
   Add `t` (temperature) argument to specify the subdir f"T{t}K".




