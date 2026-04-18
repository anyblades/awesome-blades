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
      #showcase + article {
        padding-inline: 1.5rem;

        p {
          display: flex;
          flex-wrap: wrap;
          gap: 0.5rem 1.5rem;
          margin: 0;
          font-size: 125%;

          @media (min-width: 768px) {
            justify-content: center;
          }
        }
        a {
          overflow: visible;
        }
      }
eleventyComputed:
  #TODO: add to tricks
  summary: |-
    {{ 'https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md'
     | if: site.prod | default: '../../blades/README.md' | fetch | section: 'summary' | replace: 'hgroup>', 'h1>' | replace: '<wbr>', '<br>' | markdownify }}
  hero: "<br>{{ summary }}<br>"

includes:
  - text: |-
      ## [Documentation <i><small>→</small></i>](/css/)
  - path: https://blades.ninja/css/
    section: toc
  - path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md
    section: info
  - text: ---
  - path: README.md
    section: tricks
---
