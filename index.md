---
layout: default
title: Mae Sliwinski – Portfolio
---

<style>
  /* Hide the default blue header / GitHub profile block */
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

  .page-content {
    margin-left: 0 !important;
  }

  /* Home page title screen */
  .home-shell {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 2.5rem;
    text-align: center;
  }

  .home-title {
    font-family: "Agrandir", system-ui, -apple-system, BlinkMacSystemFont,
      "Segoe UI", sans-serif;
    font-size: clamp(3rem, 6vw, 4.5rem);
    margin: 0;
  }

  .pill-links {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    width: 100%;
    max-width: 580px;
  }

  .pill-link {
    display: block;
    padding: 1.1rem 1.8rem;
    border-radius: 999px;
    text-align: center;
    font-size: 1.15rem;
    text-decoration: none;
    color: #000;
    border: 2px solid transparent;
    box-shadow: 0 6px 14px rgba(0, 0, 0, 0.04);
    transition: transform 0.12s ease, box-shadow 0.12s ease,
      background-color 0.12s ease, border-color 0.12s ease;
  }

  .pill-link--about {
    background-color: #d6dfcc; /* green */
  }

  .pill-link--projects {
    background-color: #babbdd; /* purple */
  }

  .pill-link--cv {
    background-color: #a6cff5; /* blue */
  }

  .pill-link:hover {
    transform: translateY(-2px);
    box-shadow: 0 10px 22px rgba(0, 0, 0, 0.08);
    border-color: rgba(0, 0, 0, 0.1);
  }

  @media (max-width: 640px) {
    .wrapper {
      padding-inline: 1.2rem;
    }

    .home-shell {
      justify-content: flex-start;
      padding-top: 3.5rem;
      padding-bottom: 3rem;
    }
  }

  .home-portfolio-link {
  margin-top: 1.75rem;      /* space under the blue pill */
  text-align: center;
  font-size: 1rem;
}

.home-portfolio-link a {
  text-decoration: underline;
}

</style>

<div class="home-shell">
  <h1 class="home-title">Mae Sliwinski</h1>

  <div class="pill-links">
    <a class="pill-link pill-link--about" href="{{ site.baseurl }}/about/">
      About Me
    </a>

    <a class="pill-link pill-link--projects" href="{{ site.baseurl }}/projects/">
      Projects
    </a>

    <a class="pill-link pill-link--cv" href="{{ site.baseurl }}/cv/">
      CV
    </a>
  </div>

  <!-- NEW centered bold link directly under the blue pill -->
  <p class="home-portfolio-link">
    <strong>
      View my actual portfolio
      <a href="https://maesliwinski.github.io" target="_blank" rel="noopener noreferrer">
        here
      </a>.
    </strong>
  </p>
</div>

