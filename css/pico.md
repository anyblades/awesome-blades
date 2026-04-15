---
eleventyNavigation:
  key: <i>✨</i>
  order: 1
title: Pico CSS ✨
eleventyComputed:
  summary: |-
    {{ 'https://raw.githubusercontent.com/anyblades/pico/refs/heads/main/README.md'
     | if: site.prod | default: '../../pico/README.md' | fetch | section: 'summary' | markdownify }}

includes:
  - path: https://raw.githubusercontent.com/anyblades/pico/refs/heads/main/README.md
    section: docs
---
