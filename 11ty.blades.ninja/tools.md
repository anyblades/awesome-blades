---
eleventyNavigation:
  key: Power-ups
  order: 3

bricks:
  - sections: [docs, code]
    path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/packages/eleventy-blades-base/eleventy.config.js
  - md: ---
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/do/README.md
  - md: ---
  - sections: [docs, code]
    path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/siteData.js
  - md: |-
      ---
      ## More
  - md: |-
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
  # - md: |-
  #     ---
  #     See also:
  # - teaser: /
  # - teaser: /starters/
---
