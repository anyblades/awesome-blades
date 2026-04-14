---
eleventyNavigation:
  parent: css
  key: <i class="fa-solid fa-tv fa-flip-both"></i> Breakout
  order: 5
title: <em>Br</em>eakout elements
eleventyComputed:
  summary: |-
    {{ 'https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/breakout.css'
     | if: site.prod | default: '../../blades/src/breakout.css' | fetch | section: 'summary' | markdownify }}

includes:
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/src/breakout.css
---
