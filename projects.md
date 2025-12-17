---
layout: default
title: Projects
permalink: /projects/
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
    margin-bottom: 1.5rem;
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

  .pill-card-subtitle {
    font-size: 0.9rem;
    margin-bottom: 0.4rem;
    color: #555;
  }

  .tag-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin-top: 0.8rem;
  }

  .tag-chip {
    padding: 0.25rem 0.7rem;
    border-radius: 999px;
    background-color: rgba(255, 255, 255, 0.9);
    border: 1px solid rgba(0, 0, 0, 0.06);
    font-size: 0.8rem;
  }
</style>

<div class="page-shell">

  <a class="back-link" href="{{ site.baseurl }}/">Back to Home</a>

  <h1>Projects</h1>

  <div class="pill-card pill-card--green">
    <h2>Assistive Pen Holders</h2>
    <p class="pill-card-subtitle">
      Adaptive writing tools for users with limited grip strength
    </p>
    <p>
      Designed and prototyped customizable pen holders that improve comfort,
      control, and accessibility for individuals with fine motor challenges.
    </p>
    <div class="tag-row">
      <span class="tag-chip">Human-Factors</span>
      <span class="tag-chip">3D Printing</span>
      <span class="tag-chip">Assistive Tech</span>
    </div>
  </div>

  <div class="pill-card pill-card--purple">
    <h2>Custom Wheelchair Table</h2>
    <p class="pill-card-subtitle">
      Modular work surface for school and daily use
    </p>
    <p>
      Created a removable table system tailored to a wheelchair user's posture
      and reach, balancing stability, portability, and ease of use.
    </p>
    <div class="tag-row">
      <span class="tag-chip">Ergonomics</span>
      <span class="tag-chip">Prototyping</span>
      <span class="tag-chip">User Testing</span>
    </div>
  </div>

</div>
