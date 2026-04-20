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
      th, td {
        padding-inline: 1rem !important;

        &:last-child {
          border-inline-start: 2px dotted silver;
        }
      }
      th code {
        padding: 0;
        background: none;
        font-weight: lighter;
      }
      .fa-tailwind-css { color: deepskyblue }
      .fa-bootstrap    { color: blueviolet }
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

## How it works <small>with other frameworks:</small>

|               | <i class="fa-brands fa-tailwind-css"></i> Tailwind                   | <i class="fa-brands fa-bootstrap"></i> Bootstrap | Pico ✨                                 | 🥷 *Bl*ades <hr>                                  | <small>Example:</small><br> Pico`+`*Bl*ades ✨🥷 <hr> |
| ------------- | -------------------------------------------------------------------- | ------------------------------------------------ | --------------------------------------- | ------------------------------------------------- | ----------------------------------------------------- |
| Type:         | Utility-first                                                        | Component-based                                  | Class-light                             | Class-light                                       | Class-light                                           |
| Written in:   | [JavaScript](https://github.com/tailwindlabs/tailwindcss-typography) | [SCSS](https://github.com/twbs/bootstrap)        | [SCSS](https://github.com/picocss/pico) | [Modern CSS](https://github.com/anyblades/blades) | [Modern CSS](https://github.com/anyblades/pico)       |
| CSS base:     | `modern-normalize` <br> `preflight`                                  | `normalize` <br> `reboot`                        | `normalize` <br> `sanitize`             | _⇢ inherits_                                      | `normalize` <br> `sanitize`                           |
| Typography:   | ✅ [Plugin](https://tailwindcss-typography.vercel.app/)              | ✅                                               | ✅                                      | _⇢ inherits_                                      | ✅                                                    |
| Float labels: | ❌                                                                   | ✅                                               | ❌                                      | ✅ [Docs](https://blades.ninja/css/float-label/)  | ✅                                                    |

{.striped}

---
