tepkit.io.boltztrap2.Condtens
=============================

.. py:class:: tepkit.io.boltztrap2.Condtens

   Bases: :py:obj:`tepkit.io.TableTextFile`



   The class for text files.
   The base class for `StructuredTextFile` and `TableTextFile` .



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'interpolation.condtens'``", "The default name of file when use ``from_dir()`` ."
   "``column_indices``", "``None``", ""
   "``default_from_file_config``", "``None``", ""
   "``label_texts``", "``None``", "You can change it to determine how to display the axis label."
   "``df``", "``None``", ""
   "``column_indices_dict``", "``None``", ""






Methods
-------

.. autoapisummary::

   tepkit.io.boltztrap2.Condtens.get_index
   tepkit.io.boltztrap2.Condtens.get_ts
   tepkit.io.boltztrap2.Condtens.get_carrier_type_conditions
   tepkit.io.boltztrap2.Condtens.effective_thickness_correction
   tepkit.io.boltztrap2.Condtens.add_relaxation_time
   tepkit.io.boltztrap2.Condtens.add_kappal
   tepkit.io.boltztrap2.Condtens.add_kappal_from_shengbte
   tepkit.io.boltztrap2.Condtens.calculate_carrier_density
   tepkit.io.boltztrap2.Condtens.calculate_average_effective_mass
   tepkit.io.boltztrap2.Condtens.multiply_relaxation_time
   tepkit.io.boltztrap2.Condtens.calculate_zt
   tepkit.io.boltztrap2.Condtens.plot
   tepkit.io.boltztrap2.Condtens.get_label_text




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'interpolation.condtens'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: column_indices
   :no-index:



.. py:attribute:: default_from_file_config
   :no-index:



.. py:attribute:: label_texts
   :no-index:


   You can change it to determine how to display the axis label.



.. py:attribute:: df
   :no-index:
   :type:  pandas.DataFrame



.. py:attribute:: column_indices_dict
   :no-index:



.. py:method:: get_index(quantity: str, direction: str = None, unit: str = None)
   :no-index:



.. py:method:: get_ts(df=None) -> list[int]
   :no-index:


   temperatures



.. py:method:: get_carrier_type_conditions(df=None)
   :no-index:



.. py:method:: effective_thickness_correction(proportion: float) -> None
   :no-index:



.. py:method:: add_relaxation_time(value: float, value_t: float, direction: str, carrier_type: str, with_inverse_proportion: bool = False) -> None
   :no-index:


   Add relaxation time (tau) to the dataframe.

   :param value: the relaxation time value in fs.
   :param value_t: the temperature of the relaxation time.
   :param direction: the direction of the relaxation time.
   :param carrier_type: the carrier type of the relaxation time. ["h", "e"]
   :param with_inverse_proportion: if True, it will assume that τ ∝ 1/T,
                                   the relaxation time at all temperatures will be autofilled by
                                   value * value_t / target_t.

   Example
   =======

   .. code-block:: python

       for t in obj.get_ts():
           obj.add_relaxation_time(
               value=time_at_300k * 300 / t,
               t=t,
               direction="x",
               carrier_type="h",
           )




.. py:method:: add_kappal(value: float, value_t: float, direction: str, with_inverse_proportion: bool = False, etc_applied: bool = False) -> None
   :no-index:


   Add lattice thermal conductivity (kappal) to the dataframe.

   :param value: the kappal value in W/(m·K).
   :param value_t: the temperature of the kappal.
   :param direction: the direction of the kappal.
   :param with_inverse_proportion: if True, it will assume that κ_l ∝ 1/T,
                                   the kappal at all temperatures will be autofilled by
                                   value * value_t / target_t.
   :param etc_applied: if True, it means that the effective thickness correction
                                   has been done to the input kappal.
   :return:



.. py:method:: add_kappal_from_shengbte(kappal: tepkit.io.shengbte.KappaTensorVsT) -> None
   :no-index:



.. py:method:: calculate_carrier_density(lattice, *, dimension: int, abs_density: bool = True)
   :no-index:


   :param lattice: Unit: Angstrom.
   :param dimension:
   :param abs_density:
   :return:



.. py:method:: calculate_average_effective_mass(mass_unit: str, *, volume: float, _absolute: bool = True)
   :no-index:


   Calculate the DOS average effective mass.
   Add the columns ("m_eff", mass_unit, direction) to the self.df.

   Ref:
   - Hautier, G., et al. (2014). Chemistry of Materials, 26(19), 5447-5458.
   - Hautier, G., et al. (2013). Nature Communications, 4, 2292.

   :param mass_unit: Should be "kg", "g", or "m_e".
   :param volume: The volume of the cell. (Unit: m^3)
   :param _absolute: If False, the sign of the effective mass will be consistent with the `N`,
                     which means negative for electrons, and positive for holes.



.. py:method:: multiply_relaxation_time(drop_tau: bool = False, get_pf: float = True)
   :no-index:


   Get multiply the relaxation time to the sigma and kappae.

   :param drop_tau: If True, it will drop the tau, sigma/tau, and kappae/tau columns.
   :param get_pf: If True, it will also calculate the power factor.



.. py:method:: calculate_zt()
   :no-index:



.. py:method:: plot(ax, x: str, y: str, t: float, x_unit: str = None, y_unit: str = None, x_direction: str = None, y_direction: str = None, carrier_type: str = None, **plot_kwargs)
   :no-index:



.. py:method:: get_label_text(text: str) -> str
   :no-index:




