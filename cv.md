---
layout: default
title: Curriculum Vitae
permalink: /cv/
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
    margin-bottom: 1.2rem;
  }

  .cv-button {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.9rem 1.9rem;
    border-radius: 999px;
    background-color: #d6dfcc;
    border: 2px solid #d6dfcc;
    text-decoration: none;
    color: #000;
    font-weight: 500;
    margin-bottom: 1.5rem;
  }

  .cv-button:hover {
    background-color: #f2b48f;
    border-color: #f2b48f;
  }

  .cv-button::before {
    content: "↓";
    font-size: 1rem;
  }

  .cv-frame-wrapper {
    margin-top: 0.5rem;
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
  }

  .cv-frame-wrapper iframe {
    border: none;
    display: block;
  }
</style>

<div class="page-shell">

  <a class="back-link" href="{{ site.baseurl }}/">Back to Home</a>

  <h1>Curriculum Vitae</h1>

  <p>
    I am seeking full-time Mechanical Engineering and design roles
    starting in June 2026.
  </p>

  <a
    class="cv-button"
    href="{{ site.baseurl }}/assets/Madeline%20Mae%20Sliwinski%20Resume.pdf"
    target="_blank"
  >
    View Resume PDF
  </a>

  <div class="cv-frame-wrapper">
    <iframe
      src="{{ site.baseurl }}/assets/Madeline%20Mae%20Sliwinski%20Resume.pdf#view=fitH"
      title="Mae Sliwinski Resume"
      width="100%"
      height="800"
    ></iframe>
  </div>

</div>

<p>View my actual portfolio <a href="https://maesliwinski.com" target="_blank" rel="noopener noreferrer">here</a>.</p>