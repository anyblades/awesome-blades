---
permalink: /css/
eleventyNavigation:
  key: css
  title: CSS
  order: 0
title: <em>Bl</em>ades <small>CSS</small>
eleventyComputed:
  summary: |-
    {% liquid
      # assign _ = '../node_modules/@anyblades/blades/README.md'
      assign _ = 'https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md'
      echo _ | fetch | section: 'summary' | strip_tag: 'big' | markdownify
    %}
includes:
  - text: "## Install"
  - section: install
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md
  - section: code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/blades.theme.css
  - text: |-
      ---
      ## Layout
  - section: docs-intro
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_layout.css
  - teaser: /css/breakout/
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_layout.css
  - text: |-
      ---
      ## Content
  - section: docs-intro
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/content/_typography.css
  - section: docs-intro
  - teaser: /css/link-icon/
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/content/_typography.css
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/content/_code.css
  - text: |-
      ---
      ## Table
  - teaser: /css/responsive-table/
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/content/_table.css
  - text: |-
      ---
      ## Forms
  - teaser: /css/float-label/
  - text: |-
      ---
      ## Utilities
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_utilities.css
  - text: |-
      ---
      See also:
      - https://buildexcellentwebsit.es/
      - https://github.com/picocss/pico
      - https://github.com/kevquirk/simple.css
      - https://github.com/dbohdan/classless-css
      - https://github.com/dohliam/dropin-minimal-css
      - https://github.com/troxler/awesome-css-frameworks
      - https://kittygiraudel.com/2026/03/21/heading-anchors-with-11ty/
      - https://micah.torcellini.org/2026/03/17/simple-timeline/
      - https://blog.frankmtaylor.com/2026/03/05/you-dont-know-html-tables/

      {.columns}
---
