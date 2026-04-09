---
eleventyNavigation:
  parent: 11ty
  title: Power <i class="fa-solid fa-shuttle-space fa-rotate-270"></i> Tools
  order: 3
title: <a href="/build-awesome-11ty/"><sup>Build Awesome /</sup> Eleventy</a> Power Tools
includes:
  - text: |-
      ### Blades starters {#starters}
      <nav class="grid">

      ##### [🥷 Build Awesome Starter ↗ <br><small>11ty + Tailwind + Typography + Blades</small>](https://github.com/anyblades/build-awesome-starter){role=button .outline}
      ##### [🥷 Bladeswitch Starter ↗ <br><small>Jekyll + Pico + Blades</small>](https://github.com/anyblades/bladeswitch){role=button .outline}
      </nav>

      ---
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/eleventy.config.js
  - text: ---
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/do/README.md
  - text: ---
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/siteData.js
  - text: |-
      ---
      ### Appendix
      #### Find and kill <small>11ty processes</small>

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
---
