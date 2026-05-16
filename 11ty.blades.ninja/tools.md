---
eleventyNavigation:
  key: Power-ups
  order: 3
title: <sup>Build Awesome</sup> Power <i class="fa-brands fa-eleventy"></i> tools <sub>by <a href="/"><em>Eleventy Bl</em>ades</a></sub>
includes:
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/eleventy.config.js
  - text: ---
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/do/README.md
  - text: ---
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/siteData.js
  - text: |-
      ---
      ## More
  - text: |-
      ### Find and kill <small>11ty processes</small>

      ```sh
      ps aux | grep eleventy
      pkill -f eleventy
      ```

      You can even combine it with other processes hanging around:

      ```sh
      ps aux | grep -E 'eleventy|tailwind|.bin/serve'
      pkill -f tailwind
      pkill -f .bin/serve
      ```
  - path: ./_forms.md
  - text: |-
      ---
      See also:
  - teaser: /
  - teaser: /starters/
---
