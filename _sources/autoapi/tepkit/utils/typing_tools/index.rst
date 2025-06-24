tepkit.utils.typing_tools
=========================

.. py:module:: tepkit.utils.typing_tools


Attributes
----------

.. autoapisummary::

   tepkit.utils.typing_tools.Self
   tepkit.utils.typing_tools.PathLike
   tepkit.utils.typing_tools.DataType
   tepkit.utils.typing_tools.NumpyArray
   tepkit.utils.typing_tools.NumpyArray3
   tepkit.utils.typing_tools.NumpyArray2D
   tepkit.utils.typing_tools.NumpyArray3x3
   tepkit.utils.typing_tools.NumpyArrayNx3
   tepkit.utils.typing_tools.NumpyArrayNxN
   tepkit.utils.typing_tools.AutoValue


Classes
-------

.. toctree::
   :hidden:

   /autoapi/tepkit/utils/typing_tools/AutoClass

.. autoapisummary::

   tepkit.utils.typing_tools.AutoClass


Module Contents
---------------

.. py:data:: Self
   :no-index:
   :type:  TypeAlias
   :value: Self


.. py:data:: PathLike
   :no-index:


.. py:data:: DataType
   :no-index:


.. py:data:: NumpyArray
   :no-index:
   :type:  TypeAlias
   :value: np.ndarray[Any, np.dtype[DataType]]


.. py:data:: NumpyArray3
   :no-index:
   :type:  TypeAlias
   :value: np.ndarray[(Literal[3], ), np.dtype[DataType]]


.. py:data:: NumpyArray2D
   :no-index:
   :type:  TypeAlias
   :value: np.ndarray[(Any, Any), np.dtype[DataType]]


.. py:data:: NumpyArray3x3
   :no-index:
   :type:  TypeAlias
   :value: np.ndarray[(Literal[3], Literal[3]), np.dtype[DataType]]


.. py:data:: NumpyArrayNx3
   :no-index:
   :type:  TypeAlias
   :value: np.ndarray[(Literal['N'], Literal[3]), np.dtype[DataType]]


.. py:data:: NumpyArrayNxN
   :no-index:
   :type:  TypeAlias
   :value: np.ndarray[(Literal['N'], Literal['N']), np.dtype[DataType]]


.. py:data:: AutoValue
   :no-index:


