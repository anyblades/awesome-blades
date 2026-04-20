---
permalink: /
site:
  inline_styles:
    - |-
      h1 {
        margin-block-start: 0;
        @media (max-width: 767px) { font-size: 1.75em }
      }

      th, td {
        padding-inline: 1rem !important;
        &:first-child { padding-inline-end: 2rem !important }
        &:not(:first-child) { width: 16% }
        &:nth-last-child(2) { border-inline-start: 2px dotted silver }
      }
      .fa-tailwind-css  { color: deepskyblue }
      .fa-bootstrap     { color: blueviolet }
      td big { font-weight: bold }

      #showcase + article {
        padding-inline: 1.5rem;
        p {
          display: flex;
          flex-wrap: wrap;
          gap: 0.5rem 1.5rem;
          margin: 0;
          font-size: 125%;
          @media (min-width: 768px) { justify-content: center }
        }
        a { overflow: visible }
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

## Why *Bl*ades?

*Bl*ades does not replace other frameworks, but empowers them instead:

| <hr>                              | <i class="fa-brands fa-tailwind-css"></i> Tailwind <hr>             | <i class="fa-brands fa-bootstrap"></i> Bootstrap <hr> | Pico ✨ <hr>                            | 🥷 [*Bl*ades](/css/) <hr>                         | <small>Example 1:</small><br> [Pico+*Bl*ades](https://blades.ninja/css/pico/) <hr> | <small>Example 2:</small><br> [Tailwind+*Bl*ades](https://build.blades.ninja/) <hr> |
| --------------------------------- | ------------------------------------------------------------------- | ----------------------------------------------------- | --------------------------------------- | ------------------------------------------------- | ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Type                              | Utility-first                                                       | Component-based                                       | Class-light                             | Class-light                                       | Class-light                                                                        | Utility-first                                                                       |
| Sources                           | [JavaScript](https://github.com/tailwindlabs/tailwindcss)           | [SCSS](https://github.com/twbs/bootstrap)             | [SCSS](https://github.com/picocss/pico) | [Modern CSS](https://github.com/anyblades/blades) | [Modern CSS](https://github.com/anyblades/pico)                                    | Hybrid                                                                              |
| CSS base                          | `modern-normalize` <br> `preflight`                                 | `normalize` <br> `reboot`                             | `normalize` <br> `sanitize`             | _⇢ Inherited_                                     | `normalize` <br> `sanitize`                                                        | `modern-normalize` <br> `preflight`                                                 |
| <big>Layout</big>                 | ☑️ CSS primitives                                                   | ✅                                                    | ☑️ Basic grid                           | _⇢ Inherited_                                     | ☑️ Basic grid                                                                      | ☑️ CSS primitives                                                                   |
| Text columns                      | ☑️ CSS primitives                                                   | ❌                                                    | ❌                                      | ✅ [Docs](/css/#auto-columns)                     | ✅                                                                                 | ✅                                                                                  |
| Breakout layout                   | ❌                                                                  | ❌                                                    | ❌                                      | ✅ [Docs](/css/breakout/)                         | ✅                                                                                 | ✅                                                                                  |
| <big>Typography</big>             | ✅ [Plugin](https://github.com/tailwindlabs/tailwindcss-typography) | ✅                                                    | ✅                                      | _⇢ Inherited_                                     | ✅                                                                                 | ✅ Plugin                                                                           |
| Responsive tables without wrapper | ❌                                                                  | ❌                                                    | ❌                                      | ✅ [Docs](/css/responsive-table/)                 | ✅                                                                                 | ✅                                                                                  |
| <big>Forms</big>                  | ✅ [Plugin](https://github.com/tailwindlabs/tailwindcss-forms)      | ✅                                                    | ✅                                      | _⇢ Inherited_                                     | ✅                                                                                 | ✅ Plugin                                                                           |
| Float labels                      | ❌                                                                  | ✅                                                    | ❌                                      | ✅ [Docs](/css/float-label/)                      | ✅                                                                                 | ✅                                                                                  |

{.striped}

---
