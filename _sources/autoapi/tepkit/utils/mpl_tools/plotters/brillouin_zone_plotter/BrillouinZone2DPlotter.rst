tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter
=============================================================================

.. py:class:: tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter(b_lattice: tepkit.utils.typing_tools.NumpyArray3x3, bravais_lattice_2d: tepkit.core.symmetry.BravaisLattice2D | None = None)

   Bases: :py:obj:`tepkit.utils.mpl_tools.plotters.plotter.Plotter`



   绘制二维布里渊区的类。
   可以绘制二维布里渊区的边界、高对称点、高对称路径、基矢量等。



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``b_lattice``", "``None``", ""
   "``bravais_lattice_2d``", "``None``", ""
   "``boundary_data``", "``None``", ""
   "``data``", "``None``", ""
   "``config``", "``None``", ""
   "``hsps``", "``None``", ""
   "``plot_boundary_step``", "``True``", ""
   "``plot_path_step``", "``True``", ""
   "``plot_point_step``", "``True``", ""
   "``plot_point_text_step``", "``True``", ""
   "``plot_base_vectors_step``", "``True``", ""
   "``base_vectors_length``", "``1.0``", ""






Methods
-------

.. autoapisummary::

   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.from_poscar
   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.plot
   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.plot_boundary
   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.plot_path
   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.plot_point
   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.plot_point_text
   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.plot_base_vectors
   tepkit.utils.mpl_tools.plotters.brillouin_zone_plotter.BrillouinZone2DPlotter.to_png




All Members
-----------


.. py:attribute:: b_lattice
   :no-index:
   :type:  NumpyArray3x3



.. py:attribute:: bravais_lattice_2d
   :no-index:
   :type:  tepkit.core.symmetry.BravaisLattice2D | None



.. py:attribute:: boundary_data
   :no-index:



.. py:attribute:: data
   :no-index:



.. py:attribute:: config
   :no-index:
   :type:  dict



.. py:attribute:: hsps
   :no-index:



.. py:attribute:: plot_boundary_step
   :no-index:
   :value: True



.. py:attribute:: plot_path_step
   :no-index:
   :value: True



.. py:attribute:: plot_point_step
   :no-index:
   :value: True



.. py:attribute:: plot_point_text_step
   :no-index:
   :value: True



.. py:attribute:: plot_base_vectors_step
   :no-index:
   :value: True



.. py:attribute:: base_vectors_length
   :no-index:
   :value: 1.0



.. py:method:: from_poscar(poscar: tepkit.io.vasp.Poscar, with_2pi: bool = True, bravais_lattice_2d=None, sym_prec=1e-05)
   :no-index:
   :classmethod:


   Instantiation a Plotter by a Poscar.



.. py:method:: plot(ax)
   :no-index:



.. py:method:: plot_boundary(ax)
   :no-index:


   Plot the boundary of the first Brillouin zone.



.. py:method:: plot_path(ax)
   :no-index:


   Plot the high-symmetriy paths.



.. py:method:: plot_point(ax)
   :no-index:


   Plot the high-symmetriy points.



.. py:method:: plot_point_text(ax)
   :no-index:


   Plot the name of the high-symmetriy points.



.. py:method:: plot_base_vectors(ax, length=None)
   :no-index:


   Plot the base vectors of the reciprocal lattice as arrows with dashed lines and green color.



.. py:method:: to_png()
   :no-index:




