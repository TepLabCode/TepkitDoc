tepkit.io.vasp.Poscar
=====================

.. py:class:: tepkit.io.vasp.Poscar

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   See: https://www.vasp.at/wiki/index.php/POSCAR



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'POSCAR'``", "The default name of file when use ``from_dir()`` ."
   "``comment``", "``'POSCAR'``", "The first line of POSCAR."
   "``scaling_factor``", "``1.0``", ""
   "``has_species_names``", "``True``", ""
   "``species_names``", "``['Unknown']``", ""
   "``ions_per_species``", "``[1]``", ""
   "``ion_coordinates_mode``", "``None``", ""
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

   tepkit.io.vasp.Poscar.unscale_lattice
   tepkit.io.vasp.Poscar.ion_positions
   tepkit.io.vasp.Poscar.lattice
   tepkit.io.vasp.Poscar.reciprocal_lattice
   tepkit.io.vasp.Poscar.n_ions
   tepkit.io.vasp.Poscar.species_index_per_ion
   tepkit.io.vasp.Poscar.species_name_per_ion
   tepkit.io.vasp.Poscar.thickness_info





Methods
-------

.. autoapisummary::

   tepkit.io.vasp.Poscar.from_string
   tepkit.io.vasp.Poscar.__str__
   tepkit.io.vasp.Poscar.get_lattice
   tepkit.io.vasp.Poscar.get_reciprocal_lattice
   tepkit.io.vasp.Poscar.get_shengbte_types
   tepkit.io.vasp.Poscar.get_cartesian_ion_positions
   tepkit.io.vasp.Poscar.get_fractional_ion_positions
   tepkit.io.vasp.Poscar.get_volume
   tepkit.io.vasp.Poscar.get_high_symmetry_points_2d
   tepkit.io.vasp.Poscar.get_interatomic_distances
   tepkit.io.vasp.Poscar.get_neighbor_distances
   tepkit.io.vasp.Poscar.get_atomic_numbers
   tepkit.io.vasp.Poscar.get_pymatgen_poscar
   tepkit.io.vasp.Poscar.to_supercell




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



.. py:attribute:: has_species_names
   :no-index:
   :type:  bool
   :value: True



.. py:attribute:: species_names
   :no-index:
   :type:  list[str]
   :value: ['Unknown']



.. py:attribute:: ions_per_species
   :no-index:
   :type:  list[int]
   :value: [1]



.. py:attribute:: ion_coordinates_mode
   :no-index:
   :type:  VaspCoordinatesMode



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



.. py:property:: unscale_lattice
   :no-index:
   :type: NumpyArray3x3[float]



.. py:property:: ion_positions
   :no-index:
   :type: NumpyArrayNx3[float]



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



.. py:property:: species_index_per_ion
   :no-index:
   :type: list[int]


   Returns a list of species indexes for each ion.
   e.g. [0, 0, 1, 1, 2] from Bi2Se2Te



.. py:method:: get_shengbte_types() -> list[int]
   :no-index:


   Returns a list of integers for ShengBTE-CONTROL-crystal-types.
   e.g. [1, 1, 2, 2, 3] from Bi2Se2Te



.. py:property:: species_name_per_ion
   :no-index:
   :type: list[str]


   Returns a list of species names for each ion.
   e.g. ["Bi", "Bi", "Se", "Se", "Te"] from Bi2Se2Te



.. py:property:: thickness_info
   :no-index:
   :type: dict


   Returns thickness-related data.
   Such as effective thickness, van der Waals radius of edge atoms, etc.



.. py:method:: get_cartesian_ion_positions(*, threshold: float | None = None) -> NumpyArrayNx3[float]
   :no-index:


   Return the Cartesian coordinates of ions.

   :param threshold: The absolute values smaller than this value will be set to zero. (Recommended value: 1e-13)



.. py:method:: get_fractional_ion_positions() -> NumpyArrayNx3[float]
   :no-index:


   Return the fractional coordinates of ions.



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




