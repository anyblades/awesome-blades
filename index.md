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
        min-width: 10ch;
        &:first-child { padding-inline-end: 2rem !important }
        &:not(:first-child) { width: 16% }
      }
      .fa-tailwind-css  { color: deepskyblue }
      .fa-bootstrap     { color: blueviolet }
      th code { padding: 0; background: none; font-weight: lighter }
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

|                                   | <i class="fa-brands fa-tailwind-css"></i> Tailwind                                         | 🥷 *Bl*ades                                       | <i class="fa-brands fa-tailwind-css"></i> Tailwind <br> `+` 🥷 *Bl*ades | Pico ✨                                 | Pico ✨ <br>`+` 🥷 *Bl*ades                     | <i class="fa-brands fa-bootstrap"></i> Bootstrap |
| --------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------------------------- | ----------------------------------------------------------------------- | --------------------------------------- | ----------------------------------------------- | ------------------------------------------------ |
| Demo                              | [tailwindcss-typography.vercel.app/typography](https://tailwindcss-typography.vercel.app/) | https://blades.ninja/css/                         | https://build.blades.ninja/                                             | https://picocss.com/                    | https://blades.ninja/css/pico/                  | https://getbootstrap.com/                        |
| Type                              | Utility-first                                                                              | Class-light                                       | Utility-first                                                           | Class-light                             | Class-light                                     | Component-based                                  |
| Sources                           | [JavaScript](https://github.com/tailwindlabs/tailwindcss)                                  | [Modern CSS](https://github.com/anyblades/blades) | Hybrid                                                                  | [SCSS](https://github.com/picocss/pico) | [Modern CSS](https://github.com/anyblades/pico) | [SCSS](https://github.com/twbs/bootstrap)        |
| CSS base                          | `modern-normalize` <br> `preflight`                                                        | ⇢ Inherited                                       | `modern-normalize` <br> `preflight`                                     | `normalize` <br> `sanitize`             | `normalize` <br> `sanitize`                     | `normalize` <br> `reboot`                        |
| <big>Layout</big>                 | ☑️ CSS primitives                                                                          | ⇢ Inherited                                       | ☑️ CSS primitives                                                       | ☑️ Basic grid                           | ☑️ Basic grid                                   | ✅                                               |
| Text columns                      | ☑️ CSS primitives                                                                          | ✅ [Docs](/css/#auto-columns)                     | ✅                                                                      | ❌                                      | ✅                                              | ❌                                               |
| Breakout layout                   | ❌                                                                                         | ✅ [Docs](/css/breakout/)                         | ✅                                                                      | ❌                                      | ✅                                              | ❌                                               |
| <big>Typography</big>             | ✅ [Plugin](https://github.com/tailwindlabs/tailwindcss-typography)                        | ⇢ Inherited                                       | ✅ Plugin                                                               | ✅                                      | ✅                                              | ✅                                               |
| Responsive tables without wrapper | ❌                                                                                         | ✅ [Docs](/css/responsive-table/)                 | ✅                                                                      | ❌                                      | ✅                                              | ❌                                               |
| <big>Forms</big>                  | ✅ [Plugin](https://github.com/tailwindlabs/tailwindcss-forms)                             | ⇢ Inherited                                       | ✅ Plugin                                                               | ✅                                      | ✅                                              | ✅                                               |
| Float labels                      | ❌                                                                                         | ✅ [Docs](/css/float-label/)                      | ✅                                                                      | ❌                                      | ✅                                              | ✅                                               |

{.striped}

---
