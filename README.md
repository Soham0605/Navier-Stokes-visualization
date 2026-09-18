# Navier-Stokes-visualization

# 🌊 Navier–Stokes Cinematic

### An interactive visualization of fluid dynamics, turbulence, and the $1 Million Millennium Problem

[**▶️ Launch the Interactive Simulation**](https://soham0605.github.io/Navier-Stokes-visualization/)

> Click, drag, experiment, and watch a mathematical equation turn into moving fluid.

---

## Why is everyone suddenly talking about Navier–Stokes?

The Navier–Stokes equations are not new.

They were developed in the 19th century and have been used for generations to describe the motion of fluids such as water and air. They appear throughout physics and engineering: aerodynamics, oceanography, weather, combustion, fluid machinery, and many other fields.

So why are they suddenly appearing everywhere?

Because in September 2026, the problem surrounding the mathematical behavior of the Navier–Stokes equations became part of a major discussion about artificial intelligence and mathematical research.

The Navier–Stokes existence and smoothness problem is one of the seven Millennium Prize Problems established by the Clay Mathematics Institute in 2000. Each problem carries a $1 million prize.

Recent AI-assisted mathematical work has brought renewed attention to the Navier–Stokes problem. The Clay Mathematics Institute announced on September 11, 2026 that the problem had apparently been settled, while also emphasizing that the proposed solution must go through the Institute's established verification process.

This project was created to answer a much simpler question:

> **What actually is the equation everyone is talking about?**

You don't need a graduate degree in mathematics to get an intuition for it.

---

# 🧩 What is the Navier–Stokes equation?

At its simplest, the Navier–Stokes equation is a mathematical statement of:

> **How does a fluid's velocity change because of its own motion, viscosity, pressure, and external forces?**

For an incompressible Newtonian fluid, a common form is

\[
\boxed{
\frac{\partial \mathbf{u}}{\partial t}
+
(\mathbf{u}\cdot\nabla)\mathbf{u}
=
-\nabla p
+
\nu\nabla^2\mathbf{u}
+
\mathbf{f}
}
\]

together with the incompressibility condition

\[
\boxed{
\nabla\cdot\mathbf{u}=0
}
\]

Think of the fluid as an enormous collection of tiny neighboring regions.

Every region has a velocity.

The equation tells us how those velocities change.

---

# 🔬 What do the terms mean?

## 1. Velocity

\[
\mathbf{u}
\]

This is the fluid velocity field.

In 2D,

\[
\mathbf{u}=(u,v)
\]

where:

- \(u\) = velocity in the x direction
- \(v\) = velocity in the y direction

Instead of assigning one velocity to the entire fluid, we assign a velocity to **every location**.

```text
→ → → → → → →
→ → ↗ ↗ → → →
→ ↗ ↑ ↑ ↘ → →
→ → ↘ ↘ → → →
