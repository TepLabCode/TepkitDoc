tepkit.io.vasp.outcar.Outcar
============================

.. py:class:: tepkit.io.vasp.outcar.Outcar

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   The class for text file with special structure.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'OUTCAR'``", "The default name of file when use ``from_dir()`` ."


Properties
----------

.. autoapisummary::

   tepkit.io.vasp.outcar.Outcar.fermi_energy





Methods
-------

.. autoapisummary::

   tepkit.io.vasp.outcar.Outcar.job_state
   tepkit.io.vasp.outcar.Outcar.get_piezoelectric_stress_tensors




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'OUTCAR'


   The default name of file when use ``from_dir()`` .



.. py:property:: fermi_energy
   :no-index:
   :type: float



.. py:method:: job_state() -> tepkit.core.vasp.VaspState
   :no-index:



.. py:method:: get_piezoelectric_stress_tensors(cell_z: Annotated[float, Literal['Ang']] | None = None, only_xy: bool = False) -> dict
   :no-index:




