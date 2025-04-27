tepkit.io.vasp.poscar.Poscar
============================

.. py:class:: tepkit.io.vasp.poscar.Poscar

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   See: https://www.vasp.at/wiki/index.php/POSCAR



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'POSCAR'``", "The default name of file when use ``from_dir()`` ."
   "``comment``", "``'POSCAR'``", "The first line of POSCAR."
   "``scaling_factor``", "``1.0``", ""
   "``unscale_lattice``", "``None``", ""
   "``has_species_names``", "``True``", ""
   "``species_names``", "``[]``", ""
   "``ions_per_species``", "``[]``", ""
   "``ion_coordinates_mode``", "``None``", ""
   "``ion_positions``", "``None``", ""
   "``has_selective_dynamics``", "``False``", ""
   "``selective_dynamics``", "``None``", ""
   "``has_lattice_velocities``", "``False``", ""
   "``lattice_velocities``", "``None``", ""
   "``has_ion_velocities``", "``False``", ""
   "``ion_velocities``", "``None``", ""
   "``md_extra``", "``None``", ""


Properties
----------

.. autoapisummary::

   tepkit.io.vasp.poscar.Poscar.lattice
   tepkit.io.vasp.poscar.Poscar.reciprocal_lattice
   tepkit.io.vasp.poscar.Poscar.n_ions
   tepkit.io.vasp.poscar.Poscar.thickness_info





Methods
-------

.. autoapisummary::

   tepkit.io.vasp.poscar.Poscar.from_string
   tepkit.io.vasp.poscar.Poscar.__str__
   tepkit.io.vasp.poscar.Poscar.get_lattice
   tepkit.io.vasp.poscar.Poscar.get_reciprocal_lattice
   tepkit.io.vasp.poscar.Poscar.get_cartesian_ion_positions
   tepkit.io.vasp.poscar.Poscar.get_fractional_ion_positions
   tepkit.io.vasp.poscar.Poscar.get_volume
   tepkit.io.vasp.poscar.Poscar.get_high_symmetry_points_2d
   tepkit.io.vasp.poscar.Poscar.get_interatomic_distances
   tepkit.io.vasp.poscar.Poscar.get_neighbor_distances
   tepkit.io.vasp.poscar.Poscar.get_atomic_numbers
   tepkit.io.vasp.poscar.Poscar.get_pymatgen_poscar
   tepkit.io.vasp.poscar.Poscar.to_supercell
   tepkit.io.vasp.poscar.Poscar.get_shengbte_types




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'POSCAR'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: comment
   :no-index:
   :type:  str
   :value: 'POSCAR'


   The first line of POSCAR.



.. py:attribute:: scaling_factor
   :no-index:
   :type:  float | list[float]
   :value: 1.0



.. py:attribute:: unscale_lattice
   :no-index:
   :type:  Optional[NumpyArray3x3[float]]
   :value: None



.. py:attribute:: has_species_names
   :no-index:
   :type:  bool
   :value: True



.. py:attribute:: species_names
   :no-index:
   :type:  list[str]
   :value: []



.. py:attribute:: ions_per_species
   :no-index:
   :type:  list[int]
   :value: []



.. py:attribute:: ion_coordinates_mode
   :no-index:
   :type:  VaspCoordinatesMode



.. py:attribute:: ion_positions
   :no-index:
   :type:  Optional[NumpyArrayNx3[float]]
   :value: None



.. py:attribute:: has_selective_dynamics
   :no-index:
   :type:  bool
   :value: False



.. py:attribute:: selective_dynamics
   :no-index:
   :type:  Optional[NumpyArrayNx3[bool]]
   :value: None



.. py:attribute:: has_lattice_velocities
   :no-index:
   :type:  bool
   :value: False



.. py:attribute:: lattice_velocities
   :no-index:
   :type:  Optional[NumpyArrayNx3[float]]
   :value: None



.. py:attribute:: has_ion_velocities
   :no-index:
   :type:  bool
   :value: False



.. py:attribute:: ion_velocities
   :no-index:
   :type:  Optional[NumpyArrayNx3[float]]
   :value: None



.. py:attribute:: md_extra
   :no-index:
   :type:  Optional[str]
   :value: None



.. py:method:: from_string(string: str) -> Self
   :no-index:
   :classmethod:


   Parse the string to structured data.



.. py:method:: __str__()
   :no-index:



.. py:method:: get_lattice() -> NumpyArray3x3[float]
   :no-index:



.. py:method:: get_reciprocal_lattice(with_2pi=True) -> NumpyArray3x3[float]
   :no-index:


   :param with_2pi: VASP Cartesian KPOINTS use with_2pi=False
   :return:



.. py:property:: lattice
   :no-index:
   :type: NumpyArray3x3[float]



.. py:property:: reciprocal_lattice
   :no-index:
   :type: NumpyArray3x3[float]



.. py:property:: n_ions
   :no-index:
   :type: int



.. py:property:: thickness_info
   :no-index:
   :type: dict


   Returns thickness-related data.
   Such as effective thickness, van der Waals radius of edge atoms, etc.



.. py:method:: get_cartesian_ion_positions() -> NumpyArrayNx3[float]
   :no-index:



.. py:method:: get_fractional_ion_positions() -> NumpyArrayNx3[float]
   :no-index:



.. py:method:: get_volume(unit: str = 'Angstrom^3') -> float
   :no-index:



.. py:method:: get_high_symmetry_points_2d(decimal, with_2pi=True)
   :no-index:


   Get the absolute and relative coordinates of all possible high symmetry points of a 2D material.

   :param decimal:
   :param with_2pi: VASP Cartesian KPOINTS use with_2pi=False
   :return:



.. py:method:: get_interatomic_distances() -> NumpyArrayNxN[float]
   :no-index:


   Return the distances between ions.



.. py:method:: get_neighbor_distances(max_nth=100) -> list[float]
   :no-index:


   Return the distances of the n-th neighbors.



.. py:method:: get_atomic_numbers(per_ion=False) -> list[int]
   :no-index:


   >>> poscar = Poscar.from_file("Bi2Te3.poscar")
   >>> poscar.get_atomic_numbers() # noinspection PyDocstringTypes
   [83, 52]
   >>> poscar.get_atomic_numbers(per_ion=True)
   [83, 83, 52, 52, 52]



.. py:method:: get_pymatgen_poscar()
   :no-index:



.. py:method:: to_supercell(na: int, nb: int, nc: int) -> Self
   :no-index:



.. py:method:: get_shengbte_types(start=1)
   :no-index:


   返回每个原子的元素在元素列表的索引
   例： [0, 0, 1, 1, 2]




