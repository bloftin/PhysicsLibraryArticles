---
id: M02-02
title: Free-Body Diagrams
topic: Newtonian mechanics
level: Freshman through upper undergraduate
pacs: 45.20.Dd; 45.50.-j
gre_physics: true
status: draft
license: CC BY-SA 4.0
prerequisites:
  - M00-04 Scalars and vectors in mechanics
  - M01-03 Acceleration
  - M02-01 Newton's laws of motion
next:
  - M02-03 Common forces in mechanics
  - M02-04 Weight and normal force
  - M02-05 Tension and massless strings
  - M02-07 Friction
  - M02-08 Inclined-plane dynamics
  - M02-11 Dynamics of circular motion
---

# Free-Body Diagrams

A **free-body diagram** (FBD) is a simplified picture of one chosen body or system, isolated from its surroundings, with the **external forces** acting on that body shown as vectors.

The diagram is not merely an illustration. It is the bridge between a physical situation and Newton's equations of motion.

The basic chain is

\[
\boxed{
\text{physical situation}
\longrightarrow
\text{choose a system}
\longrightarrow
\text{free-body diagram}
\longrightarrow
\sum \mathbf F
\longrightarrow
\mathbf a
}
\]

For a particle or constant-mass body,

\[
\sum \mathbf F = m\mathbf a.
\]

A correct free-body diagram therefore answers the most important setup question in elementary dynamics:

> **What forces are actually acting on the object I chose to analyze?**

A large fraction of introductory mechanics errors occur before any algebra begins: the wrong system is chosen, a force is omitted, an internal force is included, a Newton's-third-law partner is placed on the wrong diagram, or a component of a force is mistaken for an additional force.

This article develops a systematic method for avoiding those errors.

---

## 1. Learning objectives

After completing this article, you should be able to:

1. choose an appropriate system boundary for a mechanics problem;
2. distinguish external forces from internal forces;
3. draw a particle or rigid-body free-body diagram;
4. identify weight, normal, tension, friction, spring, drag, and applied forces;
5. distinguish a physical force from a force component;
6. identify Newton's-third-law pairs without putting both members on one FBD;
7. choose coordinate axes that simplify the equations;
8. convert an FBD directly into component equations of motion;
9. decide when two bodies should be analyzed separately and when they should be treated as one system;
10. recognize the modifications required in a non-inertial frame;
11. solve common GRE-style force-diagram questions quickly.

---

# 2. What does “free” mean?

To **free** a body means to conceptually remove everything outside the chosen system and replace each relevant interaction with a force or moment acting on the isolated system.

Suppose a book rests on a table.

The physical picture contains:

- the book;
- the table;
- Earth;
- perhaps the room, air, and other nearby objects.

If the **book** is the system, the FBD contains only the book, together with the external forces exerted on it by things outside the system:

```text
               N_table→book
                    ↑
                    │
                [  BOOK  ]
                    │
                    ↓
                 W = mg
```

The table itself is not drawn as part of the isolated system. Its mechanical effect on the book is represented by the normal force.

Earth need not be drawn either. Its interaction with the book is represented by the gravitational force, which near Earth's surface is usually written

\[
\mathbf W = m\mathbf g.
\]

The same physical scene can produce a different FBD if a different system is chosen.

That fact is central:

\[
\boxed{\text{A free-body diagram is always relative to a chosen system.}}
\]

---

# 3. The system boundary is the first decision

Before identifying forces, decide exactly what object or collection of objects is being analyzed.

Possible systems include:

- one particle;
- one block;
- two connected blocks together;
- a person plus an elevator;
- a car;
- a wheel;
- Earth plus a satellite;
- an entire rigid body;
- part of a rigid body;
- a collection of interacting particles.

A useful mental step is to imagine drawing a closed boundary around the chosen system.

Interactions crossing that boundary are **external**.

Interactions entirely inside that boundary are **internal**.

## Example: two blocks in contact

Let blocks \(A\) and \(B\) rest on a frictionless horizontal surface while an external force \(F\) pushes block \(A\).

If the system is **block A alone**, the contact force from \(B\) must appear:

```text
                 F → [ A ] ← N_B→A
                         ↓ mg
                         ↑ N_floor
```

If the system is **A + B together**, the contact forces between A and B are internal and disappear from the system FBD:

```text
                 F → [   A + B   ]
                         ↓ (m_A+m_B)g
                         ↑ N_floor,total
```

Both FBDs are correct. They answer different questions.

The combined-system FBD is usually better for finding the common acceleration. The single-block FBD is required if the contact force between the blocks is desired.

---

# 4. External versus internal forces

For a chosen system,

\[
\sum \mathbf F_{\mathrm{external}}
= \frac{d\mathbf P}{dt},
\]

where \(\mathbf P\) is the total momentum of the system.

Internal forces may be extremely important physically, but their treatment depends on the system boundary.

For example, for two masses connected by a rope:

- tension is external to either mass individually;
- tension is internal to the combined two-mass-plus-rope system.

This is why choosing a larger system can simplify a problem.

## A useful rule

Ask of every candidate force:

> **What object exerts this force, and is that object outside my chosen system?**

If you cannot name the interacting object or field, the arrow deserves scrutiny.

---

# 5. A repeatable seven-step FBD procedure

The following procedure works for most introductory and intermediate mechanics problems.

## Step 1 — Choose the system

State it explicitly.

Examples:

- “system = the block”;
- “system = block A + block B”;
- “system = the car”;
- “system = the pendulum bob.”

Do not proceed until this is unambiguous.

## Step 2 — Isolate the system

Sketch only the chosen body or a simplified symbol for it.

For particle dynamics, a point or small box is usually sufficient.

For rigid-body statics or rotational dynamics, preserve enough shape and geometry to show:

- force application points;
- distances;
- lever arms;
- support locations;
- applied moments.

## Step 3 — List interactions with the surroundings

Inspect the system boundary.

Typical interactions are:

- gravity;
- contact with a surface;
- strings or cables;
- springs;
- fluid or aerodynamic drag;
- electric or magnetic forces;
- externally applied pushes or pulls.

## Step 4 — Replace each interaction by a force vector

Draw the force acting **on the chosen system**.

Do not draw the surrounding object merely because it exists in the physical scene.

## Step 5 — Label forces by source

Prefer labels such as

\[
\mathbf N_{\text{floor}\to\text{box}},
\qquad
\mathbf T_{\text{rope}\to\text{mass}},
\qquad
\mathbf F_{\text{Earth}\to\text{mass}}.
\]

Source-based notation makes Newton's-third-law reasoning far less ambiguous.

## Step 6 — Choose coordinates

Axes should simplify the force components and acceleration whenever possible.

On an incline, axes parallel and perpendicular to the surface are often superior to horizontal and vertical axes.

For circular motion, radial-tangential coordinates may be superior to Cartesian coordinates.

## Step 7 — Write Newton's equations from the diagram

Only after the FBD is complete should you write

\[
\sum F_x=ma_x,
\qquad
\sum F_y=ma_y,
\qquad
\sum F_z=ma_z.
\]

For rigid-body rotation, the force equations are supplemented by the appropriate moment equation, for example

\[
\sum \tau_z = I_z\alpha
\]

for fixed-axis rotation.

---

# 6. Common forces and how they appear on an FBD

## 6.1 Weight

Near Earth's surface,

\[
\mathbf W=m\mathbf g.
\]

The weight vector points approximately toward Earth's center.

In ordinary laboratory coordinates it is drawn vertically downward.

**Do not automatically draw \(mg\) perpendicular to an inclined surface.** Gravity is vertical; its *components* relative to incline-aligned axes are what lie parallel and perpendicular to the surface.

---

## 6.2 Normal force

A normal force is a contact force perpendicular to a surface.

```text
               N
               ↑
           [ block ]
  ───────────────────────── surface
```

The normal force is **not automatically equal to \(mg\)**.

It equals \(mg\) only in certain special cases, such as a block on a horizontal surface with no vertical acceleration and no additional vertical force components.

For a block on an incline,

\[
N=mg\cos\theta
\]

only under the usual special assumptions of no acceleration perpendicular to the incline and no other force components normal to the surface.

---

## 6.3 Tension

An ideal string or cable pulls along its own direction.

```text
 rope
────────────→ T
          [ mass ]
```

A string pulls; it does not push.

For an ideal massless string passing over an ideal massless, frictionless pulley, the tension magnitude is the same along one continuous string. Real ropes and pulleys may violate this idealization.

---

## 6.4 Friction

Friction acts tangentially to a contact surface and opposes **relative slipping or the tendency to slip**, not necessarily the instantaneous direction of the object's center-of-mass velocity.

Static friction satisfies

\[
|f_s|\le \mu_s N,
\]

while kinetic friction is often modeled as

\[
f_k=\mu_k N.
\]

One of the most common FBD mistakes is to assume automatically that

\[
f_s=\mu_sN.
\]

That equality applies only at impending slip.

---

## 6.5 Spring force

For an ideal one-dimensional spring,

\[
F_s=-kx,
\]

where \(x\) is displacement from equilibrium or the defined unstretched reference, depending on the setup.

The minus sign indicates that the force is restoring.

---

## 6.6 Drag

A drag force generally opposes motion relative to a fluid.

Common models include

\[
\mathbf F_d=-b\mathbf v
\]

for linear drag and

\[
\mathbf F_d=-c|\mathbf v|\mathbf v
\]

for quadratic drag.

The relevant velocity is velocity **relative to the surrounding fluid**, not necessarily relative to the ground.

---

## 6.7 Applied forces

A hand, motor, actuator, tow cable, propeller, thruster, or other agent may apply an external force.

Do not use a generic “applied force” arrow if a more physically descriptive label is available.

---

# 7. Forces are not the same thing as components

Suppose gravity acts on a block on an incline of angle \(\theta\).

The actual gravitational force is one vector:

\[
\mathbf W=m\mathbf g.
\]

If axes are chosen parallel and perpendicular to the incline, gravity can be decomposed into

\[
W_{\parallel}=mg\sin\theta,
\qquad
W_{\perp}=mg\cos\theta.
\]

Those are **components of one force**, not two additional physical forces.

A clean FBD usually shows the actual force vector \(mg\), with components introduced during the algebra or on a separate component sketch.

Bad conceptual accounting:

```text
Draw mg AND mg sinθ AND mg cosθ as three separate forces.
```

Correct accounting:

```text
One gravitational force mg;
resolve it into components when writing equations.
```

---

# 8. Newton's third law and the “wrong diagram” error

Newton's third law says that if object \(A\) exerts a force on object \(B\), then \(B\) exerts an equal and opposite force on \(A\):

\[
\mathbf F_{A\to B}=-\mathbf F_{B\to A}.
\]

The two forces act on **different bodies**.

Therefore they do not normally appear on the same single-body FBD.

## Book on table

For the **book**:

- Earth pulls downward on book;
- table pushes upward on book.

For the **table**:

- book pushes downward on table;
- floor or support pushes upward on table;
- Earth also pulls downward on the table itself.

The upward normal force on the book and the downward weight of the book are **not** a Newton's-third-law pair. They act on the same object.

The third-law partner of the normal force on the book is the force the book exerts on the table.

The third-law partner of Earth's gravitational force on the book is the gravitational force the book exerts on Earth.

This distinction is a frequent GRE conceptual test.

---

# 9. Do not draw “ma” as a force in an inertial frame

In an ordinary inertial-frame Newtonian FBD,

\[
\sum \mathbf F=m\mathbf a
\]

means that acceleration is the **result** of the net force.

You do not add an additional arrow labeled \(m\mathbf a\) to the FBD.

Incorrect:

```text
     N ↑
       [block] → F
     mg↓      ← ma
```

Correct:

```text
     N ↑
       [block] → F
     mg↓

then write:  ΣF_x = ma_x
```

An exception arises when deliberately formulating a problem in a non-inertial frame using inertial or fictitious forces. That is an advanced extension discussed later.

---

# 10. Choosing coordinate axes

Coordinate choice does not change the physics, but it can drastically simplify the algebra.

## Horizontal surface

Ordinary \(x\)-horizontal and \(y\)-vertical axes are usually convenient.

## Incline

Choose

\[
\hat{\mathbf x}\parallel \text{incline},
\qquad
\hat{\mathbf y}\perp \text{incline}.
\]

Then the normal force lies entirely along \(y\), while gravity becomes

\[
(mg)_x = mg\sin\theta,
\qquad
(mg)_y = mg\cos\theta.
\]

## Circular motion

Radial-tangential coordinates are often natural:

\[
a_r=-\frac{v^2}{r},
\qquad
a_t=\frac{dv}{dt}.
\]

The phrase **centripetal force** should not usually appear as a separate force on the FBD. “Centripetal” describes the inward **net radial force** required by the acceleration:

\[
\sum F_r=m\frac{v^2}{r}.
\]

The actual inward forces might be tension, gravity, normal force, friction, or a combination.

---

# 11. Particle FBD versus rigid-body FBD

In first-year particle dynamics, the object's spatial extent is often irrelevant, so all forces may be shown acting at a point or simplified box.

In rigid-body problems, force locations matter because different lines of action produce different torques.

## Particle model

```text
          T
          ↑
          • → F
          ↓
          mg
```

## Rigid-body model

```text
          ↑ R_B
A ●====================● B
  ↑ R_A             ↓ P
  <------  L  ------>
```

A rigid-body FBD should retain:

- support locations;
- force application points;
- distances;
- angles;
- applied couples or moments.

The translational equation

\[
\sum \mathbf F=m\mathbf a_G
\]

must then be combined with a rotational equation.

---

# 12. Ten essential FBD archetypes

These are schematic rather than to scale. The purpose is force identification.

## Archetype 1 — Block resting on a horizontal table

```text
               N
               ↑
           [ block ]
               ↓
               mg
```

If the block remains at rest vertically,

\[
N-mg=0.
\]

---

## Archetype 2 — Block pulled horizontally on a rough surface

```text
               N
               ↑
       f ← [ block ] → F
               ↓
               mg
```

Horizontal equation:

\[
F-f=ma.
\]

---

## Archetype 3 — Block pulled upward at an angle

```text
                    ↗ F
                  θ/
               N ↑
                 [block]
             f ←
                 ↓ mg
```

Vertical equilibrium, if applicable:

\[
N+F\sin\theta-mg=0,
\]

so the upward pull reduces the normal force and therefore may reduce friction.

---

## Archetype 4 — Block on an incline

```text
                   N ↗  perpendicular to plane
                  [■]
                 / ↓ mg
                /
_______________/ θ
```

With axes parallel/perpendicular to the plane:

\[
mg_{\parallel}=mg\sin\theta,
\qquad
mg_{\perp}=mg\cos\theta.
\]

---

## Archetype 5 — Hanging mass

```text
               T
               ↑
              [m]
               ↓
               mg
```

Taking upward positive,

\[
T-mg=ma.
\]

---

## Archetype 6 — Atwood machine: separate FBDs

```text
        mass 1                 mass 2
          T ↑                    ↑ T
           [m1]                [m2]
          mg1↓                    ↓mg2
```

For \(m_2>m_1\), with each positive axis chosen in its direction of acceleration,

\[
T-m_1g=m_1a,
\]

\[
m_2g-T=m_2a.
\]

---

## Archetype 7 — Elevator passenger

```text
               N
               ↑
            [person]
               ↓
               mg
```

The apparent weight is the normal force \(N\), not \(mg\).

If the elevator accelerates upward,

\[
N=m(g+a).
\]

---

## Archetype 8 — Car on a level curve

```text
Top view:

              inward
                ← f_s
                 [car]
```

Static friction can supply the inward radial force:

\[
f_s=m\frac{v^2}{r}.
\]

There is no additional physical force called “centripetal force.”

---

## Archetype 9 — Pendulum bob

```text
          pivot
            ●
           /  T points toward pivot
          /
         ● bob
         ↓ mg
```

Radial and tangential equations are usually more useful than horizontal and vertical equations.

---

## Archetype 10 — Two blocks treated as one system

```text
                F → [ A | B ]
                     ↑ N_total
                     ↓ (mA+mB)g
```

The A-B contact force is absent because it is internal to the chosen combined system.

---

# 13. Worked example 1 — Horizontal pull on a frictionless block

A \(4.0\,\mathrm{kg}\) block rests on a frictionless horizontal surface. A horizontal force of \(12\,\mathrm N\) pulls it to the right. Find its acceleration and normal force.

## Step 1: choose the system

System = block.

## Step 2: identify forces

- applied force \(F=12\,\mathrm N\) right;
- normal force \(N\) upward;
- weight \(mg\) downward.

```text
               N
               ↑
          [4 kg] → 12 N
               ↓
               mg
```

## Step 3: equations

Horizontal:

\[
\sum F_x=ma_x
\]

\[
12=(4.0)a_x,
\]

so

\[
\boxed{a_x=3.0\,\mathrm{m/s^2}}.
\]

Vertical acceleration is zero:

\[
N-mg=0,
\]

therefore

\[
N=(4.0)(9.81)=39.24\,\mathrm N.
\]

Thus

\[
\boxed{N\approx39.2\,\mathrm N}.
\]

### Lesson

The horizontal applied force does not change the normal force because it has no vertical component.

---

# 14. Worked example 2 — Pulling upward at an angle with friction

A \(10\,\mathrm{kg}\) crate is pulled by a \(50\,\mathrm N\) force directed \(30^\circ\) above horizontal. The coefficient of kinetic friction is \(\mu_k=0.20\). Find the acceleration.

## FBD

```text
                         ↗ 50 N
                       30°
                  N ↑
                    [crate]
                fk ←
                    ↓ mg
```

Take \(+x\) to the right and \(+y\) upward.

Vertical acceleration is zero:

\[
N+F\sin30^\circ-mg=0.
\]

Hence

\[
N=mg-F\sin30^\circ.
\]

With \(g=9.81\,\mathrm{m/s^2}\),

\[
N=(10)(9.81)-(50)(0.5)=73.1\,\mathrm N.
\]

The kinetic friction magnitude is

\[
f_k=\mu_kN=(0.20)(73.1)=14.62\,\mathrm N.
\]

Horizontal equation:

\[
F\cos30^\circ-f_k=ma.
\]

Therefore

\[
a=\frac{50\cos30^\circ-14.62}{10}
\approx2.87\,\mathrm{m/s^2}.
\]

\[
\boxed{a\approx2.87\,\mathrm{m/s^2}}.
\]

### Lesson

The pull changes the friction indirectly because its upward component reduces \(N\).

---

# 15. Worked example 3 — Frictionless incline

A block of mass \(m\) slides down a frictionless incline of angle \(\theta\). Determine its acceleration and normal force.

## FBD

The physical forces are only

- gravity \(mg\);
- normal force \(N\).

Choose \(+x\) down the incline and \(+y\) perpendicular outward from the surface.

Resolve gravity:

\[
(mg)_x=mg\sin\theta,
\qquad
(mg)_y=-mg\cos\theta.
\]

Parallel to incline:

\[
mg\sin\theta=ma,
\]

thus

\[
\boxed{a=g\sin\theta}.
\]

Perpendicular to incline:

\[
N-mg\cos\theta=0,
\]

thus

\[
\boxed{N=mg\cos\theta}.
\]

### Lesson

There is no force “\(mg\sin\theta\)” in addition to gravity. It is the component of gravity parallel to the selected axis.

---

# 16. Worked example 4 — Two blocks in contact

Blocks \(A\) and \(B\), with masses

\[
m_A=2.0\,\mathrm{kg},
\qquad
m_B=3.0\,\mathrm{kg},
\]

sit on a frictionless horizontal surface. A force \(F=20\,\mathrm N\) pushes \(A\) to the right. Find the acceleration and the contact force between the blocks.

## First FBD: choose A+B as the system

The contact force is internal and does not appear.

\[
F=(m_A+m_B)a.
\]

Therefore

\[
a=\frac{20}{2+3}=4.0\,\mathrm{m/s^2}.
\]

\[
\boxed{a=4.0\,\mathrm{m/s^2}}.
\]

## Second FBD: choose B alone

The only horizontal force on \(B\) is the contact force exerted by \(A\):

\[
F_{A\to B}=m_Ba.
\]

Thus

\[
F_{A\to B}=(3.0)(4.0)=12\,\mathrm N.
\]

\[
\boxed{F_{A\to B}=12\,\mathrm N}.
\]

By Newton's third law,

\[
\mathbf F_{B\to A}=-\mathbf F_{A\to B}.
\]

### Lesson

Use a large system to eliminate internal forces; use a smaller system when an internal interaction itself is the unknown.

---

# 17. Worked example 5 — Atwood machine

Two masses \(m_1=2.0\,\mathrm{kg}\) and \(m_2=5.0\,\mathrm{kg}\) are connected by an ideal massless string over an ideal pulley. Find the acceleration and tension.

Because \(m_2>m_1\), let \(m_2\) accelerate downward and \(m_1\) upward with common magnitude \(a\).

For \(m_1\):

\[
T-m_1g=m_1a.
\]

For \(m_2\):

\[
m_2g-T=m_2a.
\]

Adding eliminates the internal string tension:

\[
(m_2-m_1)g=(m_1+m_2)a.
\]

Therefore

\[
a=\frac{m_2-m_1}{m_1+m_2}g
=\frac{3}{7}(9.81)
\approx4.20\,\mathrm{m/s^2}.
\]

\[
\boxed{a\approx4.20\,\mathrm{m/s^2}}.
\]

Now use either mass, for example \(m_1\):

\[
T=m_1(g+a)
=2.0(9.81+4.20)
\approx28.0\,\mathrm N.
\]

\[
\boxed{T\approx28.0\,\mathrm N}.
\]

### Lesson

The two weights are not placed on one single-mass FBD. Each mass gets its own weight and tension. The algebra then reflects the string constraint.

---

# 18. Worked example 6 — Elevator apparent weight

A \(70\,\mathrm{kg}\) person stands on a scale in an elevator accelerating downward at \(2.0\,\mathrm{m/s^2}\). What does the scale read?

The scale measures the normal force \(N\), not the gravitational force \(mg\).

Take upward as positive.

```text
               N
               ↑
            [person]
               ↓
               mg

          acceleration ↓
```

Then

\[
N-mg=m(-2.0).
\]

Thus

\[
N=m(g-2.0)
=70(9.81-2.0)
\approx547\,\mathrm N.
\]

\[
\boxed{N\approx5.47\times10^2\,\mathrm N}.
\]

The person feels lighter even though

\[
mg\approx687\,\mathrm N
\]

has not changed significantly.

### Lesson

“Apparent weight” is a contact force inferred by the scale. It need not equal gravitational weight.

---

# 19. Common mistakes

## Mistake 1 — Drawing forces exerted by the chosen body

An FBD shows forces **on** the chosen body, not forces it exerts on other objects.

## Mistake 2 — Drawing both members of a third-law pair on one body

Third-law partners act on different bodies.

## Mistake 3 — Automatically setting \(N=mg\)

Normal force depends on geometry and acceleration.

## Mistake 4 — Automatically setting \(f_s=\mu_sN\)

Static friction adjusts as needed up to its maximum.

## Mistake 5 — Adding “centripetal force” as an extra force

Centripetal force is the inward net force, not a new interaction.

## Mistake 6 — Adding \(ma\) as an ordinary force

In an inertial frame, \(m\mathbf a\) is the result of \(\sum\mathbf F\), not an additional physical interaction.

## Mistake 7 — Drawing force components as additional forces

\(mg\sin\theta\) and \(mg\cos\theta\) are components of \(mg\).

## Mistake 8 — Assuming friction always points opposite velocity

Friction opposes slipping or impending relative slipping at the contact.

## Mistake 9 — Forgetting the system boundary

Whether a force is internal or external changes when the chosen system changes.

## Mistake 10 — Choosing inconvenient axes

A correct but poor coordinate choice can turn a simple problem into unnecessary algebra.

---

# 20. A fast GRE FBD method

GRE mechanics questions often reward correct setup more than lengthy calculation.

A useful fast procedure is:

1. **Circle the body or system.**
2. **Name every external interaction.**
3. **Choose axes to match geometry or acceleration.**
4. **Ask which acceleration components are known to be zero.**
5. **Write only the Newton equation needed for the requested quantity.**

For example, if a crate is pulled upward at an angle and the question asks only how friction changes, you may not need to solve the entire dynamics problem. The vertical FBD immediately shows

\[
N=mg-F\sin\theta,
\]

so both kinetic friction \(\mu_kN\) and the maximum possible static friction \(\mu_sN\) decrease as the upward pull increases.

---

# 21. System choice as a problem-solving tool

The FBD is not only a bookkeeping device. The **choice of system can eliminate unknown forces**.

## Example pattern: connected particles

Suppose two blocks are tied together and pulled horizontally.

If the desired quantity is acceleration, choose both blocks as one system. Tension becomes internal and disappears.

If the desired quantity is tension, isolate one block after the acceleration is known.

This suggests a general strategy:

\[
\boxed{
\text{Choose the largest useful system first; isolate smaller parts only when needed.}
}
\]

The same strategy becomes important later in:

- center-of-mass mechanics;
- collisions;
- rigid-body mechanics;
- fluid control volumes;
- continuum mechanics.

---

# 22. FBDs in non-inertial frames

The simple equation

\[
\sum \mathbf F_{\text{physical}}=m\mathbf a
\]

has its ordinary form in an inertial frame.

If the coordinate frame itself accelerates, one may either:

1. describe the motion from an inertial frame; or
2. remain in the accelerating frame and introduce appropriate inertial or fictitious forces.

For a frame translating with acceleration \(\mathbf A\), one may write

\[
\sum \mathbf F_{\text{physical}}
+\mathbf F_{\text{inertial}}
=m\mathbf a_{\text{relative}},
\]

with

\[
\mathbf F_{\text{inertial}}=-m\mathbf A.
\]

Rotating frames introduce centrifugal, Coriolis, and Euler terms.

These are not additional physical interactions like tension or gravity. They are terms introduced so that Newton-like equations can be used in a non-inertial coordinate description.

See the later M10 non-inertial dynamics sequence.

---

# 23. FBDs and the transition to analytical mechanics

Free-body diagrams are strongly associated with Newtonian mechanics, but the underlying idea survives in more advanced formulations.

Newtonian mechanics starts from forces:

\[
\sum_i \mathbf F_i=m\mathbf a.
\]

Lagrangian mechanics often replaces explicit force-component bookkeeping with generalized coordinates and energetic quantities:

\[
L=T-U.
\]

For constrained systems this can be dramatically simpler because ideal constraint forces may disappear from the equations automatically.

This does **not** make the FBD obsolete.

A strong analytical-mechanics student should still be able to answer:

- what interactions exist physically?
- which forces are external?
- what is the system boundary?
- which forces are constraints?
- which forces perform virtual work?

The FBD therefore remains a useful conceptual check even when the final derivation uses Lagrange's equations.

---

# 24. Practice exercises

Unless otherwise stated, neglect air resistance and use \(g=9.81\,\mathrm{m/s^2}\).

## MECH-NEWTON-001 — Book on a table

A \(2.5\,\mathrm{kg}\) book rests on a horizontal table.

1. Draw the FBD of the book.
2. Find the normal force.
3. Identify the third-law partner of the normal force acting on the book.

**Answer:** \(N=24.5\,\mathrm N\). The third-law partner is the downward contact force exerted by the book on the table.

---

## MECH-NEWTON-002 — Horizontal acceleration

A \(6.0\,\mathrm{kg}\) block on a frictionless floor experiences a horizontal force of \(18\,\mathrm N\).

1. Draw its FBD.
2. Find its acceleration.

**Answer:** \(a=3.0\,\mathrm{m/s^2}\).

---

## MECH-NEWTON-003 — Upward angled pull

A \(20\,\mathrm{kg}\) crate is pulled by a \(100\,\mathrm N\) force at \(40^\circ\) above horizontal. It has no vertical acceleration.

1. Draw the FBD.
2. Find the normal force.

**Answer:**

\[
N=mg-F\sin40^\circ\approx132\,\mathrm N.
\]

---

## MECH-NEWTON-004 — Downward angled push

Repeat MECH-NEWTON-003 if the \(100\,\mathrm N\) force is directed \(40^\circ\) **below** horizontal.

**Answer:**

\[
N=mg+F\sin40^\circ\approx260\,\mathrm N.
\]

---

## MECH-NEWTON-005 — Static friction test

A horizontal force of \(30\,\mathrm N\) acts on a stationary \(10\,\mathrm{kg}\) block. The coefficient of static friction is \(\mu_s=0.50\).

1. Draw the FBD.
2. Determine the actual static friction force.
3. Does the block move?

**Answer:** The maximum static friction is \(49.1\,\mathrm N\), so the actual static friction is \(30\,\mathrm N\) opposite the applied force. The block remains at rest.

---

## MECH-NEWTON-006 — Incline without friction

A \(5.0\,\mathrm{kg}\) block is on a frictionless \(25^\circ\) incline.

1. Draw an FBD using incline-aligned axes.
2. Find the normal force.
3. Find the acceleration down the plane.

**Answer:**

\[
N=mg\cos25^\circ\approx44.5\,\mathrm N,
\]

\[
a=g\sin25^\circ\approx4.15\,\mathrm{m/s^2}.
\]

---

## MECH-NEWTON-007 — Hanging mass accelerating upward

A \(3.0\,\mathrm{kg}\) mass hangs from a cable and accelerates upward at \(1.5\,\mathrm{m/s^2}\).

1. Draw the FBD.
2. Find the cable tension.

**Answer:**

\[
T=m(g+a)\approx33.9\,\mathrm N.
\]

---

## MECH-NEWTON-008 — Hanging mass accelerating downward

The same \(3.0\,\mathrm{kg}\) mass accelerates downward at \(1.5\,\mathrm{m/s^2}\).

**Answer:**

\[
T=m(g-a)\approx24.9\,\mathrm N.
\]

---

## MECH-NEWTON-009 — Two blocks, combined system

Blocks of \(4\,\mathrm{kg}\) and \(6\,\mathrm{kg}\) are in contact on a frictionless floor. A \(50\,\mathrm N\) force pushes the \(4\,\mathrm{kg}\) block toward the \(6\,\mathrm{kg}\) block.

1. Draw the FBD of both blocks as one system.
2. Find their acceleration.
3. Draw the FBD of the \(6\,\mathrm{kg}\) block alone.
4. Find the contact force.

**Answer:** \(a=5.0\,\mathrm{m/s^2}\), contact force \(=30\,\mathrm N\).

---

## MECH-NEWTON-010 — Elevator scale

A \(60\,\mathrm{kg}\) passenger stands on a scale in an elevator accelerating upward at \(1.2\,\mathrm{m/s^2}\).

**Answer:**

\[
N=m(g+a)\approx661\,\mathrm N.
\]

---

## MECH-NEWTON-011 — Level circular turn

A \(1000\,\mathrm{kg}\) car travels at \(15\,\mathrm{m/s}\) around a level circular curve of radius \(50\,\mathrm m\).

1. Draw a top-view FBD showing the horizontal force.
2. Determine the required static-friction magnitude.

**Answer:**

\[
f_s=m\frac{v^2}{r}=4500\,\mathrm N.
\]

---

## MECH-NEWTON-012 — Conical pendulum setup

A mass moves in a horizontal circle while suspended by a string making angle \(\theta\) with the vertical.

1. Draw the FBD.
2. Write the vertical and radial equations without solving them.

**Answer:**

\[
T\cos\theta=mg,
\qquad
T\sin\theta=m\frac{v^2}{r}.
\]

---

## MECH-NEWTON-013 — System boundary choice

Two identical blocks are connected by a massless string and pulled across a frictionless surface by a force \(F\).

Explain which FBD you would use first to determine:

1. the acceleration;
2. the tension.

**Answer:** Use both blocks as one system to obtain the acceleration, eliminating internal tension. Then isolate either block to solve for the tension.

---

## MECH-NEWTON-014 — Find the conceptual error

A student draws a block sliding down a frictionless incline with arrows labeled

- \(mg\) downward;
- \(mg\sin\theta\) down the incline;
- \(mg\cos\theta\) into the incline;
- \(N\) out of the incline.

What is wrong?

**Answer:** The student has counted gravity three times. \(mg\sin\theta\) and \(mg\cos\theta\) are components of the single gravitational force \(mg\), not additional forces.

---

# 25. GRE-speed questions

These are original PhysicsLibrary questions written to practice the style and speed of mechanics reasoning. They are **not ETS questions**.

## GRE-FBD-001

A block rests on a horizontal floor. A force \(F\) is applied at an angle above horizontal, but the block remains in contact with the floor. As \(F\) increases while its angle remains fixed, the normal force on the block

A. increases  
B. decreases  
C. remains equal to \(mg\)  
D. becomes \(mg+F\)  
E. is independent of the vertical component of \(F\)

**Answer: B.** The upward component of \(F\) reduces the normal force.

---

## GRE-FBD-002

A book rests on a table. Which force is the Newton's-third-law partner of the upward normal force exerted by the table on the book?

A. the gravitational force on the book  
B. the gravitational force of the book on Earth  
C. the downward contact force exerted by the book on the table  
D. the upward force of the floor on the table  
E. the weight of the table

**Answer: C.** Third-law partners are the same interaction acting on opposite bodies.

---

## GRE-FBD-003

A car moves at constant speed around a level circular track. Which statement is correct?

A. The net force is zero because speed is constant.  
B. A new force called centripetal force must be added to the FBD.  
C. Static friction may provide the inward net force.  
D. Friction must point opposite the car's instantaneous velocity.  
E. Gravity supplies the horizontal centripetal force.

**Answer: C.** Constant speed does not imply constant velocity; the inward acceleration requires a radial net force.

---

## GRE-FBD-004

A mass hangs at rest from a single ideal vertical string. Which pair of forces belongs on the mass's FBD?

A. tension upward and the mass's pull on the string downward  
B. tension upward and weight downward  
C. two equal tensions in opposite directions  
D. weight downward and Earth's reaction force upward  
E. weight downward only

**Answer: B.** Both forces act on the mass.

---

## GRE-FBD-005

A block is at rest on a rough incline. The static friction force

A. must equal \(\mu_sN\)  
B. must point down the incline  
C. must point up the incline  
D. adjusts to whatever value is required for equilibrium, up to \(\mu_sN\)  
E. is zero because the block is not moving

**Answer: D.** Its direction and magnitude follow from the tendency to slip and the equilibrium requirement.

---

## GRE-FBD-006

Two blocks are in contact on a frictionless floor and accelerate together under one external horizontal force. If the two blocks are selected as a single system, the contact force between them

A. doubles  
B. is an external force  
C. is an internal force and is omitted from the system FBD  
D. must be equal to the applied force  
E. becomes a fictitious force

**Answer: C.** The interaction does not cross the chosen system boundary.

---

## GRE-FBD-007

An elevator is accelerating downward, but its speed is momentarily upward. For a passenger inside, which inequality is correct?

A. \(N>mg\)  
B. \(N=mg\)  
C. \(N<mg\)  
D. \(N=0\) necessarily  
E. the answer depends on whether velocity is upward

**Answer: C.** The acceleration, not the instantaneous velocity direction, determines the force imbalance.

---

## GRE-FBD-008

A block slides down a frictionless incline. Which is the most appropriate statement about \(mg\sin\theta\)?

A. It is a new interaction force created by the incline.  
B. It is the normal force.  
C. It is the component of the gravitational force parallel to the incline.  
D. It is the centripetal force.  
E. It is a Newton's-third-law reaction force.

**Answer: C.** It is a coordinate component of the single gravitational force \(mg\).

---

# 26. Summary

A free-body diagram is a disciplined representation of the **external interactions acting on a chosen system**.

The essential procedure is

\[
\boxed{
\begin{array}{c}
\text{choose the system}\\
\downarrow\\
\text{isolate it}\\
\downarrow\\
\text{identify external interactions}\\
\downarrow\\
\text{draw and label force vectors}\\
\downarrow\\
\text{choose coordinates}\\
\downarrow\\
\sum \mathbf F=m\mathbf a
\end{array}
}
\]

The most important conceptual rules are:

- draw forces acting **on** the chosen system;
- distinguish external from internal forces;
- do not put both members of a Newton's-third-law pair on one single-body FBD;
- do not confuse a force with its components;
- do not assume \(N=mg\);
- do not assume \(f_s=\mu_sN\);
- do not add “centripetal force” as an extra interaction;
- do not draw \(m\mathbf a\) as a physical force in an inertial frame;
- choose axes that exploit the geometry;
- change the system boundary strategically when it eliminates unknown internal forces.

Once an FBD is correct, the equations of motion are often straightforward. If the FBD is wrong, even perfect algebra solves the wrong physical problem.

---

# 27. Source and licensing note

This PhysicsLibrary article is an expanded instructional synthesis. Its core free-body-diagram workflow was adapted conceptually from the openly licensed **Mechanics Map** treatment and then extended with PhysicsLibrary-original material covering system boundaries, Newton's-third-law diagnostics, coordinate strategy, particle versus rigid-body diagrams, non-inertial-frame cautions, worked examples, practice exercises, and GRE-speed questions.

## Primary open source

**Jacob Moore & Contributors, Mechanics Map, “Free Body Diagrams,” Engineering LibreTexts.**  
License: **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0).**  
https://eng.libretexts.org/Bookshelves/Mechanical_Engineering/Mechanics_Map_%28Moore_et_al.%29/01%3A_Basics_of_Newtonian_Mechanics/1.04%3A_Free_Body_Diagrams

Mechanics Map's general construction sequence—isolating the selected body, replacing surrounding interactions with external forces/moments, and labeling relevant geometry—is the principal openly licensed scaffold used here. The prose, examples, diagrams, GRE questions, organization, and extensions in this PhysicsLibrary article are newly written or substantially reworked.

## Additional curriculum cross-check

**Tom Weideman, UCD Physics 9A – Classical Mechanics, Physics LibreTexts.**  
License: **CC BY-SA 4.0.**  
https://phys.libretexts.org/Courses/University_of_California_Davis/UCD%3A_Classical_Mechanics

Used as a curriculum-level cross-check for the introductory Newtonian mechanics sequence rather than as a source of copied prose or figures.

No external figures or media are copied into this article. The schematic diagrams above are original text diagrams. The numerical worked examples, practice exercises, and GRE-speed questions are original PhysicsLibrary material.

## License

Unless otherwise noted, this PhysicsLibrary article is intended for release under the **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** license.
