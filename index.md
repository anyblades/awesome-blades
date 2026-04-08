---
permalink: /
eleventyNavigation:
  key: css
  title: CSS
  order: 0
site:
  inline_styles:
    - |-
      h1 {
        margin-top: 0.25em;
      }
      @media (max-width: 767px) {
        h1 {
          font-size: 1.75em;
          br { display: none }
        }
      }
eleventyComputed:
  summary: |-
    {% liquid
      #TODO to tricks
      # assign _ = '../node_modules/@anyblades/blades/README.md'
      assign _ = 'https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md'
      echo _ | fetch | section: 'summary' | replace: 'hgroup>', 'h1>' | replace: '<wbr>', '<br>'
    %}
  hero: "<br>{{ summary | markdownify }}<br>"
includes:
  - section: docs
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md
  - text: ---
  - path: README.md
    section: index
---
