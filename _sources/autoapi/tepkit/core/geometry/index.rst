tepkit.core.geometry
====================

.. py:module:: tepkit.core.geometry


Attributes
----------

.. autoapisummary::

   tepkit.core.geometry.mid_line
   tepkit.core.geometry.cross_point


Classes
-------

.. toctree::
   :hidden:

   /autoapi/tepkit/core/geometry/Point2D
   /autoapi/tepkit/core/geometry/Line2D

.. autoapisummary::

   tepkit.core.geometry.Point2D
   tepkit.core.geometry.Line2D


Functions
---------

.. autoapisummary::

   tepkit.core.geometry.perpendicular_bisector
   tepkit.core.geometry.intersection_point
   tepkit.core.geometry.rotate_matrix_2d


Module Contents
---------------

.. py:function:: perpendicular_bisector(p1: Point2D, p2: Point2D) -> Line2D

   返回两点的中垂线


.. py:function:: intersection_point(l1: Line2D, l2: Line2D, decimal=15) -> Point2D | None

   返回两线的交点


.. py:data:: mid_line
   :no-index:


.. py:data:: cross_point
   :no-index:


.. py:function:: rotate_matrix_2d(degree, to_3d=False)

