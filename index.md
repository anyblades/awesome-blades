---
permalink: /
site:
  inline_styles:
    - |-
      h1 {
        margin-block-start: 0;

        @media (max-width: 767px) {
          font-size: 1.75em;
        }
      }
eleventyComputed:
  summary: |-
    {% liquid
      #TODO to tricks
      # assign _ = '../node_modules/@anyblades/blades/README.md'
      assign _ = 'https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md'
      echo _ | fetch | section: 'summary' | replace: 'hgroup>', 'h1>' | replace: '<wbr>', '<br>' | markdownify
    %}
  hero: "<br>{{ summary }}<br>"
includes:
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md
  - text: ---
  - path: README.md
    section: index
---
