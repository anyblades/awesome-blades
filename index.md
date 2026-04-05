---
permalink: /
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
      # assign _ = '../node_modules/@anydigital/blades/README.md'
      assign _ = 'https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/README.md'
      echo _ | fetch | section: 'summary' | replace: 'hgroup>', 'h1>' | replace: '<wbr>', '<br>'
    %}
  site.brand: |-
    <p>
      <big style="vertical-align: middle">{{ site.brand }}</big> &nbsp;
      <img src="https://img.shields.io/github/v/release/anydigital/blades?label=&color=white&include_prereleases">&nbsp;
      <a href="https://github.com/anydigital/blades"><img src="https://img.shields.io/github/stars/anydigital/blades?label="></a>
    </p>
    <div style="width: 100%">{{ summary | markdownify }}</div>
includes:
  - section: docs
    path: https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/README.md
  - text: ---
  - path: README.md
    section: index
---
