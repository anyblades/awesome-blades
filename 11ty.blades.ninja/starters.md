---
eleventyNavigation:
  parent: Get started
  key: Minimal 11ty starters
  order: 11
content_for_header: |-
  <style>
    td code { padding: 0.25em }
    td > code { font-size: x-small; vertical-align: middle }
  </style>
revised: 2026-04-24
=== CONTENT: ===
title: Best minimal <i class="fa-brands fa-eleventy"></i> starters <sub>as of May 2026</sub>
description: |-
  Eleventy ecosystem offers a [wide variety of starters](/awesome/#more-starters).

  Not sure where to begin? Start with a minimal template:
bricks:
  - path: ./_starters.md
  - md: ---
---

How to Build Awesome
minimal yet long-living <i class="fa-brands fa-eleventy"></i> starter
that support continuous updates and evolve with your project?

Let's try to make a shift from a commodity (a template) to a service (long-term stability), and solve the "maintenance trap" where developers spend more time fixing their build tools than writing content.

## The problem <small>of "maintenance trap"</small>

Why traditional starters might fail? Once a user clones a repo, they are "orphaned" from the original source. If a security patch or a new 11ty version comes out, the user has to manually port those changes into their "off-road", customized codebase.

## The solution

For a starter to evolve, it must be "pluggable" — allowing users to toggle/override features without touching the core reusable code.

First of all, let's separate all 11ty-specific yet generic enough components into separate 11ty plugin, so it can be highly reused across many different sites and even starters:

This way your generic [11ty config](/tools/#base-config), [filters](/filters/), shortcodes, [transforms](/processors/), and even [npm scripts](/tools/#base-scripts) live in a separate npm package.

So that the user’s project directory stays clean. Updating the "starter" is as simple as running npm update.

Same for generic "utility" templates, which can be potentially shared even outside of 11ty ecosystem:
