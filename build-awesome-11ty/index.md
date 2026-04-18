---
permalink: /build-awesome-11ty/
eleventyNavigation:
  key: 11ty
  title: <i class="fa-brands fa-eleventy"></i>
  order: 3
title: <sup>Build Awesome</sup> <em>Eleventy Bl</em>ades <small>plugin</small>
canonical: https://blades.ninja/build-awesome-11ty/
eleventyComputed:
  summary: |-
    {{ 'https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md'
     | if: site.prod | default: '../../eleventy-blades/README.md' | fetch | section: 'summary' | markdownify }}

includes:
  - text: |-
      ## Install
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md
    section: install
  - teaser: /build-awesome-11ty/starters/
    no_toc: true
  - text: |-
      ---
      ## Documentation
  - teaser: /build-awesome-11ty/filters/
  - path: https://blades.ninja/build-awesome-11ty/filters/
    section: toc
  - teaser: /build-awesome-11ty/processors/
  - path: https://blades.ninja/build-awesome-11ty/processors/
    section: toc
  - teaser: /build-awesome-11ty/tools/
  - path: https://blades.ninja/build-awesome-11ty/tools/
    section: toc
  - text: |-
      ---
      ## Templating <small>tricks</small>
      {#njk-vscode}
      <!-- https://bsky.app/profile/any.digital/post/3mdjvepwr7k2w -->
  - teaser: /html/
  - path: https://blades.ninja/html/
    section: toc
  - path: build-awesome-11ty/_tpl.md
  - text: |-
      ---
      ## More
  - teaser: /build-awesome-11ty/starters/
  - teaser: /build-awesome-11ty/awesome/
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md
    section: featured

revised: 2026-02-28
---
