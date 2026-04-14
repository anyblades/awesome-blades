---
eleventyNavigation:
  parent: css
  key: <i class="fa-solid fa-mobile-screen-button"></i> Table
  order: 4
title: <em>Re</em>sponsive table <sub>without wrapping container</sub>
eleventyComputed:
  summary: |-
    {{ 'https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/responsive-table.css'
     | if: site.prod | default: '../../blades/src/responsive-table.css' | fetch | section: 'summary' | markdownify }}

includes:
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/responsive-table.css
---
