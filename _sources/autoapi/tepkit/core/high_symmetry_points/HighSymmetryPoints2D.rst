tepkit.core.high_symmetry_points.HighSymmetryPoints2D
=====================================================

.. toctree::
   :hidden:

   /autoapi/tepkit/core/high_symmetry_points/HighSymmetryPoints2D.LatticeGammaException
   /autoapi/tepkit/core/high_symmetry_points/HighSymmetryPoints2D.GammaAngleException

.. py:class:: tepkit.core.high_symmetry_points.HighSymmetryPoints2D(b_lattice: tepkit.utils.typing_tools.NumpyArray3x3, bravais_lattice_2d=None, text_style: str = None, path_style: str = None)


   A class to manage the high symmetry points of a 2D material.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``boundary_tokens_dict``", "``None``", ""
   "``half_boundary_tokens_dict``", "``None``", "Used for get_2d_bz_kpoints() method."
   "``right_angle_precision``", "``0.001``", ""
   "``default_text_style``", "``'Setyawan2010_tex'``", ""
   "``default_path_style``", "``'Setyawan2010'``", ""
   "``path_style``", "``None``", "The style of the choices of the high symmetry paths.
   obj.path_style = Setyawan2010 / Tepkit2024"
   "``text_style``", "``None``", "The style of the names of the high symmetry points.
   obj.text_style = Setyawan2010 / Setyawan2010_tex / Tepkit2024 / Tepkit2024_tex"
   "``df``", "``None``", "obj.df = pd.DataFrame"
   "``bravais_lattice_2d``", "``None``", ""


Properties
----------

.. autoapisummary::

   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.lattice_gamma_type



Exceptions
----------

.. autoapisummary::

   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.LatticeGammaException
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.GammaAngleException




Methods
-------

.. autoapisummary::

   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.from_poscar
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.add_token_texts
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_gamma_angle_type
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_boundary_tokens
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_boundary_df
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_paths_tokens
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_paths_df
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_df_by_tokens
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_dict
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_list
   tepkit.core.high_symmetry_points.HighSymmetryPoints2D.get_texts




All Members
-----------


.. py:attribute:: boundary_tokens_dict
   :no-index:



.. py:attribute:: half_boundary_tokens_dict
   :no-index:


   Used for get_2d_bz_kpoints() method.



.. py:attribute:: right_angle_precision
   :no-index:
   :value: 0.001



.. py:attribute:: default_text_style
   :no-index:
   :value: 'Setyawan2010_tex'



.. py:attribute:: default_path_style
   :no-index:
   :value: 'Setyawan2010'



.. py:attribute:: path_style
   :no-index:


   The style of the choices of the high symmetry paths.
   obj.path_style = Setyawan2010 / Tepkit2024



.. py:attribute:: text_style
   :no-index:


   The style of the names of the high symmetry points.
   obj.text_style = Setyawan2010 / Setyawan2010_tex / Tepkit2024 / Tepkit2024_tex



.. py:attribute:: df
   :no-index:


   obj.df = pd.DataFrame



.. py:attribute:: bravais_lattice_2d
   :no-index:
   :type:  tepkit.core.symmetry.BravaisLattice2D



.. py:property:: lattice_gamma_type
   :no-index:



.. py:method:: from_poscar(poscar, with_2pi: bool = True, text_style: str = None, path_style: str = None)
   :no-index:
   :classmethod:


   Instantiation a Plotter by a Poscar.



.. py:method:: add_token_texts()
   :no-index:



.. py:method:: get_gamma_angle_type()
   :no-index:


   计算倒晶格 gamma 角的类型



.. py:method:: get_boundary_tokens(mode='full') -> list[str]
   :no-index:



.. py:method:: get_boundary_df(mode='full')
   :no-index:



.. py:method:: get_paths_tokens() -> list[list[str]]
   :no-index:


   根据晶格类型和角度的组合自动获取高对称路径数据。
   :return: e.g. [["G", "D1", "B", "C2B", "C2", "G"]]



.. py:method:: get_paths_df()
   :no-index:



.. py:method:: get_df_by_tokens(tokens: list[str] | None = None)
   :no-index:



.. py:method:: get_dict(key_column: str = None, value_column: str = None, tokens: list[str] = None) -> dict
   :no-index:



.. py:method:: get_list(column=None, tokens=None) -> list
   :no-index:



.. py:method:: get_texts(tokens)
   :no-index:




