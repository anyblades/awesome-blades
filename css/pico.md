---
eleventyNavigation:
  parent: css
  key: Pico <i>✨</i>
  order: 12
title: <em>Pi</em>co <small>CSS ✨</small> <sup><img src="https://img.shields.io/github/v/release/anyblades/pico?label=&color=black&include_prereleases"></sup>
eleventyComputed:
  summary: |-
    {{ 'https://raw.githubusercontent.com/anyblades/pico/refs/heads/main/README.md'
     | if: site.prod | default: '../../pico/README.md' | fetch | section: 'summary' | markdownify }}

includes:
  - section: intro
    path: https://raw.githubusercontent.com/anyblades/pico/refs/heads/main/README.md
    # path: ../../pico/README.md
  - section: toc
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/pico/refs/heads/main/README.md
    # path: ../../pico/README.md
---
