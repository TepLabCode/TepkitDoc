tepkit.io.vasp.Kpoints
======================

.. toctree::
   :hidden:

   /autoapi/tepkit/io/vasp/Kpoints.Mode

.. py:class:: tepkit.io.vasp.Kpoints

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   Ref:
   - https://www.vasp.at/wiki/index.php/KPOINTS



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'KPOINTS'``", "The default name of file when use ``from_dir()`` ."
   "``comment``", "``'KPOINTS'``", "The 1st line: The comment line."





Classes
-------

.. autoapisummary::

   tepkit.io.vasp.Kpoints.Mode


Methods
-------

.. autoapisummary::

   tepkit.io.vasp.Kpoints.get_2d_bz_kpoints




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'KPOINTS'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: comment
   :no-index:
   :type:  str
   :value: 'KPOINTS'


   The 1st line: The comment line.



.. py:method:: get_2d_bz_kpoints(b_lattice, density: int = 10, edge_density: int = 15, scale: float = 1.0 + 1e-05, mode: str = 'half')
   :no-index:
   :staticmethod:




