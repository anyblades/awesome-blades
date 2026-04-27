---
eleventyNavigation:
  parent: 11ty
  key: Starters
  order: 4
title: |-
  <sup>How to Build Awesome</sup>
  Minimal yet long-living <i class="fa-brands fa-eleventy"></i> starters
  <sub>that support continuous updates and evolve with your project<br class="opt">
  based on <a href="/build-awesome-11ty/"><em>Eleventy Bl</em>ades plugin</a></sub>
summary: Let's try to make a shift from a commodity (a template) to a service (long-term stability), and solve the "maintenance trap" where developers spend more time fixing their build tools than writing content.
site:
  inline_styles:
    - ".columns > * { break-inside: auto }"

includes:
  - teaser: /build-awesome-11ty/
  - text: |-
      This way your generic [11ty config](/build-awesome-11ty/tools/#base-config), [filters](/build-awesome-11ty/filters/), shortcodes, [transforms](/build-awesome-11ty/processors/), and even [npm scripts](/build-awesome-11ty/tools/#base-scripts) live in a separate npm package.

      So that the user’s project directory stays clean. Updating the "starter" is as simple as running npm update.

      Same for generic "utility" templates, which can be potentially shared even outside of 11ty ecosystem:
  - teaser: /html/
  - text: |-
      ---
      ## Living examples
  - path: https://raw.githubusercontent.com/anyblades/build-awesome-starter/refs/heads/main/README.md
  - text: ---
  - path: https://raw.githubusercontent.com/anyblades/bladeswitch/refs/heads/main/README.md
  - text: |-
      ---
      ### Minform <small>starter</small>

      A very minimalist approach to adding in forms templating to a website starter template that supports markdown.

      https://github.com/johnheenan/minform
  - text: ---
  - path: build-awesome-11ty/_starters.md

revised: 2026-04-24
---

## The problem <small>of "maintenance trap"</small>

Why traditional starters might fail? Once a user clones a repo, they are "orphaned" from the original source. If a security patch or a new 11ty version comes out, the user has to manually port those changes into their "off-road", customized codebase.

## The solution

For a starter to evolve, it must be "pluggable" — allowing users to toggle/override features without touching the core reusable code.

First of all, let's separate all 11ty-specific yet generic enough components into separate 11ty plugin, so it can be highly reused across many different sites and even starters:
