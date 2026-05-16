---
permalink: /
eleventyNavigation:
  title: Plugin
  order: 0
title: <sup>Build Awesome</sup> <em>Eleventy Bl</em>ades <small>plugin</small>
canonical: https://11ty.blades.ninja/
eleventyComputed:
  summary: |-
    {{ 'https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md'
     | if: site.prod | default: '../../eleventy-blades/README.md' | fetch | section: 'summary' | markdownify }}

includes:
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md
    section: install
  - teaser: /starters/
    no_toc: true
  - text: |-
      ---
      ## Documentation
  - teaser: /filters/
  # - path: https://11ty.blades.ninja/filters/
  #   section: toc
  - teaser: /processors/
  # - path: https://11ty.blades.ninja/processors/
  #   section: toc
  - teaser: /tools/
  # - path: https://11ty.blades.ninja/tools/
  #   section: toc
  - text: |-
      ---
      ## Templating <small>tricks</small> {#tpl}
      <!-- https://github.com/anyblades/awesome-11ty-build-awesome#tutorials -->
      {#njk-vscode}
      <!-- https://bsky.app/profile/any.digital/post/3mdjvepwr7k2w -->
  - teaser: https://blades.ninja/html/
  - path: https://blades.ninja/html/
    section: toc
  - path: ./_tpl.md
  - text: |-
      ---
      ## More
  - teaser: /starters/
  - teaser: /awesome/
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md
    section: featured

revised: 2026-02-28
---
