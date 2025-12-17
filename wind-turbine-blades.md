---
layout: default
title: Small Wind-Turbine Blades Design Project
permalink: /projects/wind-turbine-blades/
---

<style>
  .site-header,
  body > .wrapper > header,
  .wrapper > *:first-child {
    display: none !important;
  }

  body {
    background-color: #fff6ed;
    color: #000;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  }

  .wrapper {
    max-width: 900px;
    margin: 0 auto;
    padding: 3rem 1.5rem 4rem;
  }

  .page-shell {
    padding-top: 0;
    padding-bottom: 4rem;
  }

  .back-link {
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
    font-size: 0.9rem;
    text-decoration: none;
    color: #333;
    margin-bottom: 1.5rem;
  }

  .back-link::before {
    content: "←";
    font-size: 1rem;
  }

  .page-shell h1 {
    font-family: "Agrandir", system-ui, -apple-system, BlinkMacSystemFont,
      "Segoe UI", sans-serif;
    font-size: clamp(2.2rem, 4vw, 3rem);
    margin-bottom: 0.75rem;
  }

  .project-meta {
    font-size: 0.9rem;
    color: #555;
    margin-bottom: 1.8rem;
  }

  .pill-card {
    border-radius: 32px;
    padding: 1.4rem 1.8rem;
    border: 2px solid transparent;
    margin-bottom: 1.2rem;
    background-color: #f7f2ec;
  }

  .pill-card--green {
    background-color: #e5ecdd;
    border-color: #d6dfcc;
  }

  .pill-card--purple {
    background-color: #e8e5f2;
    border-color: #babbdd;
  }

  .pill-card--blue {
    background-color: #e3f1ff;
    border-color: #a6cff5;
  }

  .pill-card h2 {
    margin-top: 0;
  }

  .image-block {
    margin: 2rem 0;
    text-align: center;
  }

  .image-block img {
    max-width: 100%;
    border-radius: 16px;
    box-shadow: 0 8px 22px rgba(0, 0, 0, 0.08);
  }

  .image-caption {
    font-size: 0.85rem;
    color: #555;
    margin-top: 0.4rem;
  }
</style>

<div class="page-shell">

  <a class="back-link" href="{{ site.baseurl }}/">Back to Home</a>

  <h1>Small Wind-Turbine Blades Design Project</h1>
  <div class="project-meta">
    MAE 4272 – Fluids and Heat Transfer Laboratory
  </div>

  <div class="pill-card pill-card--green">
    <h2>Project Overview</h2>
    <p>
      The objective of this project was to develop a small wind-turbine blade
      design that produced maximum power at a chosen angular velocity. The wind
      conditions in the wind tunnel were based on a Weibull velocity
      distribution between 3 and 7&nbsp;m/s. Our experimental constraints
      included the wind tunnel’s operating limits and the magnetic particle
      torque brake’s maximum allowable torque.
    </p>
    <p>
      We did not use an electrical generator directly. Instead, we mechanically
      modeled power generation: varying the brake voltage in our LabVIEW VI
      allowed us to replicate how a generator would load the rotor, using the
      relationship
      <strong>P = Ω · T</strong> (power equals angular velocity times torque).
    </p>
  </div>

  <div class="pill-card pill-card--purple">
    <h2>Blade Design and Methodology</h2>
    <p>
      Our final blade was a blend of two airfoils: NACA&nbsp;4412 at the root
      and NACA&nbsp;6409 near the tip. We implemented this with nine total
      cross sections, using four NACA&nbsp;4412 sections that smoothly
      transitioned into five NACA&nbsp;6409 sections from root to tip.
    </p>
    <p>
      NACA&nbsp;4412 has a thicker chord and a more gradual increase in lift
      with relatively higher drag, making it well suited near the root where
      structural loading and bending moments at the hub are largest. In
      contrast, NACA&nbsp;6409 offers a higher lift-to-drag ratio over our
      operating range, making it ideal near the tip where local flow velocities
      are higher and minimizing drag is critical for efficiency.
    </p>
    <p>
      We created a MATLAB script using a blade element approach to automate
      and optimize the geometry. Airfoil polars guided our selection, and we
      incorporated spanwise twist to maintain an optimal angle of attack along
      the blade length.
    </p>

  </div>
  <div class="image-block">
    <img src="{{ site.baseurl }}/assets/images/bladedesign.png"
         alt="Efficiency versus tip-speed ratio">
    <div class="image-caption">
      Blade Modeled in Fusion360
    </div>
  </div>

  </div>
  <div class="image-block">
    <img src="{{ site.baseurl }}/assets/images/blades.png"
         alt="Efficiency versus tip-speed ratio">
    <div class="image-caption">
      3D Printed blades in wind tunnel
    </div>
  </div>

  <div class="pill-card pill-card--blue">
    <h2>Testing, Power Curves, and Efficiency</h2>
    <p>
      We evaluated performance in the wind tunnel by testing across a range of
      wind speeds to generate power curves and estimate turbine efficiency. For
      each wind speed, torque was incrementally increased with the magnetic
      particle brake until the turbine stalled. At each operating point we
      recorded the free-stream wind speed <em>U</em> (via pitot-static tube),
      torque <em>T</em>, rotational speed Ω in RPM, and power
      <em>P = Ω · T</em>.
    </p>
    <p>
      Across six trials (wind speeds from 2.9 to 5.8&nbsp;m/s), the data
      produced clean power curves and enabled an efficiency analysis in terms
      of tip-speed ratio λ and power coefficient <em>C<sub>p</sub></em>. We
      found that the turbine reached its highest efficiency at a tip-speed
      ratio of roughly λ ≈ 6, with an optimal operating speed of
      <strong>1360.83&nbsp;RPM</strong> for the 5.2&nbsp;m/s case.
    </p>
  </div>

  <div class="image-block">
    <img src="{{ site.baseurl }}/assets/images/wind-power-curves.png"
         alt="Measured power curves at multiple wind speeds">
    <div class="image-caption">
      Measured power curves for wind speeds between 2.9 and 5.8&nbsp;m/s.
    </div>
  </div>

  <div class="image-block">
    <img src="{{ site.baseurl }}/assets/images/wind-efficiency-tsr.png"
         alt="Efficiency versus tip-speed ratio">
    <div class="image-caption">
      Turbine efficiency (power coefficient <em>C<sub>p</sub></em>) as a
      function of tip-speed ratio λ, showing peak performance near λ ≈ 6.
    </div>
  </div>

  <div class="pill-card pill-card--green">
    <h2>My Contribution</h2>
    <p>
      I developed the final MATLAB script used to generate the blade element
      geometry for all cross sections and to support the optimization of twist
      and chord distributions. Using this script output and the design
      requirements for our target operating condition, I then modeled the full
      blade and hub attachment in Fusion&nbsp;360, translating the calculated
      geometry into a manufacturable 3D design ready for printing and
      wind-tunnel testing.
    </p>
  </div>

<p>View my actual portfolio <a href="https://maesliwinski.com" target="_blank" rel="noopener noreferrer">here</a>.</p>
</div>
