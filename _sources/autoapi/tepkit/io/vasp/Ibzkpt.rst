tepkit.io.vasp.Ibzkpt
=====================

.. py:class:: tepkit.io.vasp.Ibzkpt(mode: str | Kpoints, kpts: tepkit.utils.typing_tools.NumpyArrayNx3[float] | list[list[float]], kpts_weights: tepkit.utils.typing_tools.NumpyArray[float] | list[float], comment: str = 'KPOINTS')

   Bases: :py:obj:`ExplicitKpoints`



   Ref:
   - https://www.vasp.at/wiki/index.php/KPOINTS
   - https://www.vasp.at/wiki/index.php/IBZKPT



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'IBZKPT'``", "The default name of file when use ``from_dir()`` ."









All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'IBZKPT'


   The default name of file when use ``from_dir()`` .




