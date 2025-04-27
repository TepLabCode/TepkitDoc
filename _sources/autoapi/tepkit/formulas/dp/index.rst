tepkit.formulas.dp
==================

.. py:module:: tepkit.formulas.dp

.. autoapi-nested-parse::

   This module contains the formulas related to **deformation potential** theory.



Functions
---------

.. autoapisummary::

   tepkit.formulas.dp.carrier_mobility_3d_i
   tepkit.formulas.dp.carrier_mobility_2d_i
   tepkit.formulas.dp.carrier_mobility_2d_v
   tepkit.formulas.dp.relaxtion_time


Module Contents
---------------

.. py:function:: carrier_mobility_3d_i(*, c_i, e1_i, m_i, t, method='dp_3d')

   Get carrier mobility **component** :math:`\mu_i` by deformation potential theory for **bulk** materials.

   ========== =========== =====================
   Argument   Unit        Explanation
   ========== =========== =====================
   **Input**  —           —
   ``c``      GPa         Elastic constants
   ``e1``     eV          Deformation Potential
   ``m``      m_0         Effective Mass
   ``t``      K           Absolute Temperature
   **Output** —           —
   ``mu``     cm²·s⁻¹·V⁻¹ Carrier Mobility
   ========== =========== =====================

   Formula
   =======

   Ref: `Link Deformation Potentials and Mobilities in Non-Polar Crystals | Phys. Rev.
   <https://journals.aps.org/pr/abstract/10.1103/PhysRev.80.72>`_

   **Formula A.39:**

   .. math:: \mu_i = \frac{2 (2\pi)^{1/2} e \hbar^4 C_{ii}}{3 {m_i}^{5/2} (k_\mathrm{B} T)^{3/2} {E_1}_i^2}



.. py:function:: carrier_mobility_2d_i(*, c_i, e1_i, m_i, c_j, e1_j, m_j, t, method='dp_2d')

   Get carrier mobility **component** :math:`\mu_i` by deformation potential theory for **2D** materials.

   ========== =========== =====================
   Argument   Unit        Explanation
   ========== =========== =====================
   **Input**  —           —
   ``c``      N/m         2D Elastic constants
   ``e1``     eV          Deformation Potential
   ``m``      m_0         Effective Mass
   ``t``      K           Absolute Temperature
   **Output** —           —
   ``mu``     cm²·s⁻¹·V⁻¹ Carrier Mobility
   ========== =========== =====================

   Formula
   =======

   Ref: `Mobility anisotropy of two-dimensional semiconductors | Phys. Rev. B
   <https://journals.aps.org/prb/abstract/10.1103/PhysRevB.94.235306>`_

   You can choose from three different methods by ``method`` argument.

   - ``dp_2d`` (See Ref. Formula **33**) (Default)
       The most widely used version of the deformation potential theory for 2D materials.

       .. math::

           \mu_i = \frac
           {e \hbar^3 C^\mathrm{(2D)}_{ii}}
           { (k_{\mathrm{B}} T) (m_i)^{\frac{3}{2}} (m_j)^{\frac{1}{2}} {(E_1)}_i^2} \\

   - ``lang``  (See Ref. Formula **26**) (Recommended)
       The modified version from Haifeng Lang that better accounts for anisotropy.

       .. math::

           \mu_i = \frac {e \hbar^3}
           {
               (k_{\mathrm{B}} T) (m_i)^{\frac{3}{2}} (m_j)^{\frac{1}{2}}
           }
           \cdot F_{\mathrm{ani}} (E_1)
           \cdot F_{\mathrm{ani}} (C^{\mathrm{(2D)}})

   - ``lang_simplified``  (See Ref. Formula **27**)
       The low order approximation of the above formula.

       .. math::

           \mu_i = \frac {e \hbar^3}
           {
               (k_{\mathrm{B}} T) (m_i)^{\frac{3}{2}} (m_j)^{\frac{1}{2}}
           }
           \cdot \left( \frac{9 E_{1i}^2 + 7 E_{1i} E_{1j} + 4 E_{1j}^2} {20} \right)^{-1}
           \cdot \left( \frac{5 C^{\mathrm{(2D)}}_{ii} + 3 C^{\mathrm{(2D)}}_{jj} } {8} \right)



.. py:function:: carrier_mobility_2d_v(*, c_i, e1_i, m_i, c_j, e1_j, m_j, t, method='dp_2d')

   Get carrier mobility 2D **vector** :math:`(\mu_i, \mu_j)` by deformation potential theory for **2D** materials.


.. py:function:: relaxtion_time(mu, m, unit: dict = None)

   Get carrier relaxtion time :math:`\tau` by carrier mobility and effective mass.

   ========== =========== =====================
   Argument   Unit        Explanation
   ========== =========== =====================
   **Input**  —           —
   ``mu``     cm²·s⁻¹·V⁻¹ Carrier Mobility
   ``m``      m_0         Effective Mass
   **Output** —           —
   ``tau``    s or fs     Relaxation Time
   ========== =========== =====================

   Formula
   =======
   .. math:: \tau = \mu * m / e



