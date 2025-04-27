tepkit.io
=========

.. py:module:: tepkit.io

.. autoapi-nested-parse::

   This package is used to read and write files of various formats.



Submodules
----------

.. toctree::
   :maxdepth: 1

   /autoapi/tepkit/io/boltztrap2/index
   /autoapi/tepkit/io/indices/index
   /autoapi/tepkit/io/output/index
   /autoapi/tepkit/io/phonopy/index
   /autoapi/tepkit/io/shengbte/index
   /autoapi/tepkit/io/vasp/index


Attributes
----------

.. autoapisummary::

   tepkit.io.PathLike
   tepkit.io.Self


Classes
-------

.. toctree::
   :hidden:

   /autoapi/tepkit/io/File
   /autoapi/tepkit/io/TextFile
   /autoapi/tepkit/io/StructuredTextFile
   /autoapi/tepkit/io/TableTextFile

.. autoapisummary::

   tepkit.io.File
   tepkit.io.TextFile
   tepkit.io.StructuredTextFile
   tepkit.io.TableTextFile


Functions
---------

.. autoapisummary::

   tepkit.io.array_to_string
   tepkit.io.matrix_to_string


Package Contents
----------------

.. py:data:: PathLike
   :no-index:


.. py:data:: Self
   :no-index:
   :type:  TypeAlias
   :value: Self


.. py:function:: array_to_string(array, fmt='% f', delimiter=' ', prefix='', suffix='') -> str

.. py:function:: matrix_to_string(matrix, fmt='% f', delimiter=' ', line_prefix='', line_separator='\n', line_suffix='', prefix='', suffix='') -> str

