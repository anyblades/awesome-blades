---
permalink: /build-awesome-11ty/
eleventyNavigation:
  key: 11ty
  title: <i class="fa-brands fa-eleventy"></i>
  order: 2
title: <em>Eleventy Bl</em>ades
canonical: https://blades.ninja/build-awesome-11ty/
eleventyComputed:
  summary: |-
    {% liquid
      # assign _ = '../../eleventy-blades/README.md'
      assign _ = 'https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md'
      echo _ | fetch | section: 'summary' | markdownify
    %}
includes:
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/README.md
  - text: |-
      ---
      ## [Templating](/html/)

      {#njk-vscode}
      <!--https://bsky.app/profile/any.digital/post/3mdjvepwr7k2w-->
  - section: toc
    path: https://blades.ninja/html/
  - path: build-awesome-11ty/_tpl.md
  - text: ---
  - path: build-awesome-11ty/_starters.md
  - text: ---
  - section: index
    path: https://raw.githubusercontent.com/anydigital/awesome-11ty-build-awesome/refs/heads/master/README.md

revised: 2026-02-28
---
