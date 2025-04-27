tepkit.io.shengbte.Control
==========================

.. py:class:: tepkit.io.shengbte.Control

   Bases: :py:obj:`tepkit.io.StructuredTextFile`



   For ShengBTE input file ``CONTROL`` .

   Supported Files
   ===============
   - CONTROL



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_file_name``", "``'CONTROL'``", "The default name of file when use ``from_dir()`` ."
   "``data``", "``None``", ""


Properties
----------

.. autoapisummary::

   tepkit.io.shengbte.Control.scell
   tepkit.io.shengbte.Control.ngrid
   tepkit.io.shengbte.Control.temperature
   tepkit.io.shengbte.Control.namelist
   tepkit.io.shengbte.Control.temperatures





Methods
-------

.. autoapisummary::

   tepkit.io.shengbte.Control.from_poscar
   tepkit.io.shengbte.Control.__str__
   tepkit.io.shengbte.Control.write




All Members
-----------


.. py:attribute:: default_file_name
   :no-index:
   :value: 'CONTROL'


   The default name of file when use ``from_dir()`` .



.. py:attribute:: data
   :no-index:



.. py:property:: scell
   :no-index:



.. py:property:: ngrid
   :no-index:



.. py:property:: temperature
   :no-index:



.. py:method:: from_poscar(path) -> Self
   :no-index:
   :classmethod:



.. py:property:: namelist
   :no-index:



.. py:method:: __str__()
   :no-index:



.. py:method:: write(path='./CONTROL.nml', force=True)
   :no-index:



.. py:property:: temperatures
   :no-index:




