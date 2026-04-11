---
permalink: /css/
eleventyNavigation:
  parent: css
  key: Docs
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
  - text: "### Breakout elements → {href=/css/breakout/}"
  - section: summary
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/breakout.css
  - text: "[Demo & Docs →](/css/breakout/){role=button .outline}"
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_layout.css
  - text: |-
      ---
      ## Content
  - section: docs-intro
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_typography.css
  - section: docs-intro
  - text: "### Link [fav]icons → {href=/css/link-icon/}"
  - section: summary
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/link-icon.css
  - text: "[Demo & Docs →](/css/link-icon/){role=button .outline}"
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_typography.css
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_code.css
  - text: |-
      ---
      ## Table
      ### Responsive table without wrapper → {href=/css/responsive-table/}
  - section: summary
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/responsive-table.css
  - text: "[Demo & Docs →](/css/responsive-table/){role=button .outline}"
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/_table.css
  - text: |-
      ---
      ## Forms
      ### Float label without CSS classes → {href=/css/float-label/}
  - section: summary
    path: https://raw.githubusercontent.com/anyblades/float-label-css/refs/heads/master/README.md
  - text: "[Demo & Docs →](/css/float-label/){role=button .outline}"
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
