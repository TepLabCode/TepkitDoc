tepkit.io.vasp.ExplicitKpoints
==============================

.. py:class:: tepkit.io.vasp.ExplicitKpoints(mode: str | Kpoints, kpts: tepkit.utils.typing_tools.NumpyArrayNx3[float] | list[list[float]], kpts_weights: tepkit.utils.typing_tools.NumpyArray[float] | list[float], comment: str = 'KPOINTS')

   Bases: :py:obj:`Kpoints`



   Ref:
   - https://www.vasp.at/wiki/index.php/KPOINTS



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``comment``", "``None``", "The 1st line: The comment line."
   "``coordinates_mode``", "``None``", "The coordinate mode. Cartesian or Reciprocal."
   "``kpts``", "``None``", ""
   "``kpts_weights``", "``None``", ""
   "``b_lattice``", "``None``", ""


Properties
----------

.. autoapisummary::

   tepkit.io.vasp.ExplicitKpoints.num_kpts
   tepkit.io.vasp.ExplicitKpoints.df





Methods
-------

.. autoapisummary::

   tepkit.io.vasp.ExplicitKpoints.from_string
   tepkit.io.vasp.ExplicitKpoints.__str__
   tepkit.io.vasp.ExplicitKpoints.get_pymatgen_kpoints
   tepkit.io.vasp.ExplicitKpoints.__add__
   tepkit.io.vasp.ExplicitKpoints.plot
   tepkit.io.vasp.ExplicitKpoints.show




All Members
-----------


.. py:attribute:: comment
   :no-index:


   The 1st line: The comment line.



.. py:attribute:: coordinates_mode
   :no-index:
   :type:  Kpoints


   The coordinate mode. Cartesian or Reciprocal.



.. py:attribute:: kpts
   :no-index:
   :type:  NumpyArrayNx3[float]



.. py:attribute:: kpts_weights
   :no-index:
   :type:  NumpyArray[float]



.. py:attribute:: b_lattice
   :no-index:
   :value: None



.. py:property:: num_kpts
   :no-index:
   :type: int



.. py:property:: df
   :no-index:



.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:


   从字符串中读取结构化数据。



.. py:method:: __str__()
   :no-index:



.. py:method:: get_pymatgen_kpoints()
   :no-index:



.. py:method:: __add__(other)
   :no-index:



.. py:method:: plot(ax=None, show=False, save_path=None)
   :no-index:



.. py:method:: show()
   :no-index:




