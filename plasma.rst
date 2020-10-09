The Mechanics of Plasma
=======================

Particle Orbit Theory
---------------------

| At a first glance, treating the individual particles of a plasma seems
  an inefficient way to develop understanding of plasmas, but it is in
  fact the essential underlying physics of the entire theory of plasmas.
  Orbit theory is only valid with high-energy, low density plasmas with
  infrequent collisions. We also need symmetric external fields.
| In this section it is assumed that radiative effects are negligible,
  and that particle energies are low enough that we need only consider
  the non-relativistic Lorentz equation, for a particle of mass
  :math:`m_j`, and charge :math:`q_j` at a position :math:`\vec{r}` in
  an electric field :math:`\vec{E}(\vec{r}, t)`, and magnetic field
  :math:`\vec{B}(\vec{r}, t)`,

  .. math::

     \label{eq:lorentzeq}
       m_j \dv[2]{\vec{r}_j}{t} = q_j \qty[ \vec{E}(\vec{r},t) + \dot{\vec{r}_j} \times \vec{B}(\vec{r}, t) ]

   Whenever charge distributions or current densities are signifigant a
  statistical or fluid approach will be required.

Constant Homogeneous Magnetic Field
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Let us start with a static description,
:math:`\vec{E} = 0, \vec{B}(\vec{r},
t) = B \neq 0`. Taking the direction of :math:`\vec{B}` to define the
:math:`z`-axis, so :math:`\vec{B} = (0,0,B)`, we have the scalar product
of :math:`\hat{z}` and the Lorentz equation, equation ([eq:lorentzeq])
giving

.. math::

   \label{eq:no-z-accel}
     \ddot{z} = 0

 implying that :math:`\dot{z} = v_{\parallel}` is constant. Likewise,
:math:`m
\ddot{\vec{r}} \cdot \dot{\vec{r}} = 0`, so
:math:`\half m \dot{\vec{r}}^2` is constant. We can now find, by taking
dot products of the unit vectors with equation ([eq:lorentzeq]), that

.. math::

   \begin{aligned}
     \dv{\vec{v}_z}{t}                & = 0                                                            \\
     \dv{\vec{v}_x}{t}                & = -\frac{q B \vec{v}_y}{m}                                     \\
     \dv{\vec{v}_y}{t}                & = - \frac{q B \vec{v}_x}{m}\end{aligned}

 We now have a number of conditions which simlify the system, so, from
equation ([eq:lorentzeq]),

.. math:: \dv{\vec{v}}{t} = \frac{q}{m} \vec{v} \times \vec{B}

 and since :math:`\vec{v}_z = {\rm const}`,

.. math:: \vec{z} - \vec{z}_0 = \vec{v}_{z0}t

 The :math:`x` and :math:`y` motions are more complicated;

.. math::

   \begin{aligned}
     \dv[2]{\vec{v}_x}{t}             & = \frac{qB}{m} \dv{v_y}{t}                                                                      \\
                                      & = - \qty( \frac{q B}{m})^2 v_x                                                                  \\
     \ddot{\vec{v}}_x                 & = - \omega_{\rm c}^2 \vec{v}_x                                                                  \\
     v_x                              & = v_{x0} \exp( \pm i \omega_{\rm c} t + i \phi_x)                                               \\
     \Re(v_x)                         & = v_{x0} \cos( \omega_{\rm c} t)\end{aligned}

.. math::

   \begin{aligned}
     \dv[2]{v_y}{t}                   & = - \qty(\frac{qB}{m})^2 v_y                                                                    \\
     v_y                              & = \frac{m}{qB} \dv{v_x}{t}                                                                      \\
                                      & = - \frac{m}{qB} v_{x0} \sin( \omega_{\rm c} t) \omega_{\rm c}                                  \\
                                      & = \mp v_{x0} \sin( \omega_{\rm c} t )                                                           \\
                        \end{aligned}

Before proceeding, we’ll make the definition of the *Larmour Radius*,

The Larmour radius, :math:`r_{\rm L}` (also gyroradius, or cyclotron
radius) is the radius of the circular motion of a charged particle in a
uniform magnetic field.

.. math:: r_{\rm L} = \frac{m v_{\perp}}{|q|B}

We can now find the full equations of motion by considering

.. math::

   \begin{aligned}
     \nonumber
                        v_x^2 + v_y^2 & = v_{x0}^2 \qty( \cos[2](\omega_{\rm c} t) + \sin[2]({\omega_{\rm c}t}) ) = v_{x0}^2 = v_{\perp}^2 \\ \nonumber
     \vec{v}                          & = (v_{\parallel}, v_{\perp})                                                              \\ 
     x - x_0                          & = \frac{v_{\perp}}{\omega_{\rm c}} \sin(\omega_{\rm c}t)     = r_{\rm L} \sin(\omega_{\rm c} t)  \\
     y - y_0                          & = \frac{\mp v_{\perp}}{\omega_{\rm c}} \cos(\omega_{\rm c}t)   =\mp r_{\rm L} \cos(\omega_{\rm c} t)  \\ 
     z - z_0 &= v_{z0} t = v_{\parallel} t \\
   \nonumber
   \text{since }  \frac{v_{\perp}}{\omega_{\rm c}}    & = \frac{v_{\perp}m}{|q|B} \equiv
     r_L\end{aligned}

Constant Homogeneous Magnetic and Electric Fields
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Now let’s elaborate to a situation which involves an electric field. We
now have, from equation ([eq:lorentzeq]),

.. math:: m \dv{\vec{v}}{t} = q\vec{E} + q \vec{v} \times \vec{B}

 and take the inner product of this with the velocity,

.. math::

   \begin{aligned}
   \nonumber m\vec{v}\cdot \dv{\vec{v}}{t}             & = q \vec{v} \cdot \vec{E} + 0                 \\
   \nonumber \dv{t} \qty(\frac{mv^2}{2})          & = q \vec{v} \cdot \vec{E}                     \\
   \nonumber                                      & = - q \vec{v} \nabla \phi                     \\
   \nonumber                                      & = -q \dv{\vec{r}}{t} \cdot \dv{\phi}{\vec{r}} \\
   \nonumber                                      & = -q \dv{\phi}{t}                             \\
   \nonumber  \dv{t} \qty[ \frac{mv^2}{2}+q \phi] & = 0 \end{aligned}

Now we arrange our coordinates such that :math:`\vec{B}=(0,0, B_z)`, and
:math:`\vec{E} = (E_x, 0, E_z)`, so

.. math::

   \begin{aligned}
   \dv{v_z}{t} & = \frac{q}{m} E_z                                              \\
   \dv{v_x}{t} & = \frac{q}{m} E_x + \frac{qB_z}{m} v_y                         \\
   \dv{v_y}{t} & = - \frac{qB}{m} v_x \end{aligned}

The gyrocentre will shift, but to understand how we must solve these
equations. To do this we take a similar approach to the last lecture.

.. math::

   \begin{aligned}
   \ddot{v}_x  & = 0 + \frac{qB}{m} \dot{v}_y                                   \\
               & = - \qty(\frac{qB}{m})^2 v_x                                   \\
               & = - \omega_{\rm c}^2 v_x                                       \\
   \ddot{v}_y  & = -\omega_{\rm c} \dot{v}_x                                    \\
               & = - \frac{qB}{m} \qty( \frac{q}{m} E_x + \frac{qB}{m} v_y )    \\
               & = -\omega_{\rm c}^2 \qty( v_y + \frac{q}{m} \frac{m}{qB} E_x ) \\
               & = - \omega_{\rm c}^2 \qty( v_y + \frac{E_x}{B} )               \\
   \dv[2]{t}\qty( v_y + \frac{E_x}{B} ) &= - \omega_{\rm c}^2 \qty( v_y + \frac{E_x}{B} ) \end{aligned}

 Then, at :math:`t=0`, :math:`v_x = v_{x0}`, and :math:`v_y=0`,

.. math::

   \begin{aligned}
   v_x &= v_{x0} \cos(\omega_{\rm c} t) \\
   v_y &= \mp v_{x0} \sin(\omega_{\rm c}) - \frac{E_x}{B} \end{aligned}

Let’s take an alternative approach here, and work entirely with vectors
again, so first,

.. math::

   \begin{aligned}
   \vec{B} \times m \dv{\vec{v}}{t} &= \vec{B} \times \qty(q \vec{E} + q \vec{v} \times \vec{B})  \nonumber \\
   q \vec{B} \times \vec{E} + q \vec{B} \times \qty( \vec{v} \times \vec{B}) &= 0  \nonumber \\
   q \vec{B} \times \vec{E} + q \qty(\vec{v} \cdot B^2 - \vec{B} \qty( \vec{v} \cdot \vec{B})) &= 0  \nonumber\\
   \vec{v}_{\rm ge} B^2 &= \vec{E} \times \vec{B}  \nonumber\\
   \vec{v}_{\rm ge} &= \frac{\vec{E} \times \vec{B}}{B^2} \end{aligned}

with :math:`v_{\rm ge}` the velocity of the guiding centre.

Drift in an external field
~~~~~~~~~~~~~~~~~~~~~~~~~~

As a result of this drift, the movement of a particle in this situation
can be described by

.. math::

   \begin{aligned}
     \label{eq:1}
     \vec{v} &= \vec{u} + \vec{v}_{\rm ge} \\
   m \dv{\vec{v}}{t} &= q\vec{E} + q \vec{v} \times \vec{B} \\
   \dv{\vec{v}}{t} &= \dv{\vec{u}}{t} + \dv{\vec{v}_{\rm ge}}{t} \\
   m \dv{\vec{v}}{t} &= m \dv{\vec{u}}{t} \\ &= q \vec{E} + q \qty( \vec{u} + \vec{v}_{\rm ge}) \times \vec{B}\\
   &= q \vec{E} + q \vec{u} \times \vec{B} + q \vec{v}_{\rm ge} \times \vec{B} \\
   m \dv{u_{\parallel}}{t} &= q E_{\parallel} \\
   m \dv{v_{\rm ge}}{t} &= q \vec{u}_{\perp} \times \vec{B} \\
   \vec{u} &= u_{\parallel} \frac{\vec{B}}{|B|} + \vec{u}_{\perp} + \vec{v}_{\rm ge} \\
   m \dv{\vec{v}}{t} &= \vec{F}_{\rm ext} + q \vec{v} \times \vec{B} \\
   \vec{v}_{\rm F} &= \frac{1}{q} \frac{\vec{F} \times \vec{B}}{B^2} \\
   \vec{v}_{\rm g} &= \frac{m}{q} \frac{\vec{g} \times \vec{B}}{B^2}\end{aligned}

Now, suppose we have a non-uniform field which varies weakly, that is,

.. math:: \nabla \cdot \vec{B} \sim \frac{B}{L}

for :math:`L \gg r_{\rm L}`. Again, we set up our coordinates so
:math:`\vec{B} = (0,0, B)`, then we have

.. math::

   \begin{aligned}
     \langle \vec{F} \rangle &= \frac{1}{T} \int_0^T F(t) \dd{t} \\
   F &= q \vec{v} \times \vec{B} = \hat{\imath} v_y B - \hat{\jmath} v_x B + \hat{k} \cdot 0 \\
   \vec{B}(\vec{R}_{\rm v}+\vec{r}) &= \vec{B}_0 + ( \vec{r} \nabla ) \vec{B} + \cdots \\
   B &= B_0 + (\vec{r} \nabla) B \\
   B &= B_0 + y \cdot \pdv{y} B \\
   F_x &= q v_y B \\
   &= q v_y (B_{0z} +y \pdv{y}B) \\
   F_y &= -q v_x B \\ &= q v_x ( B_{0z} + y \pdv{B}{y} )\end{aligned}

 Now, using the results from earlier, for the unperturbed situations,

.. math::

   \begin{aligned}
     F_x &= \mp q v_{x0} \sin( \omega_{\rm c} t ) \qty( B_{0z} \pm \frac{v_{x0}}{\omega_{\rm c}} \cos(\omega_{\rm c} t) \pdv{B}{y} ) \\
   F_y &= - q v_{x0} \cos( \omega_{\rm c} t) \qty( B_{0z} \pm \frac{v_{x0}}{\omega_{\rm c}} \cos(\omega_{\rm c} t) \pdv{B_z}{y} )\end{aligned}

 Then, knowing,

.. math::

   \begin{aligned}
     \langle \sin(\omega_{\rm c}t) \rangle &= 0 \\
   \langle \cos(\omega_{\rm c}t) \rangle &= 0 \\
   \langle \sin(\omega_{\rm c} t) \cos( \omega_{\rm c} t) \rangle &= 0 \\
   \langle \cos(\omega_{\rm c} t) \cos( \omega_{\rm c} t) \rangle &= \half \end{aligned}

 so

.. math::

   \begin{aligned}
     \langle F_x \rangle &= 0 \\
   \langle F_y \rangle &= -q \frac{v_{x0}^2}{\omega_{\rm c}} \langle \cos[2](\omega_{\rm c}t) \rangle \pdv{B}{y} \\
   &= \mp q \frac{v_{\perp}^2}{2 \omega_{\rm c}} \pdv{B}{y} \\
   \langle F \rangle &= \mp q \frac{v_{\perp}^2}{2 \omega_{\rm c}} \nabla |\vec{B}| \\
   v_{\rm ge} &= \frac{1}{q} \mp q \frac{v_{\perp}^2}{2 \omega_{\rm c}} \frac{\nabla |\vec{B}| \times \vec{B}}{B^2} \\
   &= \pm \frac{v_{\perp}^2}{2 \omega_{\rm c}} \frac{\vec{B} \times \nabla|\vec{B}|}{B^2}\end{aligned}

Inhomogeneous Magnetic Fields
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In practice magnetic fields are rarely uniform, but are generally space-
and time-dependent. Normally this would lead to a numerical treatment
being required, but there are cases where it is possible to calculate
the variation analytically, by assuming the inhomogeneity to be small.

First, consider the case when a particle moves only parallel to the
magnetic field lines. The central force experienced by the particle will
be

.. math::

   \label{eq:centralforceinhommag}
     \vec{F}_{\rm cent} = \frac{m v_{\parallel}^2}{R_{\rm c}} \hat{R}_{\rm c}

 with :math:`R_{\rm c}` being the radius of curvature that the particle
is moving on. Now, we introduce the quantity

.. math:: \hat{B} \cdot \nabla := \pdv{S}

 as the directional derivative along a field line, which is the rate of
change of the magnetic field along the direction :math:`\hat{B}`, so

.. math::

   \begin{aligned}
     \frac{\vec{R}_{\rm c}}{R_{\rm c}^2} &= - \pdv{S} \qty(
     \frac{\vec{B}}{B} ) \\&= - \frac{1}{B} \pdv{\vec{B}}{S} + \frac{\vec{B}}{B^2} \pdv{B}{S} \\
   &= - \frac{1}{B^2} \qty( \vec{B} \cdot \nabla) \vec{B} + \frac{\vec{B}}{B^2} \pdv{B}{S} \\\end{aligned}

 then, returning to the force equation, ([eq:centralforceinhommag]),
and, since the particle is moving along lines of constant field
strength, so that :math:`\pdv{B}{S}=0,`

.. math::

   \label{eq:centforceinhommag2}
     \vec{F}_{\rm cent} = - \frac{mv_{\parallel}^2}{B^2} (\vec{B} \cdot \nabla) \vec{B}

 and the curvature drift velocity is then

.. math::

   \begin{eq:curvedriftvelinhommag}
   \vec{v}_{\rm D} = \frac{1}{q} \frac{\vec{F}_{\rm cent} \times \vec{B}}{B^2} = \frac{m v_{\parallel}^2}{q B^4} \qty( \vec{B} \times (\vec{B} \cdot \nabla) \vec{B} )

 and

.. math::

   \label{eq:curvedriftradinhom}
   \vec{v}_{\rm R} = \frac{m v_{\parallel}^2}{q B^2} \frac{\vec{R}_{\rm c} \times \vec{B}}{R_{\rm c}^2}

 Now, in reality there is a gradient (:math:`\nabla \vec{B}`) drift
which accompanies the curvature drift, as :math:`\vec{B}` must decrease
with radius. This is because, in a vacuum we require
:math:`\nabla \times \vec{B}
= 0` (law of conservation of energy) and
:math:`\nabla \cdot \vec{B} = 0` (Gauss’s Law). Expressing the problem
in cylindrical coorinates it is trivial to see that
:math:`\nabla \times \vec{B}` can only have an :math:`z`-component. Now,

.. math:: \vec{B} = (0, B_{\theta}, 0)

 so,

.. math::

   ( \nabla \times \vec{B} )_z = \frac{1}{r} \pdv{r} (r B_{\theta}) =
   0

 and so :math:`B_{\theta}\sim\frac{1}{r}`. Hence,
:math:`B = B_{\theta} \sim
\frac{1}{R_{\rm c}}`, and,
:math:`\frac{\nabla B}{B} = - \frac{\vec{R}_{\rm
    c}}{R_{\rm c}^2}`. Using the gradient drift expression from earlier,

.. math::

   \label{eq:2}
     \vec{v}_{\nabla B} = \pm \frac{v_{\perp}^2}{\alpha \omega_{\rm c}} \frac{\vec{B} \times \nabla B}{B^2}

 and then substituting the :math:`\nabla B` due to the curvature,

.. math::

   \label{eq:3}
     \vec{v}_{\nabla B} = \pm \frac{v_{\perp}^2}{2 \omega_{\rm c}} \frac{\vec{R}_{\rm c} \times \vec{B}}{R_{\rm c}^2 B} = \half \frac{m v_{\perp}^2}{q} \frac{\vec{R}_{\rm c} \times \vec{B}}{R_{\rm c}^2 B^2}

 Then, the combined shift is

.. math::

   \label{eq:4}
     \vec{v}_{\rm D} = \vec{v}_{R} + \vec{v}_{\nabla R} = \frac{m}{q} \frac{\vec{R}_{\rm c} \times \vec{B}}{R_{\rm c}^2 B^2} \qty( v_{\parallel}^2 + \half v_{\perp}^2 )

 so the total drift due to a non-uniform field is perpendicular to both
:math:`R_{\rm c}` and :math:`\vec{B}`, and so in dipole fields we have
drift which is perpendicular to both :math:`R_{\rm c}` and
:math:`\vec{B}`, and the drift is charge-dependent, so there is a
current, which is known as the *ring current*.

Magnetic Mirroring
~~~~~~~~~~~~~~~~~~

Consider a non-uniform magnetic field, primarily in the
:math:`z`-direction, which has a magnitude which varies in the
:math:`z`-direction. Let the field be axisymmetric, such that
:math:`B_{\theta}=0`, and :math:`\pdv{\theta}\cdot
B=0`. Since the field lines converge and diverge, :math:`B_r \neq 0`.

in 1,2,3 (7,-) .. controls (3,-) and (2,-) .. (-1,-); (7,) .. controls
(3,) and (2,) .. (-1,); (-2,0) – (8,0) node [right] :math:`z`; (-1,0) –
(-1,1) node [midway, left] :math:`r`;

From :math:`\nabla \cdot \vec{B} = 0` we have

.. math:: \frac{1}{r} \pdv{r} (r B_r) + \pdv{B_z}{z} = 0

If :math:`\pdv{B_z}{z}` at :math:`r=0` is given, and doesn’t change much
with :math:`r` we have the relation

.. math::

   r B_r = - \int_0^r r \pdv{B_z}{z} \dd{r} \approx \half r^2
   \pdv{B_z}{z} \eval_{r=0}

 The variation of :math:`B` with :math:`r` causes a :math:`\nabla B`
drift of the guiding centre about the axis of symmetry, but there is no
radial :math:`\nabla B` drift, as :math:`\pdv{B}{\theta}=0`. The Lorentz
force is then

.. math::

   \label{eq:mirroringlorentz}
     \vec{F} = q
     \begin{bmatrix}
       v_{\theta} B_z - v_z B_{\theta} \\ - v_r B_z + v_z B_r \\ v_r B_{\theta} - v_{\theta} B_r
     \end{bmatrix}

 If :math:`B_{\theta}=0` two terms are equal to zero, and as
:math:`r \to 0`, :math:`B_r
\to 0`, since :math:`B_r` vanishes on the axis. When it doesn’t vanish
the azimuthal force leads to a drift in the radial direction. This drift
makes the guiding centres follow the magnetic field lines. Consider the
:math:`z`-component of ([eq:mirroringlorentz]),

.. math:: F_z = -q v_{\theta} B_r = \half q v_{\theta} r \pdv{B_z}{z}

 averaging over a gyration,

.. math::

   \ev{F_z} = \mp \half q v_{\perp} r_{\rm L} \pdv{B_z}{z} = \mp \half
   q \frac{v_{\perp}}{\omega_{\rm c}} \pdv{B_z}{z}

 Now, making a definition,

.. math:: \mu := \half \frac{m v_{\perp}^2}{B}

The force can then be written

.. math::

   \label{eq:5}
     \vec{F}_{\parallel} = - \mu \pdv{B}{S} = - \mu \nu_{\parallel} B

 Now we can consider the component of the equation of motion along
:math:`\vec{B}`,

.. math:: m \dv{v_{\parallel}}{t} = - \mu \pdv{B}{S}

 then multiplying by :math:`v_{\parallel}`,

.. math::

   \begin{aligned}
     m v_{\parallel} \pdv{v_{\parallel}}{t} &= - \mu \pdv{B}{S} v_{\parallel} \\ &= - \mu \pdv{B}{S} \cdot \dv{S}{t} \\ &= -\mu \dv{B}{t}\end{aligned}

 Here :math:`\dv{B}{t}` is the variation of :math:`B` as seen by the
particle; :math:`\vec{B}` itself is constant. Since
:math:`\frac{mv^2}{2}` is constant, due to conservation of energy, we
have

.. math::

   \dv{t} \frac{mv^2}{2} = \dv{t} \qty( \frac{mv_{\parallel}^2}{2} +
   \frac{m v_{\perp}^2}{2} ) = \dv{t} \qty( \half mv_{\perp}^2 + \mu
   B)=0

 since

.. math:: m v_{\parallel} \dv{v_{\parallel}}{t} = \dv{t} \qty( \frac{mv^2}{2} ) = - \mu \dv{B}{t}

 so

.. math::

   - \mu \dv{B}{t} + \dv{t} \qty( \mu B ) = 0 \Leftrightarrow
   \dv{\mu}{t} = 0

 and thus the magnetic moment is a conserved quantity, and is invariant
in time. This invariance allows a plasma to be confined through magnetic
mirrors.

| As the particle moves from the weak field region into the strong-field
  region, :math:`v_\perp` must increase in order that :math:`\mu` stay
  constant. Since :math:`v_\perp^2 + v_\parallel^2` is constant, it
  follows that :math:`v_\parallel` must decrease, eventually to
  :math:`0`. Eventually the particle will be reflected back towards the
  weak-field region. We can then associate a force,
  :math:`F_{\parallel}`, or the *mirror force* with this action, and the
  plasma is magnetically trapped between two magnetic mirrors.
| The trapping is not, however, perfect. If a particle has
  :math:`v_{\perp}=0` it will have no :math:`\mu`, and so will not feel
  a mirror force. As a result, at small
  :math:`\frac{v_{\perp}}{v_{\parallel}}` we expect that there will be
  some escape of particles.
| Consider a particle with :math:`v_{\parallel,0}`
  and\ :math:`v_{\perp,0}` initially in the region :math:`B_{\rm min}`.
  By conservation of :math:`\mu`,

  .. math::

     \frac{1}{2} \frac{m v_{\perp,0}^2}{B_{\rm min}} = \half \frac{m
       v_{\perp}^{\prime 2}}{B_{\rm max}}

   Then, by conservation of :math:`v_{\perp}^2 + v_{\parallel}^2`,

  .. math:: v_0^2 = v_{\perp,0}^2 + v_{\parallel,0}^2 = v_{\perp}^{\prime 2} + v_{\parallel}^{\prime 2}

   and so

  .. math::

     \frac{B_{\rm min}}{B_{\rm max}} = \frac{v_{\perp,
         0}^{2}}{v_{\perp,0}^{\prime 2}} = \frac{v_{\perp,0}}{v_0^2} =
     \sin[2](\theta)

   so

  .. math:: \sin(\theta) := \frac{v_{\perp}}{v_0}

   We can now use :math:`\theta` to describe whether the particle
  escapes from, or is trapped by, the magnetic field.

.. math::

   \label{eq:6}
     \sin[2](\theta) = 
     \begin{cases}
       < \frac{B_{\rm min}}{B_{\rm max}} & \text{escape} \\
   > \frac{B_{\rm min}}{B_{\rm max}} & \text{trapped}
     \end{cases}

Adiabatic Invariants
~~~~~~~~~~~~~~~~~~~~

In a classical system which experiences a periodic motion, the action
integral taken over one period of the motion will be constant. That is

.. math:: \oint \vec{p} \dd{\vec{q}} = \text{constant}

If a slow change occurs in the system, such that the motion is (just)
non-periodic, the constant of the motion does not change, and is called
adiabatically invariant. The slow change is qualified by a change takes
longer than one period of the underlying motion, so that the action is
well-defined (although the integral is strictly no longer a closed loop
integral).

The First Adiabatic Invariant
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The first adaibatic invariant of a plasma involves the Larmour gyration,
so

.. math::

   \label{eq:7}
     \oint \vec{p} \dd{\vec{q}} = \oint m v_{\perp} r_{\rm L} \dd{\phi} = 2 \pi m v_{\perp} r_{\rm L} = 4 \pi \frac{m}{\abs{q}} \mu

 The magnetic moment, :math:`\mu`, will be conserved when the variation
time, :math:`\Delta t` of the magnetic field, :math:`B`, is long,
i.e. \ :math:`\Delta t
\omega_{\rm c} \gg 1`. Otherwise the magnetic moment is not conserved.

The Second Adiabatic Invariant
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The second adiabatic invariant involves the periodic oscillation of
plasma particles between magnetic mirrors. This time

.. math::

   \label{eq:8}
     \oint m v_{\parallel} \dd{S} = \text{constant}

 Since the guiding centre drifts across field lines, however, the motion
is not exactly periodic, and so the motion is adiabatically invariant.
This is also longitudinally invariant :math:`J`, defined as the
half-cycle between the two mirror points, :math:`a` and :math:`b`, with

.. math:: J= \int_a^b v_{\parallel} \dd{S}

 with :math:`S` a path along a field line. :math:`J`-invariance is
violated in *transit-time magnetic pumping*, a method for heating a
plasma. This is done by moving :math:`a` and :math:`b` over time to
increase the :math:`v_{\parallel}` as the particles approach the mirror
points.

The Bulk Properties of Plasma
=============================

Plasma is the “fourth state of matter”. It refers to a state containing
enough free charges for its dynamics to be dominated by long-range
Coloumb forces, rather than shorter-range binary collisions [1]_. The
presence of charge carriers in the matter cause a plasma to interact
strongly with electromagnetic fields.

Producing a Plasma
------------------

There are a number of approaches to producing a plasma in the lab:

#. **photoionisation**—for this we need photons with sufficient energy
   to remove electrons from the neutral species, e.g. 13.6 eV for
   Hydrogen, 24.6 eV for Helium, and 15.6 eV for molecular nitrogen. All
   of these energies lie within the ultraviolet region of the
   electromagnetic spectrum. The existence of long-lived, metastable
   states can help with ionisation processes (He has two, at 19.8 eV
   (with a half-life of 700s), and 20.61 eV; :math:`{\rm H}_{2}` at
   11.75 eV (:math:`10^{-3} {\rm s}`), and H at 0.52 eV (1 month).)

#. **electron impact**—for this we accelerate any free electrons (for
   example, the seed electrons) in an electric field until they reach
   the ionising threshold. This process makes use of the Townsend
   process, where :math:`N` electrons move along the :math:`x`-axis in
   the presence of a uniform electric field, :math:`E`; then
   :math:`\delta N` electrons are produced by electron-impact ionisation
   in a distance :math:`\dif x`, according to

   .. math::

      \label{eq:townsend}
          \delta N = \alpha_{{\rm T}} N \dif{x}

    with :math:`\alpha_{{\rm T}}` being the ionisation co-efficient.
   Thus,

   .. math::

      \label{eq:townsendint}
          N(x) = N_0 \exp(\alpha_{\rm T} x)

| For this lecture course, we shall assume that the plasma is 100 %
  ionised, i.e. there shall be no plasma-neutral interaction.

Basic Physics of Plasmas
------------------------

Electrical Neutrality and the Debye Length
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Suppose we have a gas of electrons and protons, i.e. a Hydrogen plasma,
at a temperature, :math:`T`. Consider the situation where a random
fluctuation of the electron population exposes some positive particles,
thus an unbalanced positive charge. Exposing an unbalanced positve
charge will cause a net movement of negative charge (in the form of
electrons) to move towards the positive charge. What is the associated
scale length for this process; can this be made consistent with
thermodynamics?

(-2, 1) – (2, 1); (-2, -1) – (2,-1);

(-1, 1) – (-1, -1); ( 1, 1) – ( 1, -1);

(-1, 1) rectangle (1, -1); (0,0) node [text centered] Zone of depletion;
(-1.5, 1.2) node [text centered] neutral; (1.5, 1.2) node [text
centered] neutral; (0, -1.2) node [text centered] positive;

The average kinetic energy of the electrons is
:math:`E = \frac{1}{2} k_{B
}T`. The fluctuation in the electron denisty leaves behind an unbalanced
charge, and therefore an associated electric potential :math:`\phi`.
Poisson’s equation says

.. math:: \nabla^2 \phi = - \frac{ne}{\epsilon_{0}}

 with :math:`n` being the number density. So in one dimension,

.. math:: \frac{\difp{2} {\phi}}{\dif x^2} = - \frac{ne}{\epsilon_0}

 which has a solution

.. math:: \phi(x) = {\rm const} - \frac{nex^2}{2 \epsilon_0}

 Note that symmetry rules out a linear term in :math:`x`. Then we have
boundary conditions: :math:`\phi(x=\pm d) = 0`. Applying these boundary
consitions means that

.. math:: \frac{ned^2}{2\epsilon_0} = {\rm const}

; ; ;

Now recall that we want to create this region via a small thermal
fluctuation; therefore we need :math:`\frac{1}{2} k_{B}T` to be the
maximum energy of the electrons, and to be the maximum potential energy
of the well (otherwise the electrons can’t escape.) Hence
:math:`\frac{ned^2}{2\epsilon_0} e = \frac{1}{2} k_BT`, and so

.. math:: d =\left[ \frac{\epsilon_0 k_BT}{ne^2} \right]^{\frac{1}{2}} = \lambda_{\rm D}

 which is the Debye length, which is conventially denoted
:math:`\lambda_{{\rm D}}`. And this is the characteristic screening
length for unbalanced charges.

The Debye length in a plasma is the characteristic screening length for
an unbalanced charge, which is dictated by the kinetic energy of the
plasma.

.. math:: \lambda_{\rm D} = \qty[ \frac{\epsilon_0 \kbolt T}{ne^2}]^{\frac{1}{2}}

+------------------------+---------------------------------+------------------------------------------+-----------------------------------+---------------------------------+
| Plasma                 | Density (:math:`\meter^{-3}`)   | Electron temperature (:math:`\kelvin`)   | Magnetic Field (:math:`\tesla`)   | Debye Length (:math:`\meter`)   |
+========================+=================================+==========================================+===================================+=================================+
| Solar core             | :math:`10^{32}`                 | :math:`10^7`                             | -                                 | :math:`10^{-11}`                |
+------------------------+---------------------------------+------------------------------------------+-----------------------------------+---------------------------------+
| Tokamak                | :math:`10^{20}`                 | :math:`10^7`                             | 10                                | :math:`2.10 \e{-5}`             |
+------------------------+---------------------------------+------------------------------------------+-----------------------------------+---------------------------------+
| Hot interstellar gas   | :math:`10^6`                    | :math:`10^4`                             | :math:`10^{-10}`                  | :math:`10`                      |
+------------------------+---------------------------------+------------------------------------------+-----------------------------------+---------------------------------+

The plasma parameter, :math:`N`, is the number of particles of a plasma
which are contained within the Debye sphere,

.. math:: N = n \lambda_{\rm D}^3

For a good plasma we want :math:`N \gg 1`. For the tokomak,
:math:`N \approx
1\e{6}`, for the interstellar gas, :math:`N \approx 1\e{9}`. So, the
Interstellar medium’s plasma is better than the tokomak’s.

Plasma Oscillation
~~~~~~~~~~~~~~~~~~

We know that the plasma is electrically neutral over scales around the
Debye Length, so there must be a restoring force driving the restoration
of charge neutrality. This will produce oscillations about an
equilibrium point (think of a swing).

| In the simplest case is a perturbation in the electron number density,
  holding the ions stationary, and ignoring thermal effects. Here ions
  represent a perfectly balancing positive charge density, matching the
  electrons in equilibrium.
| Let the electron number density be :math:`n_{\rm e}(x,t)`, and suppose
  :math:`n_{\rm e}(x,t) = n_0 + \delta n(x,t)`; a perturbation
  consisting of a constant, :math:`n_0`, and a small fluctuating
  component, :math:`\delta
  n(x,t)`. As in any continuum, the evolution of the mass density of a
  plasma is linked to the velocity field, and is given by the density
  conservation law:

  .. math::

     \label{eq:density-conservation}
         \frac{\partial n}{\partial t} + \nabla \cdot (n_{\rm e} \vec u) = 0

   so the change in the electron density over time, plus the flux of
  particles through a volume should be zero.

(0,0) circle (3); (4,1.7) node [black, right] Flux in … – (2,1.7);
(2.5,0) – (4,0) node[black, below, right, text width=3.5cm] and Flux out
are the only ways to change the internal density.;

Now, a change in electron population or density, relative to the
equilibrium, produced by an electric field is

.. math::

   \nabla \cdot \vec{E} = \frac{\rho_{\rm f}}{\epsilon_0} = \frac{-n_{\rm
       e}e}{\epsilon_0}

with :math:`\rho_{\rm f}` the free-charge density. How do electrons
respond to the electric field? We need the fluid momentum equation,
which is a restatement of the conservation of momentum,

.. math::

   \label{eq:fluidmom}
     m \underbrace{\left[ \frac{\partial \vec{v}_{\rm e}}{\partial t} + ( \vec{v_{\rm e}} \cdot \nabla) \vec{v}_{\rm e} \right]}_{\frac{{\rm D} \vec{v}}{{\rm D}t}} = -e \vec{E}

 with :math:`\frac{{\rm D} \vec{v}}{{\rm D}t}` being the advective
derivative,

.. math::

   \frac{\rm D}{{\rm D}t} := \frac{\partial}{\partial t} + \vec{v}
   \cdot \nabla

 Let us assume that the oscillation is a small perturbation on an
otherwise stationary (and therefore electric-field free) equilibrium.

.. math:: n_{\rm e} = n_0 + \underbrace{n_1(x,t)}_{{\rm small}}

 thus

.. math:: \vec{v} = \vec{v_0}+\vec{v_1}(\vec{x},t)

 and taking :math:`v_0 = 0`,

.. math:: \vec{E} = \vec{E_0} + \vec{E_1}(\vec{x}, t)

 with :math:`E_0 = 0` since the field is in equilibrium. We an now
perturb the full equations to see how our small distribution evolves:

.. math::

   \frac{\partial n_1}{\partial t} + \nabla \cdot (n_0 \vec{v_0}) =
   0  \tag{\star}

 So the momentum equation,

.. math:: \frac{\partial \vec{v_1}}{\partial t} = - \frac{e}{m} \vec{E_1}  \tag{\star \star \star}

 and

.. math:: \nabla \cdot \vec{E_1} = - \frac{n_1 e}{\epsilon_0} \tag{\star \star}

 Now, start by :math:`\frac{\partial \star}{\partial t} `,

.. math::

   \begin{aligned}
     \frac{\partial^2 n_1}{\partial t^2} + \nabla \cdot \left( n_0 
   \frac{\partial \vec{v_1} }{\partial t} \right) &= 0 \\
   \frac{\partial^2 n_1}{\partial t^2}+ \nabla \cdot \left( n_{0} \left( - \frac{e}{m} \vec{E_1} \right)\right) &=0 \\
   \frac{\partial^2 n_1}{\partial t^2} + n_0 (- \frac{e}{m}) \nabla \vec{E_1} &= 0  \\
   \frac{\partial^2 n_1}{\partial t^2} - \frac{n_0 e}{m} (- \frac{n_1 e}{\epsilon_0}) &= 0 \quad(\text{ by } \star \star)\\
   \frac{\partial^2 n_1}{\partial t^2} + \frac{n_0e^2}{\epsilon_0 m} n_1 &= 0\end{aligned}

.. math:: \ddot{n_1} + \omega_{\rm p}^2 n_1 = 0

.. math:: \omega_{\rm p}^2 = \frac{n_0 e^2}{\epsilon_0 m}

 Which is simple harmonic motion with fixed frequency
:math:`\omega_{\rm p}`, the plasma frequency, with
:math:`\nu_{\rm p} = 9 \sqrt{n_0}`. This is an oscillation, but not a
wave.

Plasma as a dielectric
~~~~~~~~~~~~~~~~~~~~~~

The plasma oscillation has consequences for the propogation of
electromagnetic radiation. The restoring force which produces the plasma
is a direct consequence of the plasma producing a displacement current.
It turns out that we can treat the plasma as a dielectric medium, and
that we can see this by considering the plasma’s repsonse to an
oscillating imposed electric field,

.. math:: E(t) = \hat{E} e^{-i\omega t}

 the plasma responce: consider a single particle,

.. math:: m \frac{\dif{v}}{\dif{t}} = -eE = -e \hat{E} \exp({-i \omega t})

 therefore,

.. math::

   v(t) = \frac{e}{i \omega m} \hat{E} \exp(-i \omega t) = \frac{e}{i
     \omega m} E(t)

 and the plasma particles oscillate in response, but not at the same
phase. Charges in motion constitute a current, so for the current
density we can write that

.. math::

   \begin{aligned}
    \vec{j} &= -n e \vec{v} = -ne \left( \frac{e}{i \omega m} \right) \vec{E}(t) \nonumber
    \\ &= \frac{ne^2}{i \omega m}\vec{E}(t) \end{aligned}

 Recall Maxwell’s equations for a dielectric:

.. math::

   \begin{aligned}
     \nabla \times \vec{H} = \frac{\partial \vec D}{\partial t}\end{aligned}

 with :math:`\vec{D}= \epsilon_{{\rm r}} \epsilon_0 \vec{E}`, and
:math:`\epsilon_{\rm r}` the relative permittivity of the dielectric.
The full Maxwell equation reads

.. math::

   \begin{aligned}
     \nabla \times \vec{H} &= \vec{j} + \frac{\partial \vec D}{\partial t}\end{aligned}

 in the plasma, and since :math:`\vec{D} = \epsilon_0 \vec{E}`,

.. math::

   \begin{aligned}
     \nabla \times \vec{H} = - \frac{n e^2}{i \omega m} \vec{E} - i \omega \epsilon_0 \vec{E}\end{aligned}

 and so :math:`\vec{E} \propto \exp(-i \omega t)`, and so,

.. math::

   \begin{aligned}
     \nabla \times \vec{H} &= - i \omega \left[ 1 - \frac{n e^2}{\epsilon_0 m \omega^2} \right] \epsilon_0 \vec{E} \\ &= -i \omega \epsilon \epsilon_0 \vec{E} \nonumber\end{aligned}

 just like a dielectric, where

.. math::

   \label{eq:epsilon}
     \epsilon = 1 - \frac{\omega^2_{\rm p}}{\omega^2}

 is the plasma dielectric constant. NB
:math:`\epsilon = \epsilon(\omega)`; what’s the connection with
refractive index?

.. math::

   \begin{aligned}
     \nabla \times \vec{H} &= -i \omega \epsilon \epsilon_0 \vec{E} \\
   \nabla \times (\nabla \times \vec{H}) &= -i \omega \epsilon \epsilon_0 \nabla \times \vec{E} \\ &= \nabla(\nabla \cdot H) - \nabla^2 H \\ &= - \nabla^2 \vec{H}\end{aligned}

 since :math:`\nabla \cdot \vec{H} = 0` in a plasma. So, using a complex
notation for waves. Now,
:math:`\nabla \times \vec{E} = - \frac{\partial \vec{B}}{\partial t}`,
and we will take :math:`\vec{B}= \mu_0 \vec{H}`, so,

.. math::

   \begin{aligned}
     - \nabla^2 \vec{H} &= -i \omega \epsilon \epsilon_0 \nabla \times \vec{E} \\ &= i \omega \epsilon \epsilon_0 \mu_0 \frac{\partial \vec{H}}{\partial t}\end{aligned}

 or

.. math::

   \label{eq:waveeqpropeminplasma}
     \nabla^2 \vec{H} + \frac{\omega^2}{c^2} \epsilon \vec{H} = 0

 which is the wave equation for the propagation of electromagnetic waves
in the plasma. There is then a dispersion relation,

.. math::

   \begin{aligned}
     \frac{\partial}{\partial t} & \to -i \omega \\
   \vec{\nabla} & \to i \vec{k}\end{aligned}

 so

.. math::

   \begin{aligned}
     -k^2 + \frac{\omega^2}{c^2}\epsilon &= 0 \\
   \frac{\omega}{k} &= \frac{c}{\epsilon^{\frac{1}{2}}}\end{aligned}

 so, :math:`\epsilon^{\frac{1}{2}}`, and the plasma refractive index is
then

.. math::

   \label{eq:plasmarefind}
     n_{\rm plasma} = \left[ 1 - \frac{\omega_{\rm p}^2}{\omega^2}\right]^{\frac{1}{2}}

 Hence, if :math:`\omega < \omega_{\rm p}`, the index is purely
imaginary, and there is no wave propagation. If
:math:`\omega > \omega_{\rm p}` waves can propagate, but they will be
affected. If :math:`\omega = \omega_{\rm
  p}`—as we see more closely in the full cold plasma treatment, this
represents wave absorption. The full dispersion relation can then be
written

.. math::

   \label{eq:plasmadispersion}
     \omega^2 = \omega_{\rm p}^2 + k^2c^2

Cold Magnetised Plasma Model
----------------------------

| We will generalise the dielectric concept into a plasma immersed in a
  uniform magnetic field, but again, we will ignore thermal fluctuations
  in comparison with other dynamics, i.e. a cold plasma. A cold plasma
  doesn’t need to have a low temperature, but must have the
  termodynamic-based dynamics dominated by another factor.
| Recall what happens when a moving charged particle encounters a
  uniform magnetic field,

  .. math::

     \label{eq:momentumelectron}
       m \vec{\dot{v}} &= q(\dot{\vec{v}} \times \vec{B})

   and assume that :math:`\vec{B}` lies in the
  :math:`\vec{\hat{z}}`-direction, then

  .. math:: \vec{B} = \vec{\hat{z}} B_0

   so

  .. math:: \dot{\vec{v}} = \frac{q}{m} \left[ \vec{v} \times ( \hat{\vec{z}} B_0) \right]

   so in components,

  .. math:: \dot{v_x} = \frac{q}{m} \left[ \dot{v_y}B_0 - \dot{v}_z 0\right] = \frac{q B_0}{m} v_y

  .. math:: \dot{v_y} = \frac{q}{m} \left[ \dot{v_z} 0 - \dot{v}_x B_0\right] = - \frac{q B_0}{m} v_x

  .. math:: \dot{v_z} = \frac{q}{m} 0 = {\rm const}

   so, defining the cyclotron frequency

  .. math::

     \label{eq:cyclotron}
       \omega_{\rm c} = \frac{|q|B}{m}

   and for electrons,
  :math:`\nu_{\rm c} = 28\ \giga \hertz\ \tesla^{-1}`, hence

  .. math:: \ddot{v}_{x} = \omega_{\rm c} \dot{v_y} = \omega_{\rm c} [-\omega_{\rm c} v_x]

   that is

  .. math:: \ddot{v}_x + \omega_{\rm c}^2 v_x = 0

   which is plane perpendicular to the charged particle (e.g. an
  electron), which will thus undergo circular motion. THis motion is,
  however, uniform along the field. The net effect is that the particle
  will describe a helix.
| ***Exercise**: Show that the magnetic field doesn’t change the
  particle’s energy. Hint, consider :math:`\vec{v} \cdot \dot{\vec{v}}`*
| Let’s now consider the general response of a plasma in both magnetic
  and electric fields. We need to include the positive ions and the
  electrons together, plus, since this is a plasma, we need to consider
  the collective effects, i.e. a fluid treatment. Let’s define the
  perturbation,

  .. math::

     \begin{aligned}
     n_{\rm s} & = n_0_{\rm s}+ n_1(\vec{x},t) \\
     \vec{v_{\rm s}} & = \vec{v_{0,{\rm s}}} + \vec{v_1}(\vec{x},t)\end{aligned}

   Now, under perturbation, we can linearlise the most important
  equations:

.. math::

   \begin{aligned}
     \frac{\partial n_{\rm s} }{\partial t} + \nabla \cdot \qty(n_{\rm s} \vec{v_{\rm s}}) &= 0 \\
     \dot{n_{\rm s}} + n_{0,{\rm s}} \nabla \cdot \vec{v}_{\rm s} &= 0 \end{aligned}

.. math::

   \begin{aligned}
   \frac{\partial v_{\rm s}}{\partial t} +  (\vec{v_{\rm s}} \cdot \nabla) \vec{v_{\rm s}} &= \frac{q_{\rm s}}{m_{\rm s}} \qty[ \vec{E_{\rm s}}+ \vec{v_{\rm s}}\times \vec{B} ]  \\  
   \dot{\vec{v}} &= \frac{q_{\rm s}}{m_{\rm s}} [ \vec{E_1}+\vec{v_{\rm F}}\times B_0 ] \end{aligned}

.. math::

   \begin{aligned}
   \vec{J} &= \sum_{\rm s} n_{\rm s} q_{\rm s}\vec{v_{\rm s}} \\ 
   J_1 &= \sum_{\rm s} n_{0,{\rm s}} q_s \vec{v_{1, \rm s}}\end{aligned}

Recall Maxwell’s equations

.. math::

   \begin{aligned}
     \nabla \times \vec{B} &= \mu_0 \vec{J} + \frac{1}{c^2} \frac{\partial \vec{E}}{\partial t} \\
   \nabla \times \vec{E} &= - \frac{\partial \vec{B}}{\partial t} \\
   \nabla \cdot \vec{E} &= \frac{\rho_{\rm f}}{\epsilon_0} \\
   \nabla \cdot \vec{B} &= 0\end{aligned}

 *Tactic*: If we have :math:`\vec{v}` in terms of :math:`\vec{E}`,
(:math:`\vec{v}(E)`), then,
:math:`\vec{J} = \vec{J}(\vec{v}) = \vec{J}(\vec{E})`, with
:math:`\vec{J} = \vec{\sigma} \vec{E}`, then if we have a conductivity
law we can move to a dielectric description.

.. math::

   \begin{aligned}
     \vec{v} &= \frac{q}{m} \qty[ \vec{E} + \vec{v} \times \vec{B_0}]\\
   -i \omega v_x &= \frac{q}{m} \qty[ E_x + v_yB_0] \\
   &= \frac{q}{m}E_x + \omega_cv_y \\
   -i \omega v_y &= \frac{q}{m}E_y - \omega_cv_x\end{aligned}

| so

  .. math::

     \begin{aligned}
       -i\omega v_x &= \frac{q}{m} E_x - \frac{\omega_c}{i \omega} \qty[ \frac{q}{m}E_y - \omega_cv_x] \\
     -i \omega v_x - \frac{\omega_c^2}{i \omega} v_x &= \frac{q}{m} E_x - \frac{q \omega_c}{i \omega m}E_y \\
     &= \frac{q}{m}\qty[E_x - \frac{\omega_c}{i \omega} E_y] \\
     \qty(1 - \frac{\omega_c^2}{\omega^2}) v_x &= - \frac{q}{i \omega m} \qty[E_x - \frac{\omega_c}{i \omega}E_y] \\
     \text{since } \qty(1- \frac{\omega_c^2}{c^2}) v_y &= - \frac{q}{i \omega m} \qty[ E_x + \frac{\omega_c}{i \omega} E_y] \\
     (1 - \frac{\omega_c^2}{\omega^2} \vec{v} &= M \cdot \vec{E} \\
     \vec{v} &= \frac{1}{\qty(1 - \frac{\omega_{c}^2}{\omega^2})} \cdot M \cdot \vec{E}\end{aligned}

   So, we know that we can get to this expression for
  :math:`\vec{J}`—how does this help? We now bring Maxwell’s equations
  into the mixture.

  .. math::

     \begin{aligned}
      \nabla \times \vec{E} &= \pdv{\vec{B}}{t} \\
     \nabla \times ( \nabla \times \vec{E}) &= - \nabla \times \qty( \pdv{\vec{B}}{t}) \\
     &= - \pdv{t} \qty(\nabla \times \vec{B}) \\
     &= - \pdv{t} \qty[\mu_0 \vec{J} + \frac{1}{c^2} \pdv{\vec{E}{t}}] \\
     &= - \pdv{t} \qty[\mu_0 \vec{\sigma} \cdot \vec{E} + \frac{1}{c^2} \pdv{\vec{E}}{t}]\end{aligned}

   We are interested in waves, where solutions are proportional to
  :math:`e^{i \vec{k}\cdot \vec{r} - i \omega t}`
| LHS:
| 

  .. math::

     \begin{aligned}
       \nabla \times (\nabla \times \vec{E}) &= - \vec{k} \times (\vec{k} \times \vec{E})\end{aligned}

   RHS:
| 

  .. math::

     \begin{aligned}
       i \omega \qty[ \mu_0 \vec{\sigma} \cdot \vec{E} - \frac{i \omega}{c^2} \vec{E}]\end{aligned}

   So, the full equation is

  .. math:: \vec{k} \times (\vec{k} \times \vec{E}) + \frac{\omega^2}{c^2} K \cdot \vec{E} &= 0

   with

  .. math:: K = I + \frac{i \sigma}{\epsilon_0 \omega}

   being the dielectric tensor.
| Define the generalised refractive index,

  .. math:: \vec{n}= \frac{\vec{k}c}{\omega}

   (a refractive index with “directional complications”),

  .. math:: \label{eq:genrefind} \vec{n} \times ( \vec{n} \times \vec{E} ) + K \cdot \vec{E} = 0

   To help to understand the significance of equation ([eq:genrefind]),
  let’s choose a geometry—let’s put
  :math:`\vec{B}_0 = \vec{\hat{z}} B_0`, and let’s take a wave in the
  :math:`\vec{\hat{x}}-\vec{\hat{z}}`-plane (with one component parallel
  to :math:`\vec{B}_0`, and one perpendicular),

  .. math::

     \begin{aligned}
       \vec{n} &= \hat{x} n \sin(\theta) + \hat{z} n \cos(\theta)\end{aligned}

   Then expand the vector cross-product
  :math:`\vec{n} \times (\vec{n} \times \vec{E})` for this choice of
  geometry.

  .. math::

     \begin{aligned}
       \begin{pmatrix}
     S-n^2 \cos^2\theta  & - iD & n^2 \cos(\theta) \sin(\theta) \\
     iD & S-n^2 & 0 \\
     n^2 \cos\theta \sin\theta & 0 & P- n^2 \sin^2 \theta
     \end{pmatrix}
     \begin{pmatrix}
       E_x \\ E_y \\ E_z
     \end{pmatrix}
     = 0\end{aligned}

   Where we have written

  .. math::

     \label{eq:dielectricten}
     K=
       \begin{pmatrix}
       S & -iD & 0 \\ iD & S & 0 \\ 0 & 0 & P  
       \end{pmatrix}

   Where

  .. math::

     \begin{aligned}
       S &= \frac{1}{2}(R+L) \\
       D &= \frac{1}{2}(R-L)\end{aligned}

   and

  .. math::

     \begin{aligned}
       R &= 1 - \sum_S \frac{\omega^2_{\rm P_s}}{\omega^2} \qty( \frac{\omega}{\omega+\epsilon_0 \omega_{\rm c_s}}) \\
     &= 1 - \frac{\omega_{\rm P}^2}{(\omega+\omega_{\rm C_+})(\omega-\omega_{\rm c^-})} \\
     L &= 1 - \sum_S \frac{\omega_{\rm P_s}^2}{\omega^2} \qty(\frac{\omega}{\omega-\epsilon_{\rm s} \omega_{\rm c_s}}) \\
     &= 1 - \frac{\omega_{\rm p}^2}{(\omega-\omega_{\rm c_+})(\omega+\omega_{\rm c_-})} \\
     \epsilon_{\rm s} &=
     \begin{cases}
       +1 & \text{ for positive ion } \\
       -1 & \text{ for negative electron}
     \end{cases} \\
     \omega_{\rm P}^2 &= \omega_{\rm P_+}^2 + \omega_{\rm P_{-}}^2 \\
     P &= 1 - \frac{\omega_{\rm P}}{\omega^2}\end{aligned}

   For a non-trivial electric field the determinant of the matrix must
  vanish, giving a relationship between :math:`\omega` and :math:`k` so
  th dispertion relation

  .. math::

     \label{eq:dispertionrelation}
       An^4 - Bn^2 + C = 0

   with

  .. math::

     \begin{aligned}
       A &= S \sin[2](\theta) + P \cos[2](\theta) \\
     B &= RL \sin[2](\theta) + PS (1 + \cos[2](\theta) \\
     C &= PRL\end{aligned}

   *N.B. There are two spherical cases, :math:`\theta=0`, and
  :math:`\theta= \frac{\pi}{2}`*.
| For the case :math:`\theta=0`, the propagation is parallel to
  :math:`B_0`, so

  .. math::

     \begin{pmatrix}
     S-n^2 & -iD & 0 \\
     iD & S-n^2 & 0 \\
     0 & 0 & P 
     \end{pmatrix}
     \begin{pmatrix}
       E_x \\ E_y \\ E_z
     \end{pmatrix} = 0

   i.e. :math:`(S-n^2)^2 - D^2 = 0` if :math:`E_x, E_y \neq 0` or
  :math:` P=0` if :math:`E_z\neq
  0`.
| When :math:`P=0` we have longitudinal plasma oscillations (just like
  before),

  .. math::

     \begin{aligned}
       n^2 = R & \frac{iE_x}{E_y} = - \frac{S-n^2}{D} = - \frac{S-R}{D} = 1 & \text{right circ. pol.} \\
     n^2 = L & \frac{i E_x}{E_y} = - \frac{S-n^2}{D} = - \frac{S-L}{D} = -1 & \text{left circ. pol.}\end{aligned}

   *N.B. Recall that
  :math:`S = \frac{1}{2} (R+L) \therefore S-R = \half{}(-R+L) = -D`
  etc.*
| When :math:`n^2 = R, L` we get circularly polarised transverse waves.
| :math:`n^2=R` has resonance at :math:`\omega = \omega_{\rm c_e}`,
  :math:`n^2=L` at :math:`\omega=\omega_{\rm c_i}`, which are the
  particle cyclotron frequencies where the particle naturally
  oscillates. :math:`R, L` has a cut-off when the numerator is zero,

  .. math::

     \label{eq:cutoff}
       \omega^2 \mp (\omega_{\rm re}-\omega_{\rm c_i}) \omega - (\omega_p^2 + \omega_{c_i}\omega_{c_e})=0

   i.e. at
  :math:`\omega \sim \mp \half \omega_{\rm c_e}+ \qty(\omega_{\rm p}^2 + \frac{1}{4}\omega_{c_{e}}^2)^{\frac{1}{2}}`.
  At the low-frequency limit, if :math:`\omega \ll \omega_{\rm c_i}`
  (the lowest natural frequency is :math:`\omega_{\rm c_i}`, then
  :math:`R \sim L \sim 1+ \frac{c^2}{c_A^2}`, where
  :math:`C_A^2 = \frac{B_0^2}{\mu_0\rho_0}` is the Alfven speed. The
  refractive index is :math:`n^2 = 1+\frac{c^2}{c_A^2}`, i.e.
  :math:`\omega^2 = \frac{k^2 c^2}{1 + \frac{c^2}{c_A^2}} \approx k^2c_A^2`
  which descripe non-dispersive Alfven waves (c.f. Magnetohydrodynamics
  later).

For :math:`\theta = \frac{\pi}{2}`, waves propagating perpendicular to
:math:`B_0`, the dispertion relation becomes

.. math:: Sn^4 - (RL + PS)n^2 +PRL = 0

 with two roots at :math:`n^2=P`, and :math:`n^2 = \frac{RL}{S}`.
Characteristics of these modes are best seen in a matrix system.

.. math::

   \label{eq:dispertion}
     \begin{pmatrix}
       S  & -iD   & 0 \\
       iD & S-n^2 & 0 \\
   0      & 0     & P-n^2
     \end{pmatrix}
     \begin{pmatrix}
       E_x \\ E_y \\ E_z
     \end{pmatrix} = 0

#. For :math:`E_x = E_y = 0`, and :math:`E_z \neq 0`, we have
   :math:`n^2=P`, i.e. we have the same dispertion relation as in the
   unmagnetic case. Note, :math:`\vec{k}\cdot \vec{E} = 0`, so we have
   transverse electormagnetic waves which are independent of
   :math:`B_0`, and :math:`E` is parallel to :math:`B_0`, so all motion
   is aligned with :math:`B_0`, and therefore

   .. math:: n^2 = P \qquad \text{(Ordinary mode, O-mode)}

    and the cutoff is at the plasma frequency, with no resonance.

#. Now suppose we consider :math:`E_z=0`, :math:`E_x, E_y \neq 0`, then
   :math:`n^2 = \frac{RL}{S}` in solution,

   .. math:: \frac{iE_x}{E_y} = - \frac{S-n^2}{D} = - \frac{D}{S}

    (first row gives :math:`SE_x - iD E_y = 0`). Hence the wave is
   partly longitudinal, and partly transverse, since both
   :math:`E_x, E_y \neq 0`, and thus
   :math:`\vec{k} \cdot \vec{E} \neq 0`. The fact that :math:`E` is
   perpendicular to :math:`B_0` means that same for the gyration about
   the magnetic field which is generated, so wave properties depend on
   :math:`B_0`,

   .. math:: n^2 = \frac{RL}{S} \qquad \text{(Extraordinary mode, X-mode)}

    the cutoff :math:`R=0` or :math:`L=0`, and resonance at :math:`S=0`.

| We have

  .. math::

     \begin{aligned}
       R & = 1 - \frac{\omega_{\rm p}^2}{(\omega+\omega_{\rm c_+})(\omega-\omega_{c_-})} \\
       L & = 1 - \frac{\omega_{\rm p}}{(\omega-\omega_{\rm c_+})(\omega+\omega_{\rm c_-})}\end{aligned}

   since :math:`\omega \ll \omega_{c_i}`

  .. math::

     \begin{aligned}
       R &\approx 1 - \frac{\omega_p^2}{\omega_{c_i}(-\omega_{c_e})} \\
         &= 1 + \frac{\frac{ne^2}{\epsilon_0 m_e} + \frac{n e^2}{\epsilon_0 m_i} } {\frac{eB_0}{m_i} \frac{e B_0}{m_e}} \\
         &= 1 + \frac{n(m_i+m_e)}{\epsilon_0 B_0^2} \\
         &\approx 1 + \frac{\mu_0 \rho_0 c^2}{B_0^2} \\
         &= 1 + \frac{c^2}{c_A^2} \approx \frac{c^2}{c_A^2}\end{aligned}

   For :math:`\theta = 0`, :math:`\omega \ll \omega_{c_i}`, which are
  both circular polarisations for transverse Alfven waves. Then,

  .. math:: n^2 = \frac{kL}{S} \therefore \omega^2 = k^2 c_A^2

   and

  .. math:: S = \half (R+L)

   but :math:`n^2 = P`, so there is a cutoff; no low frequency is
  possible.
| For :math:`n^2 = \frac{RL}{S}` (the X-mode) at low frequency. We have
  a compressional Alfven wave, which is different to the
  :math:`\theta=0` case, even though they share a dispersion relation.
| For :math:`\theta=\frac{\pi}{2}`,

  .. math::

     \begin{pmatrix}
         S & -iD & 0 \\
     iD & S-n^2 & 0 \\
     0 & 0 & P-n^2
       \end{pmatrix}

   So

  .. math::

     \begin{aligned}
       S E_x - iD E_y & = 0 \\
      \frac{i E_x}{E_y} &= - \frac{D}{S}\end{aligned}

   So what are the implications for the Alfven wave? Since :math:`R`,
  :math:`L` are approximately equal, for :math:`\omega \ll \omega_c`,

  .. math:: \qty|\frac{E_x}{E_y}| \ll 1

   and so :math:`|E_y| \gg |E_x|`. From the equations of motion,

  .. math::

     \begin{aligned}
     \dot{v}_x &= - \frac{e}{m} E_x - \omega_c v_y \\
     \dot{v}_y &= - \frac{e}{m} E_y - \omega_c v_x\end{aligned}

   we can differentiate the system with respect to :math:`t` to show

  .. math:: \qty| \frac{v_x}{v_y} | \approx \frac{\omega_c}{\omega} \quad \text{when}\quad \qty| \frac{E_x}{E_y} | \approx 0

   We know that the O-mode cuts off at :math:`\omega=\omega_{\rm p}`.
  For the X-mode, :math:`n^2= \frac{RL}{S}`, the two cutoffs occur at
  :math:`R=0` or :math:`L=0`. This is the same as the circuarly
  polarised waves as before, but we have two cutoff frequencies for the
  same mode. Resonance occurs at :math:`S=0`, and again, this occurs at
  two places, an upper and a lower hybrid frequency:

  .. math::

     \begin{aligned}
       \omega_u^2 &= \omega_p^2 + \omega_{c_e}^2 \\
     \omega_l^2 &= \omega_p^2 \frac{\omega_{c_i}\omega_{c_e}}{\omega_p^2+\omega_{c_e}^2}\end{aligned}

Ideal Magnetohydrodynamic Plasmas
---------------------------------

Here we consider the behaviour of plasmas at long wavelengths, and low
frequencies; in this limit we can retrieve classical thermodynamic
relations. Starting with the model equations,

.. math::

   \begin{aligned}
       \pdv{\rho}{t} + \nabla \cdot (\rho \vec{u}) &= 0 \\
   \rho \adv{\vec{u}}{t} &= - \nabla p + \vec{J} \times \vec{B} + (q \vec{E}) \\
   \adv{t} \qty[ p \rho^{-\gamma} ] &= \frac{2}{3} \rho^{-\gamma} \qty[ \vec{J} - q \vec{u}] \cdot \qty[ \vec{E} + \vec{u} \times \vec{B}] \\
   \vec{J} &= \sigma \qty[ \vec{E} + \vec{u} \times \vec{B}]
     \end{aligned}

| with :math:`\rho` the mass density, :math:`\vec{u}` the bulk fluid
  velocity field, :math:`p` the scalar pressure, :math:`q` the
  unbalanced charge, :math:`\vec{J}` the current density, and
  :math:`\vec{B}` the magnetic field. We take
  :math:`\gamma = \flatfrac{5}{3}`
| We assume there is no :math:`\vec{E}` in the momentum equation, partly
  because we assume the plasma is a single species fluid with all the
  electrical properties of an electron-ion plasma, but with no charge
  separation. Additionally, we can consider the electric field as
  arrising only due to frame changes.
| In this situation, Maxwell’s equations are

.. math::

   \begin{aligned}
       \nabla \times \vec{B} &= \mu_0 \vec{J} \\
   \nabla \times \vec{E} &= - \pdv{\vec{B}}{t} \\
   \nabla \cdot \vec{B} &= \nabla \cdot \vec{E} =0
     \end{aligned}

Notably, Ampere’s law contains no mention of displacement current, and
there is no allowance for charge separation. An ideal MHD plasma
exhibits perfect conductivity, so

.. math:: \vec{E} + \vec{u} \times \vec{B} = \eval{\frac{\vec{J}}{\sigma}}_{\sigma \to \infty}

 thus

.. math:: \vec{E} + \vec{u} \times \vec{B} =0

 and

.. math:: \adv{t}\qty[p \rho^{-\gamma}] = 0

 In order to understand how the ideal MHD plasma behaves we need to look
at the normal modes, just as with the cold plasma case. Take a
perturbation,

.. math::

   \begin{aligned}
       p   & = p_0 + p_1 (\vec{r}, t)             \\
   \vec{B} & = \vec{B}_0 + \vec{B}_1 (\vec{r}, t) \\
   \vec{u} & = \vec{u}_0 + \vec{u}_1 (\vec{r}, t) \\
   \rho    & = \rho_0 + \rho_1 (\vec{r}, t)       \\
   \vec{J} & = \vec{J}_0 + \vec{J}_1 (\vec{r}, t)
     \end{aligned}

Then we assume :math:`\vec{u}_0 = 0` (stationary equilibrium), and
:math:`\vec{J}_0 = \frac{\nabla \times \vec{B}}{\mu_0} = 0`.

Then linearise,

.. math::

   \pdv{\rho}{t} + \nabla \cdot (\rho \vec{u}) = 0 \to \pdv{\rho_1}{t}
   + \vec{u}_0 \cdot \rho_1 = 0

then, assuming all perturbed quantities are proportional to
:math:`\exp[ i(\vec{k} \cdot \vec{r} - \omega
t)]`, so

.. math::

   \begin{aligned}
     \rho_1 &= \frac{\rho_0}{\omega} (\vec{k} \cdot \vec{u}_1) \tag{I} \\
   \rho_0 &= \pdv{\vec{u}_1}{t} = - \nabla p_1 + \vec{J}_1 \times \vec{B}_0 \end{aligned}

 Wave analysis on the momentum equation leads to

.. math::

   \begin{aligned}
     \omega \rho_0 \vec{u}_1 &= \vec{k} p_1 + \frac{\vec{B}_0 \cdot \vec{B}_1}{\mu_0} \vec{k} - \frac{(\vec{k} \cdot \vec{B}_0)}{\mu_0} \vec{B}_1 \tag{II} \\
   \pdv{\vec{B}}{t} &= - \nabla \times \vec{E} = \nabla \times (\vec{u}_1 \times \vec{B}_0) \\
   \omega B_1 &= ( \vec{k} \cdot \vec{u}_1) \vec{B}_0 - (\vec{k} \cdot \vec{B}_0 ) \vec{u}_1 \tag{III} \\\end{aligned}

 Since :math:`p \rho^{-\gamma}` is constant,

.. math:: \adv{t} \qty( p \rho^{-\gamma} )

 so

.. math:: p_1 = c_{\rm s}^2\rho_1 \tag{IV}

 where :math:`c_{\rm s}^2` is the sound speed in the plasma, and since
:math:`\nabla \cdot \vec{B} = 0`,

.. math:: \vec{k} \cdot \vec{B}_1 = 0 \tag{V}

 We now want to eliminate :math:`p_1` and :math:`B_1` from (II), to
obtain everything in terms of :math:`u_1`. :math:`p_1` can be eliminated
using (IV), :math:`\rho_1` using (I), and :math:`B_1` using (III).

This process yields

.. math::

   \label{eq:mhdequation}
   \begin{split}
     \qty[ \omega^2 - \frac{(\vec{k} \cdot \vec{B}_0 )^2}{\mu_0 \rho_0}] \vec{u}_1 = \qty[(r_{\rm s}^2 + c_{\rm A}^2) \vec{k} - \qty( \frac{\vec{k} \cdot \vec{B}_0}{\mu_0 \rho_0} ) B_0] (\vec{k} \cdot \vec{u}) \\- \frac{(\vec{k}\cdot \vec{B}_0)(\vec{B}_0 \cdot \vec{u}_1)}{\mu_0 \rho_0} \vec{k}
   \end{split}

 with :math:`c_{\rm A}^2 = \frac{B_0^2}{\mu_0 \rho_0}`. Now we choose

.. math::

   \begin{aligned}
       \vec{B}_0 &= B_0 \hat{b} \\ \vec{k} &= k \hat{z}
     \end{aligned}

Then,

.. math::

   \label{eq:mhdincoordis}
   \begin{split}
     \qty[ \omega^2 - k^2 c_{\rm A}^2 (\hat{z} \cdot \hat{b})^2 ] \vec{u}_1 = \qty[ k^2 (c_{\rm s}^2 + c_{\rm A}^2) \hat{z} + \vec{k}^2 c_{\rm A}^2 (\hat{z} \cdot \hat{b} ) \hat{b} ](\hat{z} \vec{u}_1) \\ - k^2 c_{\rm A}^2 (\hat{z} \cdot \hat{b}) (\hat{b} \cdot \vec{u}_1) \hat{z}
   \end{split}

 Let’s consider a special case; In MHD :math:`\omega` is much less than
the minimum cyclotron frequency for ions and plasma frequency, and the
wavelength is much greater than the Debye length of the Larmour Radius.
Consider the component of :math:`\vec{u}_1` perpendicular to the
direction of motion, :math:`\hat{z}`. To find this direction take the
cross-product of the whole equation ([eq:mhdincoordis]), with
:math:`\hat{z}`. Now take :math:`\hat{z} \cdot \hat{b} = \cos(\theta)`.

.. math::

   \begin{aligned}
     (\omega^2 - k^2 c_A^2 \cos[2](\theta))(\hat{z} \times \vec{u}_1) &= -k^2 c_A^2 \cos(\theta) (\hat{z} \cdot \vec{u}_1)(\hat{z} \times \hat{b})\end{aligned}

 Suppose the plasma is incompressible, so
:math:`\hat{z} \cdot \vec{u}_1 = 0`, and we still have
:math:`(\omega^2 - k^2 \cos[2](\theta))(\hat{z} \times \vec{u}_1) = 0`.
Clearly a non-trivial solution, governed by the dispertion relation is
possible: a wave which satisfies

.. math::

   \label{eq:shearalfven}
     \omega^2 = k^2 c_A^2 \cos[2](\theta)

 which is an *shear Alfvén wave*. We have a transverse wave at low
frequency–for :math:`\theta=0` this is just like a cold plasma solution,
but at :math:`\theta=\frac{\pi}{2}` there is no transverse wave
solution, but the cold plasma has the low frequency limit of the X-mode,
the compressed Alfvén mode.

The general solution for MHD waves is that we have a dispertion reltion,

.. math:: \qty(\omega^2 - k^2 c_A^2 \cos[2](\theta) ) \cdot \qty( \omega^4 - k^2( c_A^2 + c_s^2) \omega^2 + k^2c_s^2c_A^2 \cos[2](\theta))

 Then there are three modes,

-  Alfven

   .. math:: \omega^2 = k^2 c_A^2 \cos[2](\theta)

-  Fast (+) and Slow (-) Magnetosonic

   .. math:: 2 \frac{\omega^2}{k^2} = c_s^2 + c_A^2 \pm \sqrt{( c_s^2 + C_A^2)^2 - 4k^2 c_s^2 c_A^2 \cos[2](\theta)}

For the fast MS mode, :math:`\frac{B^2}{2 \mu_0}` magnetic pressure
enhanes the thermodynamic pressure, :math:`p`, by varying in phase with
it. Fr the slow MS mode the magnetic presure and thermodynamic pressure
oppose one another. Magnetic pressure plays a powerful conceptual role
in MHD.

Recall the equilibrium; to see how significant the magnetic pressure can
be,

.. math::

   \begin{aligned}
     \adv{t} &= 0\\
   \nabla p_0 &= \vec{J}_0 \times \vec{B}_0 \end{aligned}

 before we set :math:`\vec{J}_0 =0` (so the plasma had a uniform
:math:`\vec{B}_0` and :math:`p_0`, however, we can generalise this,
since

.. math::

   \begin{aligned}
     \nabla \times \vec{B} &= \mu_0 \vec{J}_0 \\
   \nabla p_0 &= \frac{1}{\mu_0} (\nabla \times \vec{B}_0) \times \vec{B}_0\end{aligned}

 which can be rewritten in the form

.. math::

   \nabla \qty(p_0 + \half \frac{\vec{B}_0^2}{\mu_0}) +
   \frac{1}{\mu_0}( \vec{B}_0 \cdot \nabla) \vec{B}_0

 for the simplest geometry take
:math:`\vec{B}_0 \cdot \nabla \vec{B}_0 = 0`, for equilibrium,

.. math::

   \label{eq:equilibrium}
     \nabla \qty(p_0 + \frac{\vec{B}_0^2}{2 \mu_0} ) = 0

 That is, the plasma pressure plus the magnetic pressure is constant.
Plasma tends to avoid the strongest field regions in equilibrium. This
is a possible mechanism for confinement. How could this go wrong?
Suppose we have a cylinder of plasma, which is carrying current. It has
an azimuthal :math:`\vec{B}_0`

(2,0) ellipse (.2 and .5);

(-2,-.5) rectangle (2, .5); (-2,0) ellipse (.2 and .51);

in -1,-.5,..., 1.5 (, -.5) ..controls (+.2, -.3) and (+.2, .3) .. (,.5);
(-1.8, -.5) ..controls (-1.8+.2, -.3) and (-1.8+.2, .3) .. (-1.8,.5)
node [midway, right] :math:`\vec{B}_0`;

(0,.9) – (2,.9) node [midway, fill=white] :math:`\vec{J}`;

If we bend the cylinder, but wish to maintain :math:`\vec{J}_0`,

The magnetic pressure is stronger on the inside of the bend than the
outside. Thus the plasma is push upwards, wosening the distortion. This
gives a kink instability.

Pinch Instability
~~~~~~~~~~~~~~~~~

in 1.5,2,..., 4 (7,-) .. controls (3,-) and (2,-) .. (-1,-) (7,-) ..
controls (10,-) and (12,-) .. (15,-); (7,) .. controls (3,) and (2,) ..
(-1,) (7,) .. controls (10,) and (12,) .. (15,);

We find that :math:`\vec{B}_0` is more intense at the pinch because
:math:`\vec{J}_0` is larger. Hence the plasma is expelled from the
pinched region, drawing the current density up, and making the problem
worse. The plasma is described as pinching off.

Plasmas with Collision
----------------------

Consider a binary collision of two plasma particles, where the Coulomb
force between the particles is

.. math::

   \label{eq:15}
     F = \frac{q_1 q_2}{4 \pi \epsilon_0 r^2}

 For simplicity, we restrict the interaction to an electron and a heavy
ion.

(0,0) circle (0.5) node [midway, white] +; (-4,1) circle (0.2) node
[white] -;

(-3.7,1) – (0,1) arc (90:40:1) – ++(130:-2);

(0,1) – (4,1) (1,0)–(4,0);

(3,1) – (3,0) node [right, midway] :math:`b = r \sin(\theta)`;

Consider the change of :math:`v_{\perp}`, with a massive ion,
:math:`m_{\rm ion}
\gg m_{\rm e}`. The change of perpendicular momentum from the equation
of motion can be written

.. math::

   \label{eq:16}
     m_{\rm e} v_{\perp} = \int_{-\infty}^{+\infty} F \dd{t} \sim F \Delta t

 So, we can approximate,

.. math::

   m_{\rm e} v_{\perp} \approx \frac{q_{\rm e} q_{\rm i}}{4 \pi
     \epsilon_0 r^{2} } \frac{r}{v} = \frac{q_{\rm e} q_{\rm i}}{4 \pi
     \epsilon_0 r v }

 For large-angle collisions (where the deflection is close to
:math:`90^{\circ}`), the change of :math:`m_{\rm e} v_{\perp}` is of the
order of :math:`mv` itself, so,

.. math::

   m_{\rm e} v_{\perp} \approx m_{\rm e} v = \frac{q_{\rm e} q_{\rm i}}{4 \pi
      \epsilon_0 r v }

 and :math:`r \approx b`, so we can estimate :math:`b` as

.. math:: b = \frac{q_{\rm e} q_{\rm i}}{4 \pi \epsilon_0 v^2 m_{\rm e}}

The interaction between two particles can be described using the
interaction cross-section, :math:`\sigma`, where

.. math:: \sigma = \pi b^2

with :math:`b` being the area of the disc. We simply assume the
interaction is happening for impact parameters

.. math:: b \ll \frac{q_{\rm e} q_{\rm i}}{4 \pi \epsilon_0 v^2 m_{\rm e}}

 and no interaction for large :math:`b`.

For this interaction the cross-section is

.. math::

   \label{eq:17}
     \sigma_{\rm ei} = \pi b^2 = \pi \frac{q_{\rm e}^2 q_{\rm i}^2}{(4 \pi \epsilon_0)^2 (m_{\rm e} v)^2}

 The collision frequency is then

.. math:: \nu_{\rm ei} = n \sigma_{\rm ei} v

 Then, the e-i collision frequency for a :math:`z=1` plasma, so that
:math:`n_{\rm i} \approx n_{\rm e}`, and
:math:`q_{\rm i} = q_{\rm e} = e` is

.. math::

   \label{eq:18}
     \nu_{\rm ei} = n_{\rm e} \sigma_{\rm ei} v \approx \frac{\pi n_{\rm e} e^4}{(4 \pi \epsilon_0)^2 m_{\rm e}^2 v^3} \sim \frac{n_{\rm e}}{v^3}

 For the average electron velocity with thermal energy,

.. math:: k_{\rm B} T_{\rm e} = \half m_{\rm e} v_{\rm te}^2

 thus

.. math::

   v_{\rm te} = \qty( \frac{2 k_{\rm B} T_{\rm e}}{m}
   )^{-\frac{1}{2}}

.. math::

   \label{eq:19}
     \nu_{\rm ei} \approx \frac{\sqrt{2}}{64 \pi} \frac{\omega_{\rm pe}^4}{n_{\rm e}} \qty( \frac{k_{\rm B} T_{\rm e}}{m})^{-\frac{3}{2}} = \frac{\pi n_{\rm e} e^4}{2^{\frac{3}{2}} (4 \pi \epsilon_0)^2 m_{\rm e}^2 \qty( \frac{k_{\rm B} T_{\rm e}}{m_{\rm e}})^{\frac{3}{2}}}

 So we conclude

.. math:: \nu_{\rm ei} \sim nT^{- \frac{3}{2}}

 This is a rough estimate, there are many small-scale collsions in
plasma, and a more rigorous estimate indicates

.. math::

   \label{eq:20}
     \nu_{\rm ei} = \frac{4 \sqrt{2}}{3 \sqrt{\pi}} \frac{\pi n_{\rm e} e^4 (\log(\Lambda)}{(4 \pi \epsilon_0)^2 m_{\rm e}^{\half} (k_{\rm B}T_{\rm e})^{\frac{3}{2}}} \approx \omega_{\rm pe} \frac{\log(\Lambda)}{\Lambda}

 Where :math:`\Lambda` is the number of electrons in the Debye Sphere,
:math:`\Lambda \sim n_{\rm e} \lambda^3_{\rm De}`. :math:`\log(\Lambda)`
is the Coulomb logarithm, and is normally assumed to be constant, with a
value in the range :math:`\log(\Lambda) \in [10,30]`.

Mean Free Path
~~~~~~~~~~~~~~

Let us estimate the mean free path of an electron in a plasma;

.. math::

   \lambda = \frac{v_{\rho}}{\nu_{\rm ei}} \sim \frac{\omega_{\rm pe}
     \lambda_{\rho \rm e}}{\nu_{\rm ei}} \approx \qty( \frac{\omega_{\rm
       pe}}{\nu_{\rm ei}}) \lambda_{\rm De}

*The mean free path of the solar corona.* In the plasma composing the
solar corona,

.. math:: n_{\rm e} \sim 1 \e{15} \meter^{-3} , \qquad k_{\rm B} T_{\rm e} \sim 1\e{2} \electronvolt

 Then

.. math:: \nu_{\rm ei} \approx \frac{5\e{-11} \times 10^{15}}{10^3} \approx 50 \second^{-1}

 and since

.. math:: \omega_{\rm pe} \approx 2 \pi \nu_{\rm pe}, \qquad \nu_{\rm pe} = 9(n_e)^{\half}

 we find

.. math::

   \omega_{\rm pe} \sim 2 \pi \times 9 \times 3.2\e{3} \times 10^4 = 2
   \pi \times 3\e{8} \second^{-1} \gg \nu_{\rm ei}

 Hence the mean free path is much larger than the Debye length.

Collision Equilibration Times
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For electron-ion collisions in plasma

.. math::

   \nu_{\rm ei} \propto \frac{n}{m_{\rm e}^{\half} T_{\rm
       e}^{\frac{3}{2}}}

We define the quantity :math:`\tau_{\rm ei} :=
\frac{1}{\nu_{\rm ei}}` which is the time between collisions, or the
mean free time. For the frequency of electron-electron collisions
(taking into account the finite mass of the scattering particle, and
replacing it with :math:`m_{\rm e}`) we have a factor of two, and so,

.. math:: \nu_{\rm ee} \approx \nu_{ei}

 For ion-ion collisions the :math:`m_{\rm e}` must become
:math:`m_{\rm i}`, and so

.. math::

   \nu_{\rm ii} \approx \qty( \frac{m_{\rm e}}{m_{\rm i}} )^{\half}
   \nu_{\rm ee}

 For ion-electron collsions the transformation to the centre-of-mass
frame introduces a factor of :math:`\frac{m_{\rm e}}{m_{\rm
    i}}`, hence

.. math:: \nu_{\rm ie} \approx \frac{m_{\rm e}}{m_{\rm i}} \nu_{\rm ee}

If :math:`T_{\rm e} \neq T_{\rm i}`, there will be an exchange of
temperature caused by the collisions, and the timescales of the
interactions are

.. math::

   \tau_{\rm ee}^{\rm E} : \tau_{\rm ii}^{\rm E} : \tau_{\rm ei}^{\rm
     E} \sim 1 : \qty( \frac{m_{\rm i}}{m_{\rm e}} )^{\half} :
   \frac{m_{\rm i}}{m_{\rm e}}

It is worth noting that :math:`\nu_{\rm ei}` is not the rate at which
equilibrium is established between electrons and ions, but is instead
the rate of momentum transfer from electrons to ions, and not the rate
of energy transfer between them. The relaxation time for electorn-ion
equiilibrium is given by ion-electron collisions, and
:math:`\frac{m_{\rm e}}{m_{\rm i}} \nu_{\rm ee}`. For a Hydrogen plasma

.. math:: \frac{m_{\rm i}}{m_{\rm e}} = 1836

 so

.. math::

   \label{eq:21}
     \tau_{\rm ee} : \tau_{\rm ii} : \tau_{\rm ei}^{\rm E} \sim 1 : 43 : 1836

Resitivity and Collisions
~~~~~~~~~~~~~~~~~~~~~~~~~

Consider an unmagnetised quasineutral plasma with
:math:`n_{\rm i} \approx
n_{\rm e}` of electrons and ions both with charge :math:`q = e`. In
response to an applied electric field, :math:`\vec{E}`, a current will
flow in the plasma. The current density will be

.. math::

   \label{eq:22}
     \vec{\jmath} = n_{\rm i} e \vec{v}_{\rm i} - n_{\rm e} e \vec{v}_{\rm e}

 Electrons have a much smaller mass than the ions, so the plasma current
is predominantly carried by the electrons, hence,

.. math::

   \label{eq:23}
     m_{\rm e} n_{\rm e} \dv{\vec{v}_{\rm e}}{t} = -e n_{\rm e} \vec{E} + m_{\rm e} n_{\rm e} (\vec{v}_{\rm i} - \vec{v}_{\rm e}) \nu_{\rm ei}

 In a steady state there is no change with time, so

.. math:: \vec{E} = \frac{m_{\rm e} n_{\rm e} (\vec{v}_{\rm i} - \vec{v}_{\rm e}) \nu_{\rm ei}}{e n_{\rm e}} = \frac{e n_{\rm e} (\vec{v}_{\rm i}-\vec{v}_{\rm e} ) m_{\rm e} \nu_{\rm ei}}{e^2 n_{\rm e}} = \frac{m_{\rm e} \nu_{\rm ei}}{e^2 n_{\rm e}} \vec{\jmath}

 According to Ohm’s law,

.. math::

   \label{eq:24}
     \vec{E} = \rho \vec{\jmath}

 where :math:`\rho` is the resistivity,

.. math::

   \rho = \frac{m_{\rm e}}{e^2 n_{\rm e}} \nu_{\rm ei} =
   \frac{1}{\sigma}

 with :math:`\sigma` the conductivity. Conservation of momentum prevents
electron-electron collisions contributing to the resisitivity, and so

.. math::

   \rho = \frac{m_{\rm e}}{e^2 n_{\rm e}} \frac{\pi n_{\rm e} e^4
     \log(\Lambda)}{\qty(4 \pi \epsilon_0)^2 m_{\rm e}^{\half}
     \qty(k_{\rm B} T)^{\frac{3}{2}}} = \frac{\pi m_{\rm e}^{\half} e^2
     \log(\Lambda)}{(4 \pi \epsilon_0)^2 (k_{\rm B}T)^{\frac{3}{2}}}

 Again, it is worth noting that resistivity is independent of density,
and decreases with growing temperature.

Diffusion of Particles
~~~~~~~~~~~~~~~~~~~~~~

The fluid equation of motion including collisions for electrons is

.. math::

   \label{eq:25}
     m_{\rm e} n_{\rm e} \dv{\vec{v}}{t} = q n_{\rm e} \vec{E} - \nabla p - m_{\rm e} n_{\rm e} \nu_{\rm ei} \vec{v}

 for pressure :math:`p`, and assuming
:math:`n_{\rm e} \approx n_{\rm i} = n`, and :math:`\nu_{\rm ei}` is
constant. Considering a steady state,

.. math::

   q n_{\rm e} \vec{E} - \nabla p - m_{\rm e} n_{\rm e} \nu_{\rm ei}
   \vec{v} = 0

 and so

.. math::

   \begin{aligned}
     \vec{v} &= \frac{1}{m_{\rm p} m_{\rm e} \nu_{\rm ei}} \qty( q n \vec{E} - k_{\rm B} T \nabla n_{\rm e} ) \\
   &= \frac{q}{m_{\rm e} \nu_{\rm ei}} \vec{E} - \frac{k_{\rm B} T}{m_{\rm e} \nu_{\rm ei}} \frac{\nabla n}{n} \\
   &= \mu \vec{E} - D \frac{\nabla n}{n}\end{aligned}

 where :math:`\mu` is the mobility coefficient, and :math:`D` the
diffusion coefficient. These differ for each species.

The flux, :math:`\vec{\Gamma}`, is

.. math:: \vec{\Gamma} = n \cdot \vec{v} = \pm \mu n\vec{E} - D \nabla n

 if either there is no :math:`\vec{E}`-field, or the particles are
uncharged we find Fick’s Law,

.. math::

   \label{eq:26}
     \vec{\Gamma} = -D \nabla n

 From the continuity equation,

.. math:: \pdv{n}{t} + \nabla \cdot \vec{\Gamma} = 0

 we can construct the diffusion equation,

.. math::

   \label{eq:27}
     \pdv{n}{t} - \nabla D \nabla n = 0

Ambipolar Diffusion
~~~~~~~~~~~~~~~~~~~

A plasma should be quasi-neutral, so diffusion of electrons and ions
should adjust to some degree to preserve quasineutrality. The
fast-moving electrons have higher thermal velocities and tend to leave a
plasma first. The positive charge is then left behind, and an electric
field is setup to retard the loss of electrons, and accelerate the loss
of ions. We let :math:`\vec{\Gamma}_{\rm e} =
\vec{\Gamma}_{\rm i} = \vec{\Gamma}`, so

.. math::

   \vec{\Gamma} = \mu_{\rm i} n \vec{E} - D_{\rm i} \nabla n =
   \mu_{\rm e} n \vec{E} - D_{\rm e} \nabla n

 and solving for :math:`\vec{E}` we find

.. math::

   \vec{E} = \frac{D_{\rm i} - D_{\rm e}}{\mu_{\rm i} + \mu_{\rm e}}
   \frac{\nabla n}{n}

 and the total flux is

.. math::

   \vec{\Gamma} = \mu_{\rm i} n \frac{D_{\rm i} - D_{\rm e}}{\mu_{\rm
       i}+\mu_{\rm e}} \frac{\nabla n}{n} - D_{\rm i} \nabla n = -
   \frac{\mu_{\rm i} D_{\rm e} + \mu_{\rm e} D_{\rm i}}{\mu_{\rm i} +
     \mu_{\rm e}} \nabla n

 Which is just Fick’s law again, with an additional coefficient,

.. math::

   D_{\rm a} = \frac{\mu_{\rm i} D_{\rm e} + \mu_{\rm e}D_{\rm
       i}}{\mu_{\rm i} + \mu_{\rm e}}

 which is the ambipolar diffusion coefficient.

Kinetic Theory of Plasmas
-------------------------

There are some phenomena which neither MHD nor single-particle
descriptions of a plasma can describe. For these situations we need to
consider the velocity distribution, :math:`f(\vec{v})` of the plasma. In
fluid theory the independent variables are functions of :math:`\vec{r}`
and :math:`t` only, which is because the velocity distribution is taken
to be Maxwellian everywhere, so can be uniquely speciied by the
temperature, :math:`T`, and the number density, :math:`n(\vec{r}, t)`,

.. math::

   n(\vec{r}, t) = \int f(\vec{r}, \vec{v}, t) \d[3]{V} = \int
   f(\vec{r}, \vec{v}, t) \dd[3]{V}

If :math:`f` is correctly normalised it describes the probbaility of
finding a particle in the range :math:`\vec{r}
\in (\vec{r}, \vec{r}+\dd{\vec{r}})` and :math:`\vec{v} \in (\vec{v},
\vec{v}+\dd{\vec{v}})`. :math:`f` is a function in seven variables, and,
if it is a Maxwellian distribution, it has the form,

.. math::

   \label{eq:28}
     f(\vec{r}, \vec{v}, t) = n(\vec{r}, t) \frac{m}{(2 \pi k T)^{\frac{3}{2}}} \exp( - \frac{v^2}{v_{\rm th}^2})

 for

.. math:: v_{\rm th} = \qty(\frac{2kT}{m})^{\half}

Ignoring collisions, and assuming the plasma to be a closed system, with
no sources or sinks of particles, the function will obey the Liouville
theorem, so

.. math:: \dv{f}{t} = 0

for the time derivative along a trajectory in
:math:`(\vec{r}, \vec{v})`-phase space, so

.. math::

   \begin{aligned}
     \dv{f}{t} = \pdv{f}{t} + \dv{\vec{r}}{t} \pdv{f}{\vec{r}} + \dv{\vec{v}}{t} \pdv{f}{\vec{v}} &= 0 \\
   \pdv{f}{t} + \vec{v} \pdv{f}{\vec{r}} + \frac{\vec{F}}{m} \pdv{f}{\vec{v}} &= 0\end{aligned}

 which is the kinetic equation for the plasma. If the force is entirely
electromagnetic the equation takes the form

.. math::

   \label{eq:29}
     \pdv{f}{t} + \vec{v} \pdv{f}{\vec{r}} + \frac{q}{m} \qty( \vec{E} + \vec{v} \times \vec{B}) \pdv{f}{\vec{v}} = 0

 which is the Vlasov equation. This should be completed with the system
of Maxwell’s equations, as :math:`\vec{E}` and :math:`\vec{B}` are the
average values of the electric and magnetic fields from particles in the
plasma.

If there are collisions in the plasma, :math:`\dv{f}{t}\neq 0`, and,
using the collision integral,

.. math::

   \label{eq:30}
     \pdv{f}{t} + \vec{v} \pdv{f}{\vec{r}} + \frac{\vec{F}}{m} \pdv{f}{\vec{v}} = \qty( \pdv{f}{t} )_{\rm coll}

 which is the Boltzmann equation. The kinetic equation can be modified
to include sources or sinks of particles by adding terms on the right
hand side.

The collision term can sometimes be approximated as

.. math:: \qty( \pdv{f}{t} )_{\rm coll} = \frac{f_{\rm eq} - f}{\tau}

 where :math:`f_{\rm eq}` is the equilibrium function, and :math:`\tau`
is the collision time. This is the Krook collision term.

Plasma waves and Landau Damping
-------------------------------

As an illustration of the use of the Vlasov equation, we consider the
electron plasma oscillations in a uniform plasma with no applied
magnetic or electric fields. Consider a first order perturbation,

.. math::

   f(\vec{r}, \vec{v}, t) = f_0(\vec{r}, \vec{v}, t) + f_1(\vec{r},
   \vec{v}, t)

 the first order Vlasov equation for electrons is

.. math::

   \pdv{f_1}{t} + \vec{v} \nabla f_1 = \frac{e}{m} \vec{E}_1
   \pdv{f_0}{\vec{v}} =0

 where :math:`E_1` is a perturbation of the electric field. Using
Poisson’s equation (:math:`\epsilon_0 \nabla \vec{E} = \rho`),

.. math:: \epsilon_0 \nabla \vec{E}_1 = -e n_1 = -e \int f_1 \dd[3]{V}

 As before assume the ions are massive and immobile, and assume the
waves in the plasma are plane waves in the :math:`x`-direction. Then,

.. math:: f_1 = f_0 \exp(- i \omega t + i k x)

.. math:: E_1 = E_x \exp( - i \omega t + i k x)

 Then we can write

.. math:: - i \omega f_1 + i k v_x f_1 = \frac{e}{m} E_x \pdv{f_0}{v_x}

 from the Vlasov equation, and

.. math:: \epsilon_0 i k E_x = - \int f_1 \dd[3]{V}

 from Poisson’s equation. Combining the two,

.. math::

   \begin{aligned}
     1 & = - \frac{e^2 }{l m \epsilon_0} \int \frac{\pdv{f_0}{v_x}}{\omega- k v_x} \dd[3]{V} \\
     &= - \frac{e^2}{k m \epsilon_0} \int_{-\infty}^{\infty} \dd{v_z}
     \int_{-\infty}^{\infty} \dd{v_y} \int \frac{\pdv{f_0}{v_x}}{\omega-
       k v_x} \dd{v_x}\end{aligned}

 If :math:`f_0` is Maxwellian the integration over :math:`v_y` and
:math:`v_z` can be carried out, and

.. math::

   f_0(v_x) = n_0 \frac{m}{(2 \pi k_{\rm B} T)^{\half}} \exp( -
   \frac{m v_x^2}{2 k_{\rm B} T} )

 Taking the normalised function :math:`\tilde{f} = \frac{f_0}{n_0}`,

.. math::

   1 = \frac{\omega_{\rm pe}^2}{k^2} \int_{-\infty}^{\infty}
   \frac{\pdv{\tilde{f}_0}{v_x}}{v_x - \frac{\omega}{k}} \dd{v_x}

 This integral is non-trivial to compute, due to the singularity at
:math:`v_x =
\frac{\omega}{k}`. Landau suggested (1946) letting
:math:`\omega \to \omega
+ i o` for a small :math:`o`, which makes the integral

.. math::

   \int_{-\infty}^{\infty} \frac{y(z)}{z-io} \dd{z} = P
   \int_{-\infty}^{\infty} \frac{f(z)}{z} \dd{z} + i \pi f(0)

 where :math:`P` denotes the Cauchy principle value of the integral.
This can be written symbolically as

.. math:: \frac{1}{z-io} = P \frac{1}{z} + i \pi \delta(z)

 and then, using the Landau rule, and letting :math:`v := v_x`,

.. math::

   \label{eq:31}
     1 = \frac{\omega_{\rm pe}^2}{k^2} \qty[ P \int_{-\infty}^{\infty} \frac{\pdv*{\tilde{f}_0}{v}}{v - \frac{\omega}{k}} + i\eval{\pi \pdv{\tilde{f}_0}{v} }_{v = \frac{\omega}{k}}]

First, concentrate on the real part, where the integral can be computed
by integrating by parts,

.. math::

   \begin{aligned}
   \int_{-\infty}^{\infty} \pdv{\tilde{f}_0}{v} \frac{\dd{v}}{v - \frac{\omega}{k}} 
   &= \eval{\frac{\tilde{f}_0 \dd{v}}{(v - \frac{\omega}{k})^2}}_{-\infty}^{\infty} - \int - \frac{\tilde{f}_0 \dd{v}}{\qty(v - \frac{\omega}{k})^2} \\ 
   &= \int_{-\infty}^{\infty} \frac{\tilde{f}_0 \dd{v}}{\qty( v - \frac{\omega}{k})^2}\end{aligned}

 We can assume :math:`\frac{\omega}{k} \gg v` (i.e. large phase
velocities), and so we can expand :math:`(v - \frac{\omega}{k})^{-2}`,

.. math::

   \begin{aligned}
    (v - \frac{\omega}{k})^{-2} &= \qty( \frac{\omega}{k} )^{-2} \qty( 1 - \frac{v k}{\omega})^{-2} \\
   &= \qty( \frac{\omega}{k} )^{-2} \qty( 1 + \frac{2 v k}{\omega} + \frac{3(vk)^2}{\omega^2} + \cdots )\end{aligned}

And now, using the expansion for the integral,

.. math::

   \begin{aligned}
     \int_{-\infty}^{\infty} \frac{\tilde{f}_0 \dd{v}}{\qty( v - \frac{\omega}{k})^2} &= \qty( \frac{\omega}{k} )^{-2} \int_{- \infty}^{\infty} \qty( 1 + \frac{2 v k}{\omega} + \frac{3(vk)^2}{\omega^2} + \cdots ) \tilde{f}_0 \dd{v}\end{aligned}

 The odd terms in :math:`v` will vanish, and

.. math:: \int_{-\infty}^{\infty} v^2 \tilde{f}_0 \dd{v}

 is just an average, so assuming :math:`\tilde{f}_0` is Maxwellian,

.. math:: \int_{-\infty}^{\infty} v^2 \tilde{f}_0 \dd{v} = \frac{k_{\rm B}T_{\rm e}}{m}

Then we can write

.. math:: 1 = \frac{\omega_{\rm pe}^2}{k^2} \qty[ \qty(\frac{\omega}{k})^{-2} \qty(1+ \frac{3 k_{\rm B} T_{\rm e} k^2}{m \omega^2})] = \frac{\omega_{\rm pe}^2}{\omega^2} \qty( 1+ \frac{3 k_{\rm B} T_{\rm e} k^2}{m \omega^2} )

 If the thermal correction is small we can replace :math:`\omega^2` with
:math:`\omega_{\rm pe}^2` in the second term, so

.. math::

   \label{eq:32}
     \omega^2(k) \approx \omega_{\rm pe}^2 + \frac{3 k_{\rm B} T_{\rm e}}{m} k^2

 This is the dispertion relation for Langmuir waves. The phase speed is

.. math:: v_{\rm p} = \frac{\omega}{k} \approx \frac{\omega_{\rm pe}}{k}

 and the group velocity is

.. math::

   v_{\rm g} = \pdv{\omega}{k} \approx \frac{3 k_{\rm B} T_{\rm e}}{m}
   k

 (assuming that :math:`\omega(k) \approx \omega_{\rm pe} + \frac{3}{2}
\frac{k_{\rm B} T_{\rm e}}{m} \frac{k^2}{\omega_{\rm pe}}`). Then, the
group velocity is

.. math::

   v_{\rm g} \approx 3 \frac{k_{\rm B}T_{\rm e}}{m}
   \frac{k}{\omega_{\rm pe}} \approx 3 \frac{k_{\rm B} T_{\rm e}}{m}
   \frac{1}{v_{\rm p}} \approx 3 \frac{v_{\rm Te}^2}{v_{\rm p}}

Finally, the imaginary part. For simplicity ignore the thermal
correction, so :math:`\omega(k) \approx \omega_{\rm pe}`, then

.. math::

   1 = \frac{\omega_{\rm pe}^2}{\omega^2} + i \pi \frac{\omega_{\rm
       pe}^2}{k^2} \eval{\pdv{\tilde{f}_0}{v}}_{v=\frac{\omega}{k}}

 and so

.. math::

   \omega^2 = \omega_{\rm pe} \qty( 1 - i \pi \frac{\omega_{\rm
       pe}^2}{k^2} \eval{ \pdv{\tilde{f}_0}{v} }_{v=\frac{\omega}{k}}
   )^{-1}

 Then, assuming that the imaginary part is small,

.. math::

   \label{eq:33}
     \omega(k) = \omega_{\rm pe} + i \omega_{\rm pe} \frac{\pi}{2} \frac{\omega_{\rm pe}^2}{k} \eval{\pdv{\tilde{f}_0}{v}}_{v = \frac{\omega}{k}}

 which is Landau damping. Substituting the one-dimensional Maxwellian
distribution for :math:`\tilde{f}`,

.. math::

   \begin{aligned}
   \pdv{\tilde{f}}{v} &= \qty( \pi v_{\rm Th}^2 )^{- \half} \exp( - \frac{v^2}{v_{\rm Th}^2}) \qty( - \frac{2v}{v_{\rm Th}^2}) \\ &\approx - \frac{2v}{\sqrt{\pi} v_{\rm Th}^3} \exp( - \frac{v^2}{v_{\rm Th}^2} ) \end{aligned}

 The using the knowledge that :math:`v= \frac{\omega}{k} \approx
\frac{\omega_{\rm pe}}{k}`,

.. math::

   \begin{aligned}
     \gamma_k = \Im(\omega) &= - \frac{\pi}{2} \frac{\omega_{\rm pe}^3}{k^2} \frac{2 \omega_{\rm pe}}{k \sqrt{\pi}} \frac{1}{v_{\rm Th}^3} \exp( - \frac{\omega_{\rm pe}^2}{k^2 v_{\rm Th}^2} ) \nonumber\\
   &= - \sqrt{\pi} \omega_{\rm p} \qty( \frac{\omega_{\rm pe}}{k v_{\rm Th}})^3 \exp( - \frac{\omega_{\rm pe}}{k^2 v_{\rm Th}^2})\end{aligned}

 Which is Landau damping. A useful equation derived from this is then

.. math::

   \label{eq:34}
     \Im\qty(\frac{\omega}{\omega_{\rm pe}}) \approx -0.22 \sqrt{\pi} \qty( \frac{\omega_{\rm pe}}{k v_{\rm Th}})^3 \exp(- \frac{1}{2k^2 \lambda^2_{\rm De}} )

 The discovery of wave damping without collisional dissipation has been
described as “probably the most astounding result of plasma physics.”

The damping is not reandomisation by collisions, but a resonant
(i.e.phase velocity of waves is the same as the velocity of interacting
particles) :math:`v=\frac{\omega}{k}` transfer of energy from waves to
particles. It can be reversed if :math:`\pdv*{\tilde{f}_0}{v}>0`.

Plasma and Radiation
====================

Plasma Radiation
----------------

in 0,30,...,360 (B) (0,0)+(:7); (0,0) +(:7) – +(:10); (0,0) circle (7);

(0,0) circle (5); in 0,30,...,360 (2,0) – (:5) coordinate (A);

(0,0) node [fill=accent-blue, circle] 1; (2,0) node [fill=accent-green,
circle] 2;

in 0,30,...,360 (0,0)+(:5) – +(:7);

(0,.6) – (2,.6) node [above, midway] :math:`\Delta v \ t`;

(0,-.6) – (-5,-.6) node [fill=white, midway] :math:`r = ct`; (-170:5) –
(-170:7) node [below, yshift=-.1cm, midway]
:math:`r^{\prime} = c \Delta t`;

| Charged particles will emit electromagnetic radiation if they
  accelerate during their motion. An example of accelerated motion in a
  plasma is the gyromotion of particles; radiation from the gyromotion
  is generally called synchotron radiation. Extagalactic jets, solar
  flares, and supernova remnants all show this behaviour.
| To understand how this radiation is produced, consider a charge,
  :math:`q` at a time :math:`t=0`, which is stationary at the origin of
  a laboratory rest frame. The electric field of the charge can be
  visualised as lines radiating from the charge. Now, let the particle
  accelerate to :math:`\Delta
  \vec{v}` in a time :math:`\Delta t`. We assume that
  :math:`\abs{ \Delta \vec{v} }
  \ll c`, so that relativistic corrections are small. After the
  acceleration the field of the particle will be radial about its new
  location. This field extends a distance of :math:`r = ct` from the new
  location of the charge. The old field will continue to exist in the
  region :math:`r> c(t + \Delta t)`. In the region between these two
  there is a thin shell, with thickness :math:`c \Delta t` where the
  field lines from the before and after cases must join up. As a result
  there must be a non-radial component of :math:`\vec{E}` in this
  region, and this constitutes a propogating pulse of electromagnetic
  field.
| The electric field lines are radial at :math:`t=0` and :math:`t=T`,
  but they have different origins. The lines joining the old and new
  field lines have a non-radial electric field component,
  :math:`\vec{E}_{\phi}`, in addition to the radial component
  :math:`\vec{E}_{r}`.

The radial component has the usual form,

.. math:: \vec{E}_r = \frac{q}{4 \pi \epsilon_0} \frac{\vec{r}}{r^2}

while the :math:`\vec{E}_{\phi}` component is given by the number of
radial field-lines per unit area in the direction of :math:`\vec{\phi}`.
From geometry arguments,

.. math::

   \label{eq:9}
     \frac{E_{\phi}}{E_r} = \frac{\Delta v t \sin(\phi)}{c \Delta t}

 then, since :math:`t = \frac{r}{c}`,
:math:`\frac{\Delta v}{\Delta t} = \ddot{r}`, and substituting
:math:`\vec{E}_r`,

.. math::

   \label{eq:10}
     E_{\phi} = \ddot{r} \sin(\phi) \frac{q}{4 \pi \epsilon_0} \frac{1}{c^2 r}

 :math:`\vec{E}_{\phi}` is known as the *acceleration field*, and has a
strength varying with :math:`\frac{1}{r}`, in contrast to the radial
field which varies with :math:`\frac{1}{r}`. This “kink” is an outward
moving pulse of electromagnetic radiation. The power per unit area per
second is given by the Poynting vector,

.. math::

   \vec{S} = \frac{\vec{E} \times \vec{B}}{\mu_0} = c \epsilon_0 E^2
   \hat{r}

 The total energy radiated per second then becomes

.. math::

   P(t) = \int \vec{S} \cdot \dd{\vec{A}} = \int \vec{S} r^2
   \dd{\vec{\Omega}}

 Recalling that for a sphere,
:math:`\dd{\Omega} = 2 \pi \sin(\phi) \dd{\phi}`,

.. math::

   \label{eq:11}
     P(t) = \frac{q^2 |\ddot{r}|^2}{6 \pi \epsilon_0 c^3}

 which is Larmour’s formula. This is a general expression for the
radiated power from an accelerated charge, and can be applied to our
specific case of a particle gyrating in an electric field.

Cyclotron Radiation
~~~~~~~~~~~~~~~~~~~

Consider the rest frame of a charge :math:`q`, called
:math:`S^{\prime}`, and a lab frame :math:`S`.

.. math:: \text{In the $S$ frame} \quad m \dv{\vec{v}}{t} = q \vec{v} \times \vec{B}

.. math::

   \text{In the $S^{\prime}$ frame} \quad m
   \dv{\vec{v}^{\prime}}{t^{\prime}} = q \vec{B}^{\prime}

 The electric field :math:`E^{\prime} = v \gamma B \sin(\theta)` (with
:math:`\theta` the electron pitch angle) due to the relativistic
transformations of :math:`\vec{E}` and :math:`\vec{B}`. Using Larmour’s
formula,

.. math::

   \begin{aligned}
     P(t)^{\prime} &= \frac{q^2 \abs{\dot{v}^{\prime}}^2}{6 \pi
       \epsilon_0 c^3}\\ &= \frac{q^2}{6 \pi \epsilon_0 c^3}
     \frac{q^2}{m^2} \abs{\vec{B}^{\prime}}^2 \\ &= \frac{q^4}{6 \pi
       \epsilon_0 c^3 m^2} (v \gamma B)^2 \sin[2](\theta)\end{aligned}

 This gives the power radiated in the rest frame of the electron. Power
is Lorentz invariant (:math:`P = P^{\prime}`), so the power in the lab
frame must be the same. The total power radiated in the lab frame from a
particle with pitch anfgle :math:`\theta` is

.. math::

   P = \frac{q^4 B^2}{6 \pi \epsilon_0 c m^2} \gamma^2 \beta
   \sin[2](\theta)

 for :math:`\beta = \frac{v}{c}`. and simplifying,

.. math:: P = 2 \sigma_{\rm T} c U_{\rm mag} \gamma^2 \sin[2](\theta)

 with :math:`\sigma_{\rm T}` the Thomson cross-section,
:math:`U_{\rm mag} =
\frac{B^2}{2 \mu_0}`.

The distribution of the radiation about the moving charge is worth
considering;

.. math::

   \label{eq:12}
     \dv{P}{\Omega} = c \epsilon_0 \frac{q^2}{(4 \pi \epsilon_0)^2} \frac{(\ddot{r})^2}{c^4} \sin[2](\phi)

 this is a dipole emission pattern.

If the particle is relativistic we must consider the effect on the
cyclotron frequency. The relativistic frequency will be

.. math::

   \omega_{\rm r} = \frac{\omega_{\rm c}}{\gamma} =
   \frac{\abs{q}B}{\gamma m_0}

where :math:`m_0` is the rest-mass of the particle. This can be
decomposed into a series of harmonics, :math:`\omega_n`,

.. math::

   \omega_n = \frac{n \omega_{\rm r}}{\qty(1 - \beta_{\parallel}
     \cos(\theta) )}

 As a result, the spectrum of highly relativistic electrons will be
distinctly different from the delta-function peak we expect from a
non-relativistic charge. A distribution of electrons will in fact
display a power-law spectrum. As the charge becomes more relativistic
the dipole shape of the radiation is deformed, and an effect known as
“relativistic beaming” will be observed, with the output of radiation
becoming more and more focussed.

Faraday Rotation in a Cold Plasma
---------------------------------

| Parallel to a uniform magnetic field, :math:`\vec{B}_0` there are two
  electromagnetic modes (cold plasma modes), where

  .. math:: n^2 = R \qquad n^2 = L \quad L \neq R

  thus different polarisations have different phase speeds—we can
  exploit this as a remote diagnostic of the plasma conditions.
| Consider two circuarly polarised modes, :math:`n^2 = \{R, L \}`, then

  .. math:: n^2 = \frac{k^2 c^2}{\omega^2}

  Thus it is possible to convert between :math:`n` and
  :math:`\frac{\omega}{k}`. A superposition of the circuarly polarised
  waves produces an evolution along the propogation ray of the net
  :math:`\vec{E}` polarisation direction.

(0,-4.4) – (7,-4.4) node [midway, below] :math:`z`;

(0,0) circle (2); (0,-2) – (0,2) node [midway, right, black]
:math:`\vec{E}`; (2,4) node [text width=3cm, left, text ragged] At
:math:`z=0` :math:`R` and :math:`L` are synchronised, producing a
vertical polarisation.; (-1,-3) circle (.8) node :math:`R`; (1,-3)
circle (.8) node :math:`L`; (-1,-2.2) circle (0.1); (1,-2.2) circle
(0.1); (-1,-2) arc (90:135:1); (1,-2) arc (270:225:-1);

(0,4) node [text width=3cm, text ragged] As :math:`z` increases,
:math:`R` and :math:`L` the faster rotation of the :math:`L` mode causes
the polarisation to become diagonal.; (0,0) circle (2); (0,-2) – (0,2)
node [midway, right, black] :math:`\vec{E}`;

(-1,-3) circle (.8) node :math:`R`; (1,-3) circle (.8) node :math:`L`;
(-1,-2.2) circle (0.1); (1,-2.2) circle (0.1); (-1,-2) arc (90:135:1);
(1,-2) arc (270:225:-1);

Suppose the polarisation vector :math:`\vec{E}` shifts by an angle
:math:`\dd{\theta}` as a result of the varying phase interference of the
superposed :math:`R` and :math:`L` modes. Then,

.. math:: \dd{\theta} = \frac{1}{2} (k_L - k_R) \dd{z}

| Considering the special case of an electron plasma, with
  :math:`\omega \gg
  \omega_{\rm c_e}`, we can see that :math:`n^2 = \{R,L\}` are

  .. math::

     \begin{aligned}
       R & = 1 - \frac{\omega_{\rm p}^2}{\omega(\omega-\omega_{\rm c_e})} \\
       L & = 1 - \frac{\omega_{\rm p}^2}{\omega(\omega+\omega_{\rm c_e})}\end{aligned}

   with :math:`\omega_{\rm c_+} \to 0`, as :math:`m_+ \to \infty`. Thus

  .. math::

     \begin{aligned}
       \eval{n}_{\rm RCP} &\approx 1 - \frac{\omega_{\rm p}^2}{2 \omega (\omega-\omega_{\rm c_e})} \\
       \eval{n}_{\rm LCP} &\approx 1 - \frac{\omega_{\rm p}^2}{2 \omega(\omega+\omega_{\rm c_e})}\end{aligned}

   Then

  .. math::

     \begin{aligned}
       (n_R - n_L) &= \frac{\omega_{\rm p}^2}{2 \omega} \qty[ \frac{1}{\omega - \omega_{\rm c_e}} - \frac{1}{\omega(\omega+\omega_{\rm c_e})}]\\
     &= \frac{\omega_{\rm p}^2}{2 \omega} \frac{\omega + \omega_{\rm c_e}-(\omega-\omega_{\rm c_e})}{\omega^2 - \omega_{\rm c_e}^2} \\
     &= \frac{\omega_{\rm p}^2 \omega_{\rm c_e}}{\omega(\omega^2-\omega_{\rm c_e}^2)} \\
     &\approx \frac{\omega_{\rm p}^2 \omega_{\rm c_e}}{\omega^3} \\\end{aligned}

   Hence,

  .. math::

     \begin{aligned}
       \dd{\theta} &= \half \qty| (k_R - k_L)| \dd{z} \\
     & \approx \half \int_0^2 \frac{\omega_{\rm p}^2 \omega_{\rm c_e} \dd{z}}{c \omega^2} \\
     &= \half \int_0^2 \frac{ \frac{ne^2}{m_{\rm e}^2} \frac{eB}{m_{\rm e}}}{ c \omega^2} \dd{z}\\
     &= \frac{e^2}{2 \epsilon_0 m_{\rm e}^2 c \omega^2} \int_0^2 nB \dd{z}\end{aligned}

   We could allow :math:`n` and :math:`B` to vary slowly, i.e. with the
  gradient-scale length of :math:`n,B` much greater than the wavelength
  of the circular poalrisation modes, and still have a Faraday rotation
  result which is reasonably slow.
| When observing the wave we can only make a detection at one point in
  the propogation path, but using the frequency dependence we can detect
  polarisation variation by measuring the polarisation at multiple
  frequencies.
| Using Faraday rotation allows the measurement of
  :math:`\int nB \dd{z}` along the line-of-sight path as a function of
  frequency. Suppose we have a system with a plasma between the observer
  and a multispectral event. We set off a flash which travels through
  the plasma, and observe the radiation on the far side. Plasma slows
  different frequencies to a different degree, so the time elapsed
  between different frequencies allows the line-of-sight integrated
  number density to be found, which in turn allows the integrated
  line-of-sight magnetic field to be found, which can be used to make
  maps of magnetic fields.

We can generalise this result, with

.. math::

   \label{eq:faradayangle}
     \theta_{\rm F} = \frac{1}{\omega^2} \frac{e^3}{2 \epsilon_0 m_{\rm e}^2 c} \int_0^z n B \cos \theta \dd{z'}

 with :math:`\theta_{\rm F}` being the angle between the full magnetic
field direction and the line-of-sight direction.

| For a cold plasma we have the dispertion relation in equation
  ([eq:dispertion]), for a wave with :math:`\omega \gg \omega_{\rm p}`
  and :math:`\omega \gg \omega_{\rm ci}`,

  .. math::

     \begin{aligned}
       S &= \half \qty( 1 + \frac{\omega_{\rm p}^2}{(\omega + \omega_{\rm ci})(\omega_{\rm ei}-\omega)} + 1 - \frac{\omega_{\rm p}^2}{(\omega - \omega_{\rm ei})(\omega+\omega_{\rm ce})}) \\
     &= \half \qty( 2+ \omega_{\rm p}^2 \frac{(\omega-\omega_{\rm ci})(\omega+\omega_{\rm ce}) - (\omega+\omega_{\rm ci})(\omega_{\rm ce}-\omega)}{(\omega^2-\omega_{\rm ci}^2)(\omega_{\rm ce}^2 - \omega^2)}) \\
     &= \half \qty( 2+ \omega_{\rm p}^2  \frac{\omega \qty(\omega+\omega_{\rm ce} - (\omega_{\rm ce}-\omega))}{\omega^2(\omega_{\rm ce}^2 - \omega^2)})\\
     &= \half \qty( 2+ \omega_{\rm p}^2 \frac{2 \omega^2}{\omega^2 \qty(\omega_{\rm ce}^2 - \omega^2)} )\\
     &= \half \qty( 2+ \omega_{\rm p}^2 \frac{2 \omega^2}{\omega^2 \qty(\omega^2_{\rm ce} - \omega^2)}) \\
     &= 1 + \frac{\omega_{\rm p}^2}{\qty( \omega_{\rm ce}^2 - \omega^2)}\end{aligned}

   Now introducing :math:`\Gamma_{\rm p} := \frac{\omega_{\rm
      p}^2}{\omega^2_{\rm ce} - \omega^2}`, finally,

  .. math::

     \begin{aligned}
       S &= \half (R+L) = 1+r_{\rm p}\\
     D &= \half (R-L) = r_{\rm p} \frac{\omega_{\rm ce}}{\omega}\\
     P &= 1 - \frac{\omega_{\rm p}^2}{\omega^2} \approx S\end{aligned}

   In the limit :math:`\omega \gg \omega_{\rm ce}`. The general cold
  plasma dispertion relation is equation ([eq:dispertionrelation]),
  which can be solved for :math:`n^2`,

  .. math::

     \begin{aligned}
     n^2 &= \frac{2 PS +(RL-PS)(\sin[2](\theta)) \pm \sqrt{(RL-PS)^2 \sin[4](\theta)} }{{2 \qty[ P+(S-P) \sin[2](\theta)]}} \\& \quad+ \frac{{4 P^2D^2 \cos[2](\theta)}}{2 \qty[ P+(S-P) \sin[2](\theta)]} \end{aligned}

   In the limit :math:`\omega \gg \omega_{\rm ce}`, :math:`P \approx S`
  and

  .. math:: RL - PS \approx  RL -S^2 = -D^2

   hence

  .. math::

     \begin{aligned}
       n_{\pm}^2 &= \frac{2 S^2 - D^2 \sin[2](\theta) \pm \sqrt{D^4 \sin[4](\theta) + 4 S^2 D^2 \cos[2](\theta)}}{2S}\end{aligned}

   where the :math:`\pm` corresponds to the right and left polarisations
  respectively. We can further simplify for small angles of wave
  propogation, so :math:`\cos(\theta)\approx 1` and :math:`v \approx 0`.

  .. math::

     \begin{aligned}
      n_{\pm}^2 &\approx S \pm D \cos(\theta) \\
     & \approx 1 + r_{\rm p} \pm r_{\rm p} \frac{\omega_{\rm ce}}{\omega} \cos(\theta) \\
     & \approx \frac{\omega_{\rm ce}^2 - \omega^2 + \omega_{\rm p}^2}{\omega_{\rm ce}^2 - \omega^2} \pm \frac{\omega_{\rm p}^2}{\omega_{\rm ce}^2 -\omega^2} \frac{\omega_{\rm ce}}{\omega} \cos(\theta) \\
     & \approx 1  \mp \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{\omega^3} \cos(\theta)\end{aligned}

   For :math:`\omega^2 \gg \omega_{\rm p}^2`,
  :math:`\omega^2 \gg \omega_{\rm ce}^2`. Then

  .. math::

     \begin{aligned}
       n_+ & \approx \qty( 1 - \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{\omega^3} \cos(\theta))^{\half} \approx 1 - \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{2 \omega^3 \cos(\theta)} \\
       n_- & \approx \qty( 1+ \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{\omega^3} \cos(\theta) )^{\half} \approx 1 + \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{2 \omega^3} \cos(\theta)\end{aligned}

   And so,

  .. math:: \Delta n = n_- - n_+ \approx \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{\omega^3} \cos(\theta)

   Since :math:`n = \frac{kc}{\omega}`, we know
  :math:`k = \frac{\omega}{c} n`, and so

  .. math::

     \begin{aligned}
       K_- - K_+ \approx \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{c \omega^2} \cos(\theta) \end{aligned}

   and so finally, the rotation angle is

  .. math::

     \label{eq:13}
       \dd{\phi} = \half \frac{\omega_{\rm p}^2 \omega_{\rm ce}}{c \omega^2} \cos(\theta) \dd{z}

   At the high wave frequency limit,

  .. math:: \omega = k c = \frac{2 \pi c}{\lambda}

   Hence, as :math:`\omega_{\rm p}
  = \sqrt{\frac{4 \pi e^2 n_{\rm e}}{4 \pi m \epsilon_0}}`, and
  :math:`\omega_{\rm c} = \frac{eB}{m}`,

  .. math::

     \begin{aligned}
       \dv{\phi}{z} &=  \half \frac{e^2 n }{m \epsilon_0} \frac{eB}{m} \frac{1 \lambda^2}{c (2 \pi)^2 c^2} \cos(\theta) \\
     &= \frac{e^3 B n_{\rm e} \lambda^2}{8 \pi^2 m^2 \epsilon_0 c^3} \cos(\theta)\end{aligned}

   And then, to find the Farday angle after the radiation has travelled
  along a path :math:`r`,

  .. math::

     \label{eq:14}
       \phi_{\rm F} = \frac{e^3  \lambda^2}{8 \pi^2 m^2 \epsilon_0 c^3} \int_0^r B(z) n_{\rm e}(z) \cos(\theta) \dd{z}

   Assuming a uniform number density the Faraday rotation is a measure
  of the magnetic field along the path.
| Faraday rotation occurs because light which is polarised in the
  direction of electron gyration has a higher phase speed than that
  which is polarised in the opposing direction. The rotation is higher
  for low-frequency waves.

.. [1]
   Air generally has around :math:`10^{9} {\rm m}^{-3}` ions and
   electrons which are caused by background sources and friction. These
   can be harnassed as seeds for further ionisation.
