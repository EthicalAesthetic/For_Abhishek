# B.Sc. (Hons.) Physics - Semester I
## Mechanics (2024-2025) 
### Complete Solutions

**Duration:** 3 Hours | **Maximum Marks:** 90

---

## Question 1: Short Answer Questions (18 marks)

### (a) Three Freight Trucks Problem (3 marks)

**Question:** Three freight trucks of mass $m$ each are pulled with force $F$ by a locomotive. Find the forces on each car.

**Solution:**

Let the tensions be $T_1$ (between locomotive and car 1), $T_2$ (between cars 1 and 2), and $T_3$ (between cars 2 and 3).

Total mass = $3m$
Acceleration: $a = \frac{F}{3m}$

**For Car 3:** 
$$T_3 = ma = \frac{F}{3}$$

**For Cars 2 and 3:**
$$T_2 = 2ma = \frac{2F}{3}$$

**For all three cars:**
$$T_1 = F$$

**Answer:** Forces are $\boxed{F, \frac{2F}{3}, \frac{F}{3}}$ respectively.

---

### (b) Moment of Inertia Definition (3 marks)

**Answer:**

**Moment of Inertia (I)** is the measure of resistance of a body to rotational motion about an axis. Mathematically:

$$I = \sum m_i r_i^2 = \int r^2 dm$$

where $r$ is the perpendicular distance from the axis.

**Physical Significance:**
- Rotational analog of mass in linear motion
- Determines the torque needed for angular acceleration: $\tau = I\alpha$
- Depends on mass distribution and axis of rotation
- Units: $kg \cdot m^2$

---

### (c) Work Done in Force Field (3 marks)

**Question:** Find work done in moving a particle in field $\vec{F} = 3x^2\hat{i} + (2xz-y)\hat{j} + z\hat{k}$ from $(0,0,0)$ to $(2,1,3)$.

**Solution:**

Check if field is conservative: $\nabla \times \vec{F} = 0$?

$$\nabla \times \vec{F} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ 3x^2 & 2xz-y & z \end{vmatrix}$$

$$= \hat{i}(0-2x) - \hat{j}(0-0) + \hat{k}(2z-0) = -2x\hat{i} + 2z\hat{k}$$

Since $\nabla \times \vec{F} \neq 0$, field is non-conservative. We need to integrate along the path.

Using straight line path: $\vec{r}(t) = (2t, t, 3t)$, $0 \leq t \leq 1$

$$d\vec{r} = (2dt, dt, 3dt)$$

$$\vec{F} \cdot d\vec{r} = 3(2t)^2(2dt) + (2(2t)(3t)-t)(dt) + 3t(3dt)$$
$$= 24t^2 dt + (12t^2 - t + 9t) dt = (24t^2 + 8t) dt$$

$$W = \int_0^1 (24t^2 + 8t) dt = [8t^3 + 4t^2]_0^1 = 8 + 4 = \boxed{12 \text{ J}}$$

---

### (d) Effective Weight of Astronaut (3 marks)

**Question:** Effective weight of 70 kg astronaut in rocket accelerating upward at $5g$.

**Solution:**

Apparent weight is normal force: $N = m(g + a)$

Where $a = 5g$ (upward acceleration)

$$N = 70(g + 5g) = 70 \times 6g = 420g$$

$$N = 420 \times 10 = \boxed{4200 \text{ N}}$$

Or in terms of weight multiples: $\boxed{6 \text{ times the normal weight}}$

---

### (e) Block Hitting Spring with Friction (3 marks)

**Question:** Block mass $M$, speed $V_0$ hits spring constant $k$. Friction coefficient $\mu = bx$. Find energy loss when block stops.

**Solution:**

Using energy conservation from $x = 0$ to maximum compression $x = x_{max}$:

Initial KE: $\frac{1}{2}MV_0^2$

Work by friction: $W_f = -\int_0^{x_{max}} bx \cdot Mg \, dx = -bMg\frac{x_{max}^2}{2}$

Spring PE: $\frac{1}{2}kx_{max}^2$

At maximum compression (v = 0):
$$\frac{1}{2}MV_0^2 = \frac{1}{2}kx_{max}^2 + bMg\frac{x_{max}^2}{2}$$

$$\boxed{\Delta E = bMg\frac{x_{max}^2}{2} = \text{Loss in mechanical energy}}$$

where $x_{max} = \sqrt{\frac{MV_0^2}{k + bMg}}$

---

### (f) Sphere vs Cylinder on Incline (3 marks)

**Question:** Which reaches bottom first: sphere or cylinder (same $M, R$) on incline?

**Solution:**

For rolling without slipping down incline of angle $\theta$:

$$a = \frac{g\sin\theta}{1 + \frac{I}{MR^2}}$$

**For sphere:** $I = \frac{2}{5}MR^2$, so $a_s = \frac{5g\sin\theta}{7}$

**For cylinder:** $I = \frac{1}{2}MR^2$, so $a_c = \frac{2g\sin\theta}{3}$

Comparing: $\frac{5}{7} \approx 0.714 > \frac{2}{3} \approx 0.667$

**Answer:** $\boxed{\text{Sphere reaches bottom first}}$ (greater acceleration)

---

### (g) Relativistic Velocity Addition (3 marks)

**Question:** Two spaceships flying apart at speed $0.99c$. Find speed of one relative to other.

**Solution:**

Using relativistic velocity addition:
$$v = \frac{v_1 + v_2}{1 + \frac{v_1v_2}{c^2}} = \frac{0.99c + 0.99c}{1 + \frac{(0.99c)^2}{c^2}}$$

$$= \frac{1.98c}{1 + 0.9801} = \frac{1.98c}{1.9801} = \boxed{0.9995c}$$

Compare to Galilean: $0.99c + 0.99c = 1.98c$ (impossible!)

---

## Question 2: Center of Mass and Rocket Motion (18 marks)

### (a) Center of Mass Location (2 marks)

**Question:** Does center of mass necessarily lie within the body? Give example.

**Answer:** **No.** 

**Example:** Ring or hollow sphere - the center of mass lies at the geometric center, which is outside the material body itself.

---

### (b) Bomb Shell Explosion (6 marks)

**Question:** Shell explodes mid-flight. Show CM continues along original path.

**Solution:**

For the unexploded shell, equation of motion:
$$m\vec{a}_{cm} = \vec{F}_{external} = m\vec{g}$$

$$\vec{a}_{cm} = \vec{g}$$

When shell explodes into fragments with masses $m_1, m_2, \ldots m_n$ and velocities $\vec{v}_1, \vec{v}_2, \ldots \vec{v}_n$:

The center of mass velocity:
$$\vec{v}_{cm} = \frac{\sum m_i \vec{v}_i}{\sum m_i}$$

The acceleration of CM:
$$\vec{a}_{cm} = \frac{\sum m_i \vec{a}_i}{\sum m_i}$$

Internal forces (explosion forces) cancel in pairs by Newton's third law. Only external force (gravity) acts:

$$\sum m_i \vec{a}_i = \sum m_i \vec{g} = (\sum m_i)\vec{g}$$

$$\vec{a}_{cm} = \vec{g}$$

Therefore, the CM follows the same parabolic path as the unexploded shell.

**Conclusion:** The center of mass continues on the original trajectory despite the explosion. ✓

---

### (c) Rocket Velocity Derivation (10 marks)

**Question:** Rocket starts from rest with initial mass $M_0$, reaches velocity $V$ with final mass $M$. Show: $V = u \ln\left(\frac{M_0}{M}\right)$

**Solution:**

**Equation of Motion:**

At time $t$, let rocket have mass $m$ and velocity $v$.

In time $dt$:
- Mass ejected: $dm$ (outward, velocity $v_e$ relative to rocket)
- Velocity of rocket: $v + dv$

**Momentum consideration:**

Initial momentum: $m \cdot v$

Final momentum: $(m - dm)(v + dv) + dm(v - u)$

where $u$ is exhaust velocity relative to ground.

By conservation: $mv = (m-dm)(v+dv) + dm(v-u)$

Expanding:
$$mv = mv + mdv - vdm - dmdv + vdm - udm$$

Neglecting second-order terms:
$$0 = mdv - udm$$

$$mdv = u \, dm$$

$$dv = u \frac{dm}{m}$$

Integrating from $M_0$ to $M$:
$$\int_0^V dv = \int_{M_0}^M u \frac{dm}{m}$$

$$V = u[\ln m]_{M_0}^M = u(\ln M - \ln M_0)$$

$$\boxed{V = u \ln\left(\frac{M_0}{M}\right)}$$

This is the **Tsiolkovsky rocket equation**.

---

## Question 3: Fictitious Forces and Kepler's Laws (18 marks)

### (a) Fictitious Forces Definition (2 marks)

**Answer:**

**Fictitious forces** (pseudo-forces) are apparent forces that arise in non-inertial (accelerating) reference frames.

**Examples:**
1. **Centrifugal force:** $m\omega^2 r$ (outward in rotating frame)
2. **Coriolis force:** $-2m\vec{\omega} \times \vec{v}$
3. **Inertial force:** $-m\vec{a}$ (in accelerating frame)

These are not real forces but consequences of analyzing motion in non-inertial frames.

---

### (b) Potential Energy Curve (3 marks)

**Answer:**

**Potential Energy Curve:** Graph of potential energy $U(r)$ vs separation $r$.

**Key Points:**

1. **Turning Point:** Where total energy equals potential energy ($E = U$), velocity = 0

2. **Equilibrium Points:** Where $\frac{dU}{dr} = 0$:
   - **Stable:** Minimum ($\frac{d^2U}{dr^2} > 0$) - small displacement → restoring force
   - **Unstable:** Maximum ($\frac{d^2U}{dr^2} < 0$) - small displacement → repulsive force
   - **Neutral:** Inflection point - marginally stable

3. **Forbidden regions:** Where $E < U$ (classically inaccessible)

---

### (c) Kepler's Laws and Satellite Velocity (12 marks)

**Kepler's First Law:** Planets move in elliptical orbits with Sun at one focus.

**Kepler's Second Law:** The radius vector sweeps equal areas in equal times.

**Derivation of Satellite Velocity:**

For circular orbit at radius $r$ around Earth (mass $M$):

Gravitational force provides centripetal force:
$$\frac{GMm}{r^2} = \frac{mv^2}{r}$$

$$v^2 = \frac{GM}{r}$$

$$\boxed{v = \sqrt{\frac{GM}{r}}}$$

**For Earth orbiting at radius $r$:**
$$v = \sqrt{\frac{GM_E}{r}}$$

Standard values:
- $G = 6.67 \times 10^{-11}$ N·m²/kg²
- $M_E = 5.97 \times 10^{24}$ kg
- For low Earth orbit ($r \approx 6.37 \times 10^6$ m): $v \approx 7.9$ km/s

---

## Question 4: Gravity and Rotating Frames (18 marks)

### (a) Effective Gravity Due to Earth's Rotation (10 marks)

**Question:** Find $g$ as function of latitude $\lambda$.

**Solution:**

The measured acceleration $g$ differs from true gravitational acceleration $g_0$ due to Earth's rotation.

At latitude $\lambda$:

**Gravitational acceleration (downward):** $g_0$

**Centrifugal acceleration (outward):** $\omega^2 R \cos\lambda$

Components:
- Radial (outward): $\omega^2 R \cos^2\lambda$
- Tangential (poleward): $\omega^2 R \sin\lambda \cos\lambda$

**Effective gravity magnitude:**
$$g = \sqrt{(g_0 - \omega^2 R\cos^2\lambda)^2 + (\omega^2 R\sin\lambda\cos\lambda)^2}$$

For small $\omega^2R$ compared to $g_0$:
$$\boxed{g = g_0 - \omega^2 R\cos^2\lambda}$$

where $\omega = \frac{2\pi}{T}$ is Earth's angular velocity, $T = 24$ hours.

**Variation:**
- At equator ($\lambda = 0$): $g = g_0 - \omega^2 R$ (minimum)
- At poles ($\lambda = 90°$): $g = g_0$ (maximum)

**Numerical values:**
- $\omega^2 R \approx 0.034$ m/s²
- Difference: $\approx 0.5\%$ of $g$

---

### (b) Angular Momentum Change (6 marks)

**Question:** Constant torque $\vec{\tau} = 4\hat{i} + 4\hat{j} + 6\hat{k}$ Nm acts. Initial $\vec{L}_0 = 2\hat{i} + 7\hat{j} + 8\hat{k}$ kg·m²/s. Find $\vec{L}$ after $t = 6$ s.

**Solution:**

Using: $\frac{d\vec{L}}{dt} = \vec{\tau}$

$$\vec{L}(t) = \vec{L}_0 + \vec{\tau} \cdot t$$

$$\vec{L}(6) = (2\hat{i} + 7\hat{j} + 8\hat{k}) + (4\hat{i} + 4\hat{j} + 6\hat{k}) \times 6$$

$$= (2\hat{i} + 7\hat{j} + 8\hat{k}) + (24\hat{i} + 24\hat{j} + 36\hat{k})$$

$$\boxed{\vec{L}(6) = 26\hat{i} + 31\hat{j} + 44\hat{k} \text{ kg·m}^2\text{/s}}$$

---

### (c) Moment of Inertia of Cube (2 marks)

**Question:** Find MI of uniform cube side $a$ about axis through center parallel to face.

**Solution:**

Using parallel axis theorem or direct integration:

$$I = \int y^2 dm$$

where $y$ is perpendicular distance from axis.

For axis parallel to face (say z-axis through center):

$$\boxed{I = \frac{Ma^2}{6}}$$

where $M$ is total mass.

(This is same as for a thin rod along diagonal.)

---

## Question 5: Elastic Collisions (18 marks)

### (a) Elastic Collision in CM Frame (7 marks)

**Question:** $m_1$ slides and collides elastically with stationary $m_2 = 3m_1$. CM speed before = 3 m/s. Find speeds after collision.

**Solution:**

**Before collision:**
- $v_1 = ?$, $v_2 = 0$
- $v_{cm} = \frac{m_1 v_1 + 0}{m_1 + 3m_1} = \frac{v_1}{4} = 3$ m/s

Therefore: $v_1 = 12$ m/s

**In CM frame:**

Velocities in CM frame:
- $v_1' = v_1 - v_{cm} = 12 - 3 = 9$ m/s
- $v_2' = v_2 - v_{cm} = 0 - 3 = -3$ m/s

Check: $m_1(9) + 3m_1(-3) = 9m_1 - 9m_1 = 0$ ✓ (CM velocity = 0 in CM frame)

**After elastic collision in CM frame:**

In CM frame, speeds reverse:
- $v_1'' = -9$ m/s
- $v_2'' = 3$ m/s

**Back to lab frame:**

$$v_1^{final} = v_1'' + v_{cm} = -9 + 3 = -6 \text{ m/s}$$

$$v_2^{final} = v_2'' + v_{cm} = 3 + 3 = 6 \text{ m/s}$$

**Answers:**
- **CM speed remains:** $v_{cm} = \boxed{3 \text{ m/s}}$
- **$m_1$ speed after:** $\boxed{6 \text{ m/s (backward)}}$
- **$m_2$ speed after:** $\boxed{6 \text{ m/s (forward)}}$

---

### (b) Conservative Force Field (3 marks)

**Question:** Position $\vec{R}(t) = a\cos(\omega t)\hat{i} + b\sin(\omega t)\hat{j}$. Show force is conservative.

**Solution:**

$$\vec{v} = -a\omega\sin(\omega t)\hat{i} + b\omega\cos(\omega t)\hat{j}$$

$$\vec{a} = -a\omega^2\cos(\omega t)\hat{i} - b\omega^2\sin(\omega t)\hat{j} = -\omega^2\vec{R}$$

$$\vec{F} = m\vec{a} = -m\omega^2\vec{R}$$

This is a central force (restoring force toward origin).

$$\nabla \times \vec{F} = 0$$ ✓

Therefore, force is **conservative**. (Derived from potential $U = \frac{1}{2}m\omega^2 R^2$)

---

### (c) Angular Momentum of Particle System (8 marks)

**Concept of Angular Momentum:**

For system of $n$ particles:
$$\vec{L}_{total} = \sum_{i=1}^{n} \vec{L}_i = \sum_{i=1}^{n} \vec{r}_i \times m_i\vec{v}_i$$

$$\vec{L}_{total} = \vec{L}_{cm} + \sum_{i=1}^{n} \vec{r}_i' \times m_i\vec{v}_i'$$

where primed quantities are relative to CM.

**In absence of external torque:**

$$\frac{d\vec{L}_{total}}{dt} = \vec{\tau}_{external} = 0$$

$$\boxed{\vec{L}_{total} = \text{constant}}$$

**Applications:**
1. Earth's orbit conservation
2. Spinning skater pulling arms in
3. Planetary motion
4. Atomic angular momentum

---

## Question 6: Relativity - Length Contraction (18 marks)

### (a) Meter Rod in Moving Frame (5 marks)

**Question:** Meter rod at 30° in frame moving at $v = 0.6c$ to rod. Find length and orientation.

**Solution:**

**Initial orientation:** 30° to x-axis

**Components:** 
- $L_{x0} = L_0\cos(30°) = \frac{\sqrt{3}}{2}$ m
- $L_{y0} = L_0\sin(30°) = 0.5$ m

**Lorentz contraction:** Only parallel to motion

$\gamma = \frac{1}{\sqrt{1-v^2/c^2}} = \frac{1}{\sqrt{1-0.36}} = \frac{1}{0.8} = 1.25$

$$L_x = \frac{L_{x0}}{\gamma} = \frac{0.866}{1.25} = 0.693 \text{ m}$$

$$L_y = L_{y0} = 0.5 \text{ m}$$ (perpendicular, no contraction)

**New length:**
$$L = \sqrt{L_x^2 + L_y^2} = \sqrt{0.693^2 + 0.5^2} = \sqrt{0.480 + 0.250} = \boxed{0.855 \text{ m}}$$

**New angle:**
$$\tan\theta' = \frac{L_y}{L_x} = \frac{0.5}{0.693} = 0.722$$

$$\theta' = \boxed{35.9°}$$

---

### (b) Why Particles Cannot Exceed $c$ (3 marks)

**Answer:**

From relativistic kinetic energy:
$$E_k = (\gamma - 1)mc^2 = \frac{mc^2}{\sqrt{1-v^2/c^2}} - mc^2$$

As $v \to c$: $\gamma \to \infty$

Therefore, $E_k \to \infty$

**Physical reason:** It would require infinite energy to accelerate any mass to light speed. Since energy is finite, $v < c$ always.

**For photons:** Massless particles travel at $c$ naturally (no acceleration needed).

---

### (c) Einstein's Velocity Addition (10 marks)

**Derivation:**

Consider two frames S and S', where S' moves with velocity $u$ relative to S.

Lorentz transformations:
$$x = \gamma(x' + ut'), \quad t = \gamma(t' + \frac{ux'}{c^2})$$

If particle has velocity $v'$ in S':
$$v_x' = \frac{dx'}{dt'}, \quad x' = v_x't'$$

In frame S:
$$v_x = \frac{dx}{dt} = \frac{\gamma(dx' + udt')}{\gamma(dt' + \frac{u dx'}{c^2})}$$

$$= \frac{dx'/dt' + u}{1 + \frac{u}{c^2} \cdot \frac{dx'}{dt'}} = \boxed{\frac{v' + u}{1 + \frac{uv'}{c^2}}}$$

**Application:** If particle has $K.E. = 3mc^2$ (3 times rest energy):

Total energy: $E = K.E. + mc^2 = 3mc^2 + mc^2 = 4mc^2$

Also: $E = \gamma mc^2 = 4mc^2$

$\gamma = 4 \implies 1 - v^2/c^2 = 1/16$

$$v^2/c^2 = 15/16$$

$$\boxed{v = \frac{\sqrt{15}}{4}c \approx 0.968c}$$

---

## Important Formulas Summary

| Concept | Formula |
|---------|---------|
| Centripetal Acceleration | $a = \frac{v^2}{r} = \omega^2 r$ |
| Moment of Inertia | $I = \int r^2 dm$ |
| Torque | $\vec{\tau} = \vec{r} \times \vec{F} = I\alpha$ |
| Angular Momentum | $\vec{L} = \vec{r} \times \vec{p} = I\omega$ |
| Gravitational Force | $F = \frac{GMm}{r^2}$ |
| Orbital Velocity | $v = \sqrt{\frac{GM}{r}}$ |
| Rocket Equation | $V = u\ln(M_0/M)$ |
| Lorentz Factor | $\gamma = \frac{1}{\sqrt{1-v^2/c^2}}$ |
| Relativistic Energy | $E = \gamma mc^2$ |
| Velocity Addition | $v = \frac{u+v'}{1+uv'/c^2}$ |

---

**Total Marks: 90**
**Difficulty Level: Intermediate to Advanced**
**Time Required: 3 hours**

*Solutions assume standard values: $g = 10$ m/s², $c = 3 \times 10^8$ m/s*