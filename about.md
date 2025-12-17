---
layout: default
title: About Me
permalink: /about/
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

  .pill-card--blue {
    background-color: #e3f1ff;
    border-color: #a6cff5;
  }

  .pill-card-subtitle {
    font-size: 0.9rem;
    margin-bottom: 0.4rem;
    color: #555;
  }
</style>

<div class="page-shell">

  <a class="back-link" href="{{ site.baseurl }}/">Back to Home</a>

  <h1>About Me</h1>

  <p>
    Hello! I'm Mae Sliwinski, a mechanical engineering student passionate about human-centered design and product design.
  </p>

  <p>
    At Cornell, I've combined mechanical engineering fundamentals with an
    interest in assistive technologies and robotics.
  </p>

  <h2>Expertise</h2>

  <div class="pill-card pill-card--green">
    <h3>Human-Centered Design</h3>
    <p class="pill-card-subtitle">
      Accessibility, ergonomics, user research
    </p>
    <p>
      Designing products around real users, with a focus on usability and comfort 
    </p>
  </div>

  <div class="pill-card pill-card--purple">
    <h3>Mechanical Design &amp; Prototyping</h3>
    <p class="pill-card-subtitle">
      CAD, 3D printing, testing
    </p>
    <p>
      Experience taking ideas from sketches to functional prototypes using CAD, rapid prototyping, and iterative testing.
    </p>
  </div>

  <div class="pill-card pill-card--blue">
    <h3>Leadership &amp; Operations</h3>
    <p class="pill-card-subtitle">
      Teams of 50–120+ people
    </p>
    <p>
      Leading large teams and coordinating logistics to deliver solutions that are thoughtful and drive productivity.
    </p>
  </div>

<p>View my actual portfolio <a href="https://maesliwinski.com" target="_blank" rel="noopener noreferrer">here</a>.</p>

