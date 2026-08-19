---
title: Welcome!
hide:
  - navigation
  - toc
---

<style>
  /* 1. Nuke padding on parent layout elements */
  .md-main__inner,
  .md-content,
  .md-content__inner {
    margin-top: 0 !important;
    padding-top: 0 !important;
  }

  /* 2. Hide hidden sidebar wrappers that hold top vertical space */
  .md-sidebar {
    display: none !important;
  }

  /* 3. Pull hero flush against the top navigation bar */
  .hero-banner {
    margin: -2rem -0.8rem 2rem -0.8rem !important;
    padding: 5rem 1.5rem;
    text-align: center;
    color: #ffffff;
    background: 
      linear-gradient(rgba(5, 30, 57, 0.8), rgba(5, 30, 57, 0.9)),
      url("assets/images/stinger-complete.webp") center/cover no-repeat;
  }

  @media screen and (min-width: 60em) {
    .hero-banner {
      /* On desktop, pull up higher to counter the tab bar height offset */
      margin: -3.5rem -2.4rem 2.5rem -2.4rem !important;
      padding: 6rem 2rem;
    }
  }

  .hero-banner h1 {
    color: #ffffff !important;
    font-size: 2.2rem;
    margin-top: 0 !important;
    margin-bottom: 0.5rem;
    border: none !important;
  }

  .hero-banner p {
    color: #e2e8f0;
    font-size: 1.15rem;
    max-width: 700px;
    margin: 0 auto 1.75rem;
  }
</style>

<div class="hero-banner" markdown>

# Stinger Autonomous Marine Stack

Autonomous surface and underwater vehicle software, simulation testbeds, and hardware operational guides.

[Get Started](software/index.md){ .md-button .md-button--primary }
[View Architecture](software/index.md#software-stack-architecture){ .md-button }

</div>

![Stinger Complete](/stinger-guide/assets/images/stinger-complete.webp)

The build guide. This website is still under construction!

[Browse Tutorials :arrow_right:](tutorials/index.md){ .md-button .md-button--primary }
[View on GitHub](https://github.com/your-username/your-repo){ .md-button }

---

<div class="grid cards" markdown>

-   **Hardware**

    ---

    Detailed mechanical assembly steps with complete BOM lists, required tools, and torque specs.

-   **Wiring & Electronics**

    ---

    Clear schematics, pinout diagrams, and cable routing guides to protect sensitive electronics.

-   **Software Setup**

    ---

    First-boot scripts, container setup, and sensor integration checklists to get moving quickly.

</div>
