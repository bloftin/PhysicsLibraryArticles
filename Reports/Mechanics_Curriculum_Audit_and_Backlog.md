# PhysicsLibrary Mechanics Curriculum Audit and Backlog

**Repository:** PhysicsLibraryArticles  
**Report date:** 2026-08-18  
**Scope:** freshman calculus-based mechanics through graduate classical mechanics at approximately the Goldstein level, with explicit GRE Physics Subject Test coverage.

## 1. Goal

Turn the existing PhysicsLibrary mechanics entries into a coherent learning system rather than a collection of isolated encyclopedia pages. The finished mechanics area should support four overlapping uses:

1. a first-year calculus-based university mechanics course;
2. GRE Physics Subject Test preparation;
3. upper-undergraduate analytical mechanics;
4. graduate classical mechanics through the main Goldstein-level topics.

PACS should remain the classification system, but PACS should not be the student-facing table of contents. A separate **Mechanics Learning Path** should order the material pedagogically.

## 2. Current PhysicsLibrary audit summary

The existing mechanics corpus is substantial but uneven.

### Strong or useful existing clusters

- Basic objects: position, velocity, acceleration, mass, momentum, kinetic energy, work, power, friction, equilibrium.
- Newtonian examples: constant acceleration, projectile motion, inclined planes, circular motion, gravitation, conservation of momentum.
- Systems of particles: center of mass, center-of-mass motion, angular momentum, total energy.
- Celestial mechanics: Newtonian gravitation, Kepler laws, orbital-period examples, central-force seed material.
- Analytical mechanics seed: generalized coordinates, coordinate examples, Hamilton's principle, Lagrange's equations, variational principle.
- Rigid-body/GNC representation material: DCMs, Euler-angle sequences, axis-angle, quaternions, Euler-angle velocity relations, inertia tensor, Euler moment equations.
- Fluids seed: Archimedes' principle, continuity equation, Lagrangian derivative, Reynolds transport theorem.

### Major gaps

- free-body diagrams and systematic force modeling;
- work-energy theorem and a coherent potential-energy sequence;
- impulse and collision problem solving;
- elementary rotational mechanics beneath the existing advanced attitude-representation material;
- complete oscillations sequence;
- elementary fluids required by the GRE;
- non-inertial reference frames required by the GRE;
- complete central-force/scattering treatment;
- small oscillations and normal modes;
- Hamiltonian mechanics itself;
- Poisson brackets, canonical transformations, Hamilton-Jacobi theory, action-angle variables, perturbation theory, and nonlinear dynamics.

### Immediate correctness/classification issues

- `simple harmonic oscillator` needs a correctness review before expansion. The current initial-condition form should use the coefficient `v_0/omega` multiplying `sin(omega t)` when `v_0` denotes initial velocity.
- `resonance` should be cross-classified into classical mechanics/oscillations.
- `anharmonic` should be moved/cross-classified from abstract harmonic analysis into nonlinear/anharmonic mechanics.
- Several celestial-mechanics PACS listings contain unrelated elementary mechanics examples and should be cleaned up.
- Existing attitude-conversion articles should be retained, but moved later in the student-facing rigid-body path so elementary torque, angular momentum, inertia, and rigid-body dynamics come first.

## 3. GRE coverage target

ETS currently assigns **20%** of the GRE Physics Subject Test to Classical Mechanics. The mechanics learning path should explicitly cover:

- kinematics;
- Newton's laws;
- work and energy;
- oscillatory motion;
- rotational motion about a fixed axis;
- dynamics of systems of particles;
- central forces and celestial mechanics;
- three-dimensional particle dynamics;
- Lagrangian and Hamiltonian formalism;
- non-inertial reference frames;
- elementary fluid dynamics.

Source: https://www.ets.org/gre/test-takers/subject-tests/about/content-structure.html

## 4. Licensing and OER source policy

PhysicsLibrary content is intended to remain compatible with its CC BY-SA 4.0 contribution model. Use the following source policy for mechanics work.

| Key | Source | License/use recommendation |
|---|---|---|
| `PL` | Existing PhysicsLibrary material | Reuse/repair existing material and preserve provenance. |
| `UCD9A` | UCD Physics 9A Classical Mechanics | CC BY-SA 4.0. Excellent freshman mechanics source. https://phys.libretexts.org/Courses/University_of_California_Davis/UCD%3A_Classical_Mechanics |
| `MM` | Mechanics Map, Moore et al. | CC BY-SA 4.0. Excellent for FBDs, statics, particle/rigid-body dynamics, worked examples and homework. https://eng.libretexts.org/Bookshelves/Mechanical_Engineering/Mechanics_Map_%28Moore_et_al.%29 |
| `OS16` | Archived 2016 University Physics Vol. 1 clone | CC BY 4.0. Use the archived licensed revision, not text copied from the current OpenStax live edition. https://pressbooks.bccampus.ca/universityphysicssandboxbook1/ |
| `WB` | Wikibooks Classical Mechanics | CC BY-SA. Useful for analytical mechanics, constraints, non-inertial frames and Hamiltonian topics. https://en.wikibooks.org/wiki/Classical_Mechanics |
| `WIKI` | Wikipedia/Wikimedia | Wikipedia text is CC BY-SA; check each image/media file separately. |
| `CROWELL` | Benjamin Crowell, Mechanics / Light and Matter | CC BY-SA. https://www.lightandmatter.com/mechanics/ |
| `SCHNICK` | Jeffrey W. Schnick, Calculus-Based Physics I | CC BY-SA 3.0 except where otherwise noted. https://collection.bccampus.ca/textbook/AfcGnrKw/ |
| `PD` | Verified public-domain historical material | Good for historical derivations, diagrams and source excerpts after work-level verification. |
| `ORIGINAL` | New PhysicsLibrary derivation/problem set | Preferred when no clean BY/BY-SA source exists or a consistent notation is important. |
| `REF` | Goldstein, Taylor, Landau, MIT OCW, other restricted/NC references | Use to benchmark scope and correctness only; do not transplant restricted prose/figures. |

**OpenStax warning:** the current live OpenStax *University Physics* edition is CC BY-NC-SA 4.0. The archived 2016 BCcampus clone explicitly records CC BY 4.0. Creative Commons licenses are irrevocable for copies already released under them, but provenance must identify the exact archived revision and figure-level exceptions must still be checked.

## 5. Backlog conventions

### Priority

- **P0** — correctness, classification, or structural prerequisite; do first.
- **P1** — freshman/GRE core. Completing P0+P1 should produce full GRE mechanics topic coverage.
- **P2** — upper-undergraduate analytical mechanics and deeper mechanics.
- **P3** — graduate/Goldstein-level completion.

### Exercise shorthand

- `W` = fully worked examples.
- `P` = practice/derivation/computational problems.
- `G` = GRE-speed multiple-choice problems.

A core P1 article should normally end with roughly `3-5W / 8-12P / 4-8G`. Advanced articles can replace GRE problems with derivation/computational problems.

### Current-URL note

Where an exact article permalink was not independently verified, the backlog points to the confirmed PhysicsLibrary PACS listing rather than guessing a permalink. New articles use `—`.

---

# 6. Mechanics article backlog

## M00 — Learning path and foundations

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M00-01 | Mechanics learning path | New hub | All | Yes | — | None | Roadmap, prerequisite graph, diagnostic, section links | ORIGINAL/WIKI | P0 |
| M00-02 | Classical mechanics | Upgrade | All | Yes | https://physicslibrary.org/browse/objects/45./ | Vectors, calculus | Scope, domains, limitations, history; 2W/6P/3G | PL/WIKI | P1 |
| M00-03 | Units and dimensional analysis | New | Freshman | High | — | Algebra | Dimensions, scaling, Buckingham-style intuition; 3W/10P/6G | OS16/UCD9A/SCHNICK | P1 |
| M00-04 | Scalars and vectors in mechanics | New | Freshman | High | — | Algebra/trig | Components, dot/cross products; 4W/12P/6G | UCD9A/SCHNICK | P1 |
| M00-05 | Coordinate systems for mechanics | New | Freshman-Graduate | High | — | Vectors | Cartesian/cylindrical/spherical overview; 4W/10P/4G | OS16/UCD9A/WB | P1 |
| M00-06 | Reference frames in Newtonian mechanics | Upgrade | Freshman-Upper UG | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Vectors, kinematics | Galilean frames and transformations; 3W/8P/5G | PL/UCD9A/WIKI | P1 |
| M00-07 | Degrees of freedom | New | Freshman-Graduate | Medium | — | Coordinates | Particle/system/rigid-body examples; 3W/8P | WB/WIKI | P2 |

## M01 — Kinematics

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M01-01 | Position and displacement | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.05.%2Bx/ | Vectors | 1D/2D/3D definitions and graphs; 3W/10P/5G | PL/UCD9A/OS16 | P1 |
| M01-02 | Velocity | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.05.%2Bx/ | Position, derivative | Average/instantaneous/vector velocity; 3W/10P/5G | PL/UCD9A/OS16 | P1 |
| M01-03 | Acceleration | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.05.%2Bx/ | Velocity, derivative | Average/instantaneous/vector acceleration; 3W/10P/5G | PL/UCD9A/OS16 | P1 |
| M01-04 | Motion graphs | New | Freshman | High | — | Position/velocity/acceleration | x-t, v-t, a-t interpretation; 4W/12P/8G | UCD9A/OS16 | P1 |
| M01-05 | Constant-acceleration motion | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.Dd/ | 1D kinematics | Derive equations, vertical motion; 4W/12P/8G | PL/UCD9A/OS16 | P1 |
| M01-06 | Variable-acceleration motion | New | Freshman-Upper UG | Medium | — | Calculus, kinematics | Integration and position-dependent acceleration; 4W/10P/4G | UCD9A/SCHNICK | P1 |
| M01-07 | Projectile motion | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45./ | 2D vectors | Equal/unequal-height launches; 4W/12P/8G | PL/UCD9A/OS16 | P1 |
| M01-08 | Uniform circular motion | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Vectors | Centripetal acceleration derivation; 4W/10P/6G | PL/UCD9A/OS16 | P1 |
| M01-09 | Relative motion | New | Freshman-Upper UG | High | — | Vectors, velocity | 1D/2D Galilean velocity addition; 4W/10P/6G | UCD9A/OS16 | P1 |
| M01-10 | Polar-coordinate particle kinematics | New | Upper UG | Medium | — | Calculus, vectors | Unit-vector derivatives, velocity/acceleration; 3W/8P/2G | WB/MM/WIKI | P2 |
| M01-11 | Cylindrical and spherical particle kinematics | New | Upper UG | Medium | — | Vector calculus | Full velocity/acceleration formulas; 3W/8P/2G | WB/WIKI | P2 |

## M02 — Newtonian dynamics

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M02-01 | Newton's laws of motion | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Kinematics | Three laws, inertial frames, applications; 4W/12P/8G | PL/UCD9A/OS16 | P1 |
| M02-02 | Free-body diagrams | New | Freshman | High | — | Newton's laws, vectors | Conventions + at least 10 archetypes; 6W/14P/8G | MM/UCD9A | P1 |
| M02-03 | Common forces in mechanics | New hub | Freshman | High | — | Newton's laws | Weight/normal/tension/spring/friction/drag map; 3W/8P/5G | MM/OS16 | P1 |
| M02-04 | Weight and normal force | New/merge | Freshman | High | https://physicslibrary.org/browse/objects/45.50.Dd/ | FBDs | Elevators, curved paths, apparent weight; 4W/10P/6G | PL/MM/UCD9A | P1 |
| M02-05 | Tension and massless strings | New | Freshman | High | — | FBDs | Connected-particle examples; 4W/10P/6G | MM/UCD9A | P1 |
| M02-06 | Pulleys and Atwood machines | New | Freshman | High | — | Tension, constraints | Ideal and compound systems; 4W/12P/6G | MM/UCD9A | P1 |
| M02-07 | Friction | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.05.%2Bx/ | FBDs | Static/kinetic/impending motion; 4W/12P/7G | PL/MM/UCD9A | P1 |
| M02-08 | Inclined-plane dynamics | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | FBDs, friction | Frictionless/friction/pulley variants; 4W/10P/6G | PL/MM | P1 |
| M02-09 | Spring force and Hooke's law | New | Freshman | High | — | Newton's laws | Force law and energy bridge; 4W/10P/5G | OS16/UCD9A/CROWELL | P1 |
| M02-10 | Drag forces and terminal velocity | New | Freshman-Upper UG | Medium | — | ODEs, Newton's laws | Linear/quadratic drag, terminal speed; 4W/10P/4G | CROWELL/WIKI | P1 |
| M02-11 | Dynamics of circular motion | New | Freshman | High | — | Circular kinematics, FBDs | Banked turns, loops, conical pendulum; 5W/12P/7G | UCD9A/OS16 | P1 |

## M03 — Work, energy, and potentials

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M03-01 | Work | Upgrade | Freshman | High | https://physicslibrary.org/encyclopedia/Work.html | Vectors, force | Constant/variable force; 4W/10P/6G | PL/UCD9A/OS16 | P1 |
| M03-02 | Kinetic energy | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.05.%2Bx/ | Velocity | Particle/system distinction; 3W/8P/5G | PL/UCD9A | P1 |
| M03-03 | Work-energy theorem | New | Freshman | High | — | Work, Newton's laws | Derivation and applications; 5W/12P/8G | UCD9A/OS16 | P1 |
| M03-04 | Power | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45./ | Work, velocity | Average/instantaneous, P=F dot v; 3W/8P/5G | PL/UCD9A/OS16 | P1 |
| M03-05 | Conservative forces | New | Freshman-Upper UG | High | — | Work, calculus | Path independence and closed loops; 3W/8P/4G | UCD9A/WIKI | P1 |
| M03-06 | Potential energy | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Work | Gravity, spring and general potentials; 4W/10P/6G | PL/UCD9A/OS16 | P1 |
| M03-07 | Force from potential energy | Upgrade | Freshman-Upper UG | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Potential, derivative | F=-dU/dx and -grad U; 4W/10P/5G | PL/UCD9A/WIKI | P1 |
| M03-08 | Mechanical-energy conservation | New hub | Freshman | High | — | Kinetic/potential energy | Conservative/nonconservative accounting; 5W/12P/8G | UCD9A/OS16 | P1 |
| M03-09 | Potential-energy diagrams and equilibrium | New | Freshman-Upper UG | High | — | Potential energy, derivatives | Turning points and stability; 4W/10P/6G | UCD9A/WIKI | P1 |
| M03-10 | Virial theorem | Upgrade | Graduate | Low | https://physicslibrary.org/browse/objects/45.40.-f/ | Time averages, potentials | Classical derivation and power-law forces; 2W/6P | PL/WIKI/ORIGINAL | P3 |

## M04 — Momentum, collisions, and particle systems

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M04-01 | Linear momentum | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.05.%2Bx/ | Newton's laws | Momentum form of Newton II; 3W/10P/6G | PL/UCD9A/OS16 | P1 |
| M04-02 | Impulse and impulse-momentum theorem | New | Freshman | High | — | Momentum, integration | Force-time graphs and theorem; 4W/10P/6G | UCD9A/OS16 | P1 |
| M04-03 | Conservation of linear momentum | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Momentum, systems | Isolation criteria; 4W/12P/8G | PL/UCD9A | P1 |
| M04-04 | Center of mass | Upgrade | Freshman-Upper UG | High | https://physicslibrary.org/browse/objects/45.40.-f/ | Integrals, momentum | Discrete/continuous distributions; 4W/10P/5G | PL/UCD9A/OS16 | P1 |
| M04-05 | Center-of-mass motion | Upgrade | Freshman-Upper UG | High | https://physicslibrary.org/browse/objects/45.40.Cc/ | COM, momentum | External-force theorem; 3W/8P/4G | PL/UCD9A | P1 |
| M04-06 | Elastic and inelastic collisions | New/merge | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Momentum, energy | 1D collision classes and restitution; 5W/12P/8G | PL/UCD9A/OS16 | P1 |
| M04-07 | Two-dimensional collisions | New | Freshman | High | — | Vector momentum | Component method; 4W/10P/6G | UCD9A/OS16 | P1 |
| M04-08 | Angular momentum of a particle system | Upgrade | Upper UG | Medium | https://physicslibrary.org/browse/objects/45.40.Cc/ | Momentum, cross product | Origin/COM decomposition; 3W/8P/3G | PL/WB/WIKI | P2 |
| M04-09 | Variable-mass systems and rocket equation | New/upgrade | Upper UG | Medium | https://physicslibrary.org/browse/objects/45.50.-j/ | Momentum, calculus | Tsiolkovsky plus external forces; 4W/10P/3G | PL/WIKI/ORIGINAL | P2 |

## M05 — Elementary rotation, statics, and angular momentum

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M05-01 | Angular position, velocity, and acceleration | New | Freshman | High | — | Circular motion | Fixed-axis kinematics; 4W/10P/6G | MM/UCD9A/OS16 | P1 |
| M05-02 | Torque | New | Freshman | High | — | Cross product, force | Lever arm and vector form; 4W/10P/6G | MM/UCD9A | P1 |
| M05-03 | Moment of inertia | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.40.-f/ | Mass distribution, integrals | Discrete/continuous bodies; 4W/12P/6G | PL/MM/UCD9A | P1 |
| M05-04 | Parallel-axis theorem | New | Freshman | High | — | MOI, COM | Derivation and applications; 3W/10P/5G | MM/UCD9A | P1 |
| M05-05 | Rotational dynamics about a fixed axis | New | Freshman | High | — | Torque, MOI | Sum tau = I alpha; 5W/12P/8G | MM/UCD9A/OS16 | P1 |
| M05-06 | Rotational kinetic energy | New | Freshman | High | — | MOI, energy | Derivation, compound objects; 4W/10P/5G | UCD9A/OS16 | P1 |
| M05-07 | Rotational work and power | New | Freshman | High | — | Torque, energy | W=int tau dtheta, P=tau omega; 3W/8P/4G | MM/UCD9A | P1 |
| M05-08 | Angular momentum | Upgrade | Freshman-Upper UG | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Momentum, rotation | Particle/fixed-axis body; 4W/10P/6G | PL/UCD9A | P1 |
| M05-09 | Torque-angular momentum theorem | New | Freshman | High | — | Torque, angular momentum | dL/dt=tau; 4W/10P/6G | UCD9A/WIKI | P1 |
| M05-10 | Conservation of angular momentum | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Angular momentum | Skater/orbit/rotor examples; 4W/10P/6G | PL/UCD9A | P1 |
| M05-11 | Rolling without slipping | New | Freshman | High | — | Translation + rotation | Constraint, energy and friction; 5W/12P/8G | UCD9A/OS16 | P1 |
| M05-12 | Static equilibrium | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.40.Cc/ | FBDs, torque | 2D/3D equilibrium; 5W/12P/6G | PL/MM | P1 |
| M05-13 | Gyroscopic precession: elementary treatment | New | Upper UG | Medium | — | Angular momentum, torque | Fast-top approximation; 3W/8P/3G | UCD9A/WIKI | P2 |

## M06 — Gravitation and celestial mechanics

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M06-01 | Newton's law of universal gravitation | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.-j/ | Vectors, Newton | Vector form and superposition; 4W/10P/6G | PL/UCD9A/OS16 | P1 |
| M06-02 | Gravitational field and acceleration | New | Freshman | High | — | Gravitation | Field superposition; 3W/8P/4G | OS16/UCD9A | P1 |
| M06-03 | Gravitational potential energy | New | Freshman | High | — | Potential energy | U=-GMm/r; 4W/10P/6G | UCD9A/OS16 | P1 |
| M06-04 | Escape speed | New | Freshman | High | — | Energy, gravitation | Derivation and examples; 3W/8P/5G | UCD9A/OS16 | P1 |
| M06-05 | Circular orbits and orbital energy | New | Freshman | High | — | Circular dynamics, energy | Speed, period, total energy; 5W/12P/7G | UCD9A/OS16 | P1 |
| M06-06 | Kepler's first and second laws | Upgrade | Freshman-Upper UG | High | https://physicslibrary.org/browse/objects/45.50.Pk/ | Gravitation, angular momentum | Geometry plus dynamical origin; 4W/10P/5G | PL/UCD9A | P1 |
| M06-07 | Kepler's third law | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/45.50.Pk/ | Circular orbit | General two-body form; 4W/10P/6G | PL/UCD9A | P1 |
| M06-08 | Two-body reduction and reduced mass | New | Upper UG | Medium | — | COM, momentum | Relative-coordinate reduction; 3W/8P | WB/WIKI/ORIGINAL | P2 |
| M06-09 | Effective potential for orbital motion | New | Upper UG | Medium | — | Angular momentum, energy | Turning points and stable circular orbit; 4W/8P | WB/WIKI | P2 |

## M07 — Oscillations and resonance

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M07-01 | Simple harmonic oscillator | Correct/rewrite | Freshman | High | https://physicslibrary.org/encyclopedia/SimpleHarmonicOscillator.html | ODEs, Hooke law | Correct initial-condition solution, energy, phase; 5W/12P/8G | PL/UCD9A/OS16 | P0 |
| M07-02 | SHO energy and phase | New | Freshman | High | — | SHO | Energy exchange and phase-plane intro; 4W/10P/6G | UCD9A/OS16 | P1 |
| M07-03 | Simple pendulum | New | Freshman | High | — | Newton/torque | Small-angle approximation; 4W/10P/6G | OS16/UCD9A | P1 |
| M07-04 | Physical pendulum | New | Freshman-Upper UG | Medium | — | MOI, pendulum | Period and center of oscillation; 3W/8P/3G | OS16/WIKI | P2 |
| M07-05 | Damped harmonic oscillator | New | Freshman-Upper UG | High | — | SHO, ODEs | Under/critical/over damping; 4W/10P/5G | UCD9A/WIKI | P1 |
| M07-06 | Driven harmonic oscillator | New | Freshman-Upper UG | High | — | Damped oscillator | Steady-state amplitude and phase; 4W/10P/5G | UCD9A/WIKI | P1 |
| M07-07 | Resonance | Reclassify/upgrade | Freshman-Upper UG | High | https://physicslibrary.org/?from=objects&name=Resonance&op=getobj | Driven oscillator | Mechanical focus, linewidth and response; 4W/10P/5G | PL/UCD9A/WIKI | P0 |
| M07-08 | Quality factor and bandwidth | New | Upper UG | Medium | — | Resonance | Q definitions and energy loss; 3W/8P/3G | UCD9A/WIKI | P2 |
| M07-09 | Coupled oscillators | New | Upper UG | Medium | — | SHO, linear algebra | Two-mass systems; 4W/10P | UCD9A/WB | P2 |
| M07-10 | Normal modes and normal coordinates | New | Upper UG | Medium | — | Coupled oscillators | Eigenvector interpretation; 4W/10P | UCD9A/WB | P2 |
| M07-11 | Anharmonic oscillation | Reclassify/expand | Upper UG | Low | https://physicslibrary.org/?from=objects&name=Anharmonic&op=getobj | SHO | Duffing-style terms, period shift; 3W/8P | PL/WIKI/ORIGINAL | P0 |
| M07-12 | Nonlinear pendulum | New | Upper UG | Low | https://physicslibrary.org/encyclopedia/ApplicationsOfTheMaclaurinSeriesInPhysicalModeling.html | Pendulum, energy | Beyond small angle, phase portrait; 3W/8P | PL/WIKI/ORIGINAL | P2 |

## M08 — Fluids and elasticity

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M08-01 | Density and pressure | New | Freshman | High | — | Units | Definitions and manometry; 3W/10P/5G | OS16/WIKI | P1 |
| M08-02 | Hydrostatic pressure | New | Freshman | High | — | Pressure, calculus | dp/dz=-rho g; 4W/10P/6G | OS16/WIKI | P1 |
| M08-03 | Pascal's principle | New | Freshman | Medium | — | Pressure | Hydraulic applications; 3W/8P/3G | OS16/WIKI | P1 |
| M08-04 | Archimedes' principle | Upgrade | Freshman | High | https://physicslibrary.org/browse/objects/47.85.Dh/ | Hydrostatics | Derivation, floating objects; 4W/10P/5G | PL/OS16 | P1 |
| M08-05 | Fluid continuity equation | Upgrade | Freshman-Upper UG | High | https://physicslibrary.org/browse/objects/47.10.%2Bg/ | Mass conservation | 1D incompressible to differential form; 4W/10P/5G | PL/OS16/WIKI | P1 |
| M08-06 | Bernoulli equation | New | Freshman | High | — | Energy, continuity | Derivation, applications, limitations; 5W/12P/7G | OS16/WIKI | P1 |
| M08-07 | Viscosity and Newtonian fluids | New | Freshman-Upper UG | Medium | — | Fluid kinematics | Shear stress and viscosity; 3W/8P/3G | OS16/WIKI | P1 |
| M08-08 | Poiseuille flow | New | Upper UG | Medium | — | Viscosity, pressure | Pipe-flow scaling; 3W/8P/3G | OS16/WIKI | P2 |
| M08-09 | Reynolds number and flow regimes | New | Upper UG | Medium | — | Dimensional analysis | Laminar/turbulent interpretation; 3W/8P/3G | WIKI/ORIGINAL | P2 |
| M08-10 | Reynolds transport theorem | Upgrade/bridge | Upper UG | Low | https://physicslibrary.org/browse/objects/47.10.%2Bg/ | Control volumes | Add concrete mechanics examples; 2W/6P | PL/MM/WIKI | P3 |
| M08-11 | Stress and strain | New | Freshman-Upper UG | Medium | — | Forces, geometry | Normal/shear stress/strain; 4W/10P/3G | OS16/WIKI | P2 |
| M08-12 | Elastic moduli and elastic energy | New | Freshman-Upper UG | Medium | — | Stress/strain | Young/shear/bulk moduli and energy; 4W/10P/3G | OS16/WIKI | P2 |

## M09 — Constraints and Lagrangian mechanics

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M09-01 | Generalized coordinates | Upgrade hub | Upper UG | High | https://physicslibrary.org/browse/objects/45.20.Jj/ | Coordinates, DOF | Unify current examples and notation; 4W/10P/4G | PL/WB/WIKI | P1 |
| M09-02 | Constraints in classical mechanics | New | Upper UG | Medium | — | DOF, generalized coordinates | Holonomic/nonholonomic; scleronomic/rheonomic; 4W/10P | WB/WIKI | P2 |
| M09-03 | Virtual displacement | New | Upper UG | Low | — | Constraints | Allowed variations and examples; 3W/8P | WB/WIKI | P2 |
| M09-04 | Virtual work and d'Alembert's principle | New | Upper UG | Low | — | Virtual displacement, Newton | Constraint-force elimination; 3W/8P | WB/WIKI/ORIGINAL | P2 |
| M09-05 | Calculus of variations for mechanics | New bridge | Upper UG | Medium | — | Calculus | Functionals, first variation, Euler-Lagrange; 4W/10P | WIKI/ORIGINAL | P2 |
| M09-06 | Hamilton's principle | Upgrade | Upper UG | High | https://physicslibrary.org/browse/objects/45.20.Jj/ | Variational calculus | Action stationarity, endpoint conditions; 4W/10P/4G | PL/WB/WIKI | P1 |
| M09-07 | Lagrange's equations | Upgrade | Upper UG | High | https://physicslibrary.org/browse/objects/45.20.Jj/ | Hamilton principle | Derivation and canonical examples; 5W/12P/5G | PL/WB/WIKI | P1 |
| M09-08 | Generalized forces | New | Upper UG | Medium | — | Lagrange equations | Nonconservative force treatment; 3W/8P/2G | WB/WIKI | P2 |
| M09-09 | Lagrange multipliers in constrained dynamics | New | Upper UG | Medium | — | Constraints, Lagrange equations | Pendulum/contact examples; 4W/10P/2G | WB/WIKI | P2 |
| M09-10 | Generalized momentum | New | Upper UG | High | — | Lagrangian | p_i = partial L / partial qdot_i; 3W/8P/3G | WB/WIKI | P1 |
| M09-11 | Cyclic coordinates and first integrals | New | Upper UG | Medium | — | Generalized momentum | Conservation shortcuts; 4W/10P/3G | WB/WIKI | P2 |
| M09-12 | Noether's theorem in classical mechanics | New | Upper UG-Graduate | Medium | — | Variational mechanics | Time/translation/rotation symmetries; 4W/10P | WIKI/ORIGINAL | P2 |

## M10 — Three-dimensional and non-inertial dynamics

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M10-01 | Three-dimensional particle dynamics | New hub | Upper UG/GRE | High | — | Vector kinematics, Newton | Cartesian/cylindrical/spherical examples; 4W/10P/5G | WB/WIKI/ORIGINAL | P1 |
| M10-02 | Time derivatives in rotating frames | New | Upper UG | High | — | Vectors, angular velocity | Transport theorem; 4W/10P/4G | WB/WIKI/ORIGINAL | P1 |
| M10-03 | Translating non-inertial frames | New | Upper UG | High | — | Reference frames | Translational fictitious force; 3W/8P/3G | WB/WIKI | P1 |
| M10-04 | Rotating reference frames | New | Upper UG | High | — | Transport theorem | Full velocity/acceleration relation; 4W/10P/5G | WB/WIKI | P1 |
| M10-05 | Centrifugal force | New | Upper UG | High | — | Rotating frames | Effective-potential examples; 3W/8P/4G | WB/WIKI | P1 |
| M10-06 | Coriolis force | New | Upper UG | High | — | Rotating frames | Earth and turntable examples; 4W/10P/5G | WB/WIKI | P1 |
| M10-07 | Euler force | New | Upper UG | Medium | — | Rotating frames | Time-varying angular velocity; 3W/8P/2G | WIKI/ORIGINAL | P2 |
| M10-08 | Foucault pendulum | New | Upper UG | Medium | — | Coriolis, oscillations | Latitude dependence; 3W/8P/2G | WIKI/ORIGINAL | P2 |

## M11 — Central-force mechanics and scattering

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M11-01 | Motion in a central-force field | Upgrade | Upper UG | Medium | https://physicslibrary.org/browse/objects/45.50.Pk/ | Angular momentum, Lagrangian | Plane motion and conserved quantities; 4W/10P | PL/WB/WIKI | P2 |
| M11-02 | Central-force effective potential | New | Upper UG | Medium | — | Central-force motion | General U_eff and orbit stability; 4W/10P | WB/WIKI | P2 |
| M11-03 | Orbit equation and Binet's equation | New | Upper UG | Medium | — | Central-force motion | u(theta) derivation; 4W/10P | WB/WIKI/ORIGINAL | P2 |
| M11-04 | Kepler problem from the orbit equation | New | Upper UG | Medium | — | Binet equation | Conic solution; 4W/10P | WB/WIKI | P2 |
| M11-05 | Laplace-Runge-Lenz vector | New | Upper UG-Graduate | Low | — | Kepler problem | Hidden symmetry and orbit geometry; 3W/8P | WIKI/ORIGINAL | P3 |
| M11-06 | Bertrand's theorem | New | Graduate | Low | — | Central-force orbits | Statement, intuition, proof sketch; 2W/6P | WIKI/ORIGINAL | P3 |
| M11-07 | Classical scattering kinematics | New | Upper UG | Medium | — | Central forces | Impact parameter and scattering angle; 3W/8P | WB/WIKI | P2 |
| M11-08 | Differential scattering cross section | New | Upper UG | Medium | — | Scattering kinematics | d sigma / d Omega derivation; 3W/8P | WB/WIKI | P2 |
| M11-09 | Rutherford scattering | New | Upper UG | Medium | — | Cross section, inverse-square force | Full classical derivation; 4W/10P | WB/WIKI | P2 |

## M12 — Small oscillations and normal modes

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M12-01 | Linearization about equilibrium | New | Upper UG | Medium | — | Taylor expansion, potential | Hessian/stability bridge; 3W/8P | WIKI/ORIGINAL | P2 |
| M12-02 | Two-degree-of-freedom oscillators | New | Upper UG | Medium | — | Coupled oscillators | Mass-spring examples; 4W/10P | UCD9A/WB | P2 |
| M12-03 | Mass and stiffness matrices | New | Upper UG | Low | — | Linear algebra, Lagrange | M qddot + K q = 0; 3W/8P | WB/ORIGINAL | P2 |
| M12-04 | Generalized eigenvalue problem for modes | New | Upper UG | Low | — | M/K matrices | det(K-omega^2 M)=0; 3W/8P | WB/ORIGINAL | P2 |
| M12-05 | Orthogonality of normal modes | New | Graduate | Low | — | Eigenproblem | M/K orthogonality proof; 2W/6P | ORIGINAL | P3 |
| M12-06 | Normal-coordinate transformation | New | Upper UG-Graduate | Low | — | Normal modes | Modal decoupling derivation; 3W/8P | WB/ORIGINAL | P2 |
| M12-07 | Continuum limit of a mass-spring chain | New | Graduate bridge | Low | — | Normal modes | Derive wave equation; 3W/8P | WIKI/ORIGINAL | P3 |

## M13 — Rigid-body kinematics and dynamics

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M13-01 | Rigid body | Upgrade hub | Upper UG | Medium | https://physicslibrary.org/browse/objects/45.40.Cc/ | Particle systems | DOF and kinematics overview; 3W/8P | PL/WB/WIKI | P2 |
| M13-02 | Existing DCM/Euler/axis-angle/quaternion article family | Retain/reorder | Upper UG | Low | https://physicslibrary.org/browse/objects/45.40.-f/ | Elementary rotation, frames | Cross-link as representation subpath; add prerequisite headers | PL | P2 |
| M13-03 | Angular velocity of a rigid body | New/merge | Upper UG | Medium | https://physicslibrary.org/browse/objects/45.40.-f/ | Rigid rotation | Body/inertial components; 4W/10P | PL/WB/WIKI | P2 |
| M13-04 | Inertia tensor | Upgrade | Upper UG | Medium | https://physicslibrary.org/browse/objects/45.40.-f/ | MOI, matrices | Tensor derivation and transformation; 4W/10P | PL/WB/WIKI | P2 |
| M13-05 | Principal axes and principal moments | New | Upper UG | Medium | — | Inertia tensor, eigenvectors | Diagonalization and physical meaning; 4W/10P | WB/WIKI | P2 |
| M13-06 | Rigid-body angular momentum L = I omega | New | Upper UG | Medium | — | Inertia tensor, angular velocity | Nonparallel L and omega; 4W/10P | WB/WIKI | P2 |
| M13-07 | Euler's equations of rigid-body motion | Upgrade | Upper UG-Graduate | Medium | https://physicslibrary.org/browse/objects/45.40.-f/ | Rotating frames, inertia tensor | Derive in body frame; 4W/10P | PL/WB/WIKI | P2 |
| M13-08 | Torque-free rigid-body motion | New | Graduate | Low | — | Euler equations | Intermediate-axis theorem; 3W/8P | WB/WIKI/ORIGINAL | P3 |
| M13-09 | Symmetric top, precession, and nutation | New | Graduate | Low | — | Euler equations, Lagrangian | Heavy/symmetric top; 4W/10P | WB/WIKI/ORIGINAL | P3 |

## M14 — Hamiltonian and Poisson mechanics

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M14-01 | Legendre transform in mechanics | New | Upper UG | High | — | Lagrangian, generalized momentum | Geometric/algebraic derivation; 4W/10P/3G | WB/WIKI/ORIGINAL | P1 |
| M14-02 | Hamiltonian | New | Upper UG | High | — | Legendre transform | Definition, energy relation, examples; 4W/10P/4G | WB/WIKI | P1 |
| M14-03 | Hamilton's equations | New | Upper UG | High | — | Hamiltonian | Derivation + oscillator/central-force examples; 5W/12P/5G | WB/WIKI | P1 |
| M14-04 | Phase space | New | Upper UG | Medium | — | Hamilton's equations | Trajectories, flow, fixed points; 4W/10P/2G | WB/WIKI | P2 |
| M14-05 | Hamiltonian harmonic oscillator | New worked example | Upper UG | Medium | — | Hamilton's equations, SHO | Phase ellipse and canonical solution; 3W/8P/2G | WB/WIKI | P2 |
| M14-06 | Poisson bracket | New/replace thin bridge | Upper UG-Graduate | Medium | https://physicslibrary.org/browse/objects/45.20.-d/ | Hamilton's equations | Definition, algebra, examples; 4W/10P | WB/WIKI | P2 |
| M14-07 | Poisson brackets and time evolution | New | Graduate | Low | — | Poisson bracket | df/dt relation; 3W/8P | WB/WIKI | P3 |
| M14-08 | Canonical variables and constants of motion | New | Graduate | Low | — | Poisson brackets | Fundamental brackets and conserved quantities; 3W/8P | WB/WIKI | P3 |
| M14-09 | Liouville's theorem | New | Graduate | Low | — | Phase space, Hamilton equations | Phase-volume conservation; 3W/8P | WIKI/ORIGINAL | P3 |
| M14-10 | Symplectic structure of Hamiltonian mechanics | New | Graduate | Low | — | Canonical variables, linear algebra | Symplectic form and maps; 3W/8P | WB/WIKI/ORIGINAL | P3 |

## M15 — Canonical transformations, Hamilton-Jacobi, action-angle, perturbation

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M15-01 | Canonical transformations | New | Graduate | Low | — | Hamiltonian mechanics | Definition and symplectic condition; 3W/8P | WB/WIKI/ORIGINAL | P3 |
| M15-02 | Generating functions F1-F4 | New | Graduate | Low | — | Canonical transformations | Four types, transformation equations, examples; 4W/10P | WIKI/ORIGINAL | P3 |
| M15-03 | Infinitesimal canonical transformations | New | Graduate | Low | — | Poisson brackets, canonical transforms | Generators and symmetry; 3W/8P | WIKI/ORIGINAL | P3 |
| M15-04 | Hamilton-Jacobi equation | New | Graduate | Low | — | Canonical transformations | Derivation and interpretation; 4W/10P | WB/WIKI/ORIGINAL | P3 |
| M15-05 | Hamilton's principal and characteristic functions | New | Graduate | Low | — | HJ equation | S versus W and complete integrals; 3W/8P | WIKI/ORIGINAL | P3 |
| M15-06 | Separation of variables in Hamilton-Jacobi theory | New | Graduate | Low | — | HJ equation | Oscillator and central-force examples; 4W/10P | WB/ORIGINAL | P3 |
| M15-07 | Action-angle variables | New | Graduate | Low | — | HJ theory, periodic motion | Definitions, geometry, frequencies; 4W/10P | WIKI/ORIGINAL | P3 |
| M15-08 | Harmonic oscillator in action-angle variables | New worked example | Graduate | Low | — | Action-angle variables | Compute J and theta; 3W/8P | ORIGINAL | P3 |
| M15-09 | Adiabatic invariants | New | Graduate | Low | — | Action variables | Slowly varying systems; 3W/8P | WIKI/ORIGINAL | P3 |
| M15-10 | Canonical perturbation theory | New | Graduate | Low | — | Action-angle variables | Near-integrable Hamiltonians; 3W/8P | WIKI/ORIGINAL | P3 |
| M15-11 | Secular terms and averaging | New | Graduate | Low | — | Perturbation theory | Oscillator/orbit examples; 3W/8P | WIKI/ORIGINAL | P3 |

## M16 — Nonlinear dynamics, continuum, and relativistic bridge

| ID | Article | Status | Level | GRE | Current PL | Prerequisites | Minimum deliverable | Source | Priority |
|---|---|---|---|---|---|---|---|---|---|
| M16-01 | Phase portraits and fixed points | New | Upper UG-Graduate | Low | — | ODEs, phase space | Fixed-point classification and examples; 4W/10P | WIKI/ORIGINAL | P3 |
| M16-02 | Linear stability of dynamical systems | New | Graduate | Low | — | Jacobians, eigenvalues | Mechanical examples; 3W/8P | WIKI/ORIGINAL | P3 |
| M16-03 | Bifurcations in mechanical systems | New | Graduate | Low | — | Stability | Saddle-node/pitchfork/Hopf examples; 3W/8P | WIKI/ORIGINAL | P3 |
| M16-04 | Poincare sections and deterministic chaos | New | Graduate | Low | — | Nonlinear ODEs | Construction, interpretation, sensitivity; 4W/10P | WIKI/ORIGINAL | P3 |
| M16-05 | Lagrangian density and field Euler-Lagrange equations | New | Graduate | Low | — | Variational mechanics | Discrete-to-continuum bridge; 4W/10P | WIKI/ORIGINAL | P3 |
| M16-06 | Vibrating string from a variational principle | New worked example | Graduate | Low | — | Field Euler-Lagrange | Derive wave equation; 3W/8P | WIKI/ORIGINAL | P3 |
| M16-07 | Continuum mechanics overview | New hub | Upper UG-Graduate | Low | https://physicslibrary.org/browse/objects/46-XX/ | Stress/strain, fields | Solids/fluids roadmap; 3W/8P | WIKI/ORIGINAL | P3 |
| M16-08 | Relativistic particle mechanics | New bridge | Upper UG | Separate GRE category | — | Special relativity, Lagrangian | Action, momentum, energy; 4W/10P | WIKI/ORIGINAL | P3 |
| M16-09 | Relativistic Lagrangian and Hamiltonian | New | Graduate | Separate GRE category | — | Relativistic particle mechanics | Canonical formulation; 3W/8P | WIKI/ORIGINAL | P3 |

---

# 7. Exercise-bank backlog

Article creation and exercise creation should proceed together. Do not postpone exercises until after the article corpus is written.

## Required problem types

Every core section should include:

1. **Concept checks** — signs, directions, conservation-law recognition, limiting cases.
2. **Standard calculations** — conventional homework-length problems.
3. **Derivations** — upper-undergraduate/graduate mathematical development.
4. **Computational/visual problems** — numerical integration, phase plots, effective potentials, orbit plots, normal-mode visualization, Poincare sections.
5. **GRE-speed problems** — short multiple-choice questions emphasizing scaling, ratios, dimensional analysis, conservation shortcuts and equation recognition.

## Naming convention

Use stable identifiers independent of article titles, for example:

- `MECH-KIN-001`
- `MECH-NEWTON-014`
- `MECH-ENERGY-021`
- `MECH-ROT-032`
- `MECH-GRAV-018`
- `MECH-OSC-027`
- `MECH-LAGRANGE-012`
- `MECH-HAM-009`

Recommended metadata per exercise:

- level: Freshman / GRE / Upper Undergraduate / Graduate;
- type: Concept / Calculation / Derivation / Computational;
- difficulty: 1-5;
- estimated time;
- prerequisites;
- answer / hint / full-solution status;
- source/provenance and license if adapted.

## Exercise quantity targets

| Deliverable | Target |
|---|---:|
| Fully worked examples | 150-200 |
| Introductory practice exercises | 250-300 |
| Upper-undergraduate exercises | 200-250 |
| Graduate/Goldstein-level exercises | 100-150 |
| GRE-tagged questions | 250+ |
| Mixed GRE mechanics mini-tests | 8-10 sets of about 14 questions |

The GRE-tagged pool can overlap the main practice bank; the long-term goal is roughly **600-750 distinct mechanics exercises**, with at least **250 carrying a GRE tag**.

# 8. Milestones and recommended build order

## Milestone A — P0 cleanup

1. Correct/rewrite SHO.
2. Reclassify resonance and anharmonic material.
3. Create the Mechanics Learning Path.
4. Clean obvious PACS misclassification/cross-linking issues.
5. Add consistent article metadata: level, prerequisites, next article, GRE tag, examples, exercises, source/license.

## Milestone B — Freshman mechanics + complete GRE mechanics coverage

Complete **all P1 rows** in approximately this order:

1. M00-M02: foundations, kinematics, Newtonian dynamics.
2. M03-M04: energy and momentum.
3. M05-M06: elementary rotation and gravitation.
4. M07-M08: oscillations and fluids.
5. M10: 3D/non-inertial dynamics.
6. M09 and M14 P1 rows: generalized coordinates, Hamilton principle, Lagrange equations, generalized momentum, Legendre transform, Hamiltonian and Hamilton's equations.

**Definition of done:** every explicit ETS classical-mechanics bullet has at least one coherent article path, worked examples, practice problems and GRE-speed problems.

## Milestone C — Upper-undergraduate analytical mechanics

Complete P2 material:

- constraints and d'Alembert;
- central forces and scattering;
- coupled/small oscillations;
- inertia tensor/principal axes/Euler equations;
- phase space and Poisson brackets;
- stronger fluids/elasticity bridge.

## Milestone D — Goldstein-level completion

Complete P3 material:

- advanced rigid-body motion;
- Poisson/symplectic mechanics;
- canonical transformations;
- Hamilton-Jacobi theory;
- action-angle variables;
- canonical perturbation theory;
- nonlinear dynamics and chaos;
- continuum variational mechanics;
- relativistic mechanics bridge.

# 9. Article definition of done

A new or substantially revised mechanics article should contain, when appropriate:

1. Concept and physical intuition.
2. Definitions and assumptions.
3. Mathematical formulation.
4. Derivation rather than only the final equation.
5. Units/dimensional checks.
6. Limiting or special cases.
7. At least one worked example; core articles should have several.
8. Common mistakes and sign/convention warnings.
9. Exercises with stable IDs.
10. GRE-speed exercises for P1/GRE-relevant topics.
11. Prerequisite and next-article links.
12. Bibliography.
13. Explicit source/provenance/license note for adapted OER text or figures.

# 10. Immediate first sprint

The first mechanics sprint should be deliberately narrow enough to establish the article/exercise template while delivering major student value.

### Sprint 1 recommended items

- M00-01 Mechanics learning path.
- M02-02 Free-body diagrams.
- M03-03 Work-energy theorem.
- M05-01 Angular position, velocity and acceleration.
- M05-02 Torque.
- M05-05 Rotational dynamics about a fixed axis.
- M07-01 SHO correction/rewrite.
- M08-01 Density and pressure.
- M08-02 Hydrostatic pressure.
- M08-06 Bernoulli equation.

For each Sprint 1 article, create the full article plus its worked examples and exercise set before moving it to done. This sprint establishes the reusable mechanics format and closes several of the most visible undergraduate/GRE gaps immediately.
