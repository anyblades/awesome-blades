---
eleventyNavigation:
  parent: More
  key: Starters
eleventyComputed:
  content_for_header: |-
    <meta property="og:image" content="{{ site.base }}{{ page.url }}og.png">
    <meta name="twitter:card" content="summary_large_image">
title: |-
  <sup style>Best minimal</sup>
  <i class="fa-brands fa-eleventy"></i><span hidden>11ty</span> / Build&nbsp;Awesome
  <mark>starters</mark>
  <sub style>as of August 2026</sub>
description: |-
  Eleventy ecosystem offers a [wide variety of starters](/awesome/#starters).

  Not sure where to begin? Start with a minimal template:
bricks:
  - content_here: "{{ content | replace('>https://github.com/', '>@') | safe }}"
revised: 2026-04-24
---

<!--section:micro-->
<style>
  table {
    a[href*="://github.com/"] > i { display: none }
    code { padding: 0.25em; font-size: max(50%, 0.5rem); vertical-align: middle }
  }
</style>

| Repo                                                                                                                                                                                            | Code size                                                                                                                 | Direct dependencies                                                  | Custom JS <hr>                                                | Custom templates <hr>                             | Custom CSS <hr>                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------------------------------------- |
| **_🌱_ Micro-starters:**                                                                                                                                                                        |                                                                                                                           |                                                                      |                                                               |                                                   |                                                                                 |
| [buildawesome-content-first](//content.build.blades.ninja/) <sub style>Best content-first micro-starter powered by Build Awesome Kit and Blades CSS</sub>                                       | <img src="https://img.shields.io/github/languages/code-size/anyblades/buildawesome-content-first?label=&color=green">     | 🌱 2 pkgs                                                            | 🌱 0                                                          | 🌱 3 files                                        | 🌱 0 files `2 lines`                                                            |
| [buildawesome-micro-starters](//micro.build.blades.ninja/) <sub style>Modern <big class="mark-brand">11-in-1</big> micro-starter showcasing Build Awesome Kit's all-in-one config package</sub> | <img src="https://img.shields.io/github/languages/code-size/anyblades/buildawesome-micro-starters?label=&color=green">    | 🌱 2 pkgs <sub style>+1 pkg if Shotpipe<br>+3 pkgs if Tailwind</sub> | 🌱 0 <sub style>1 file if Shotpipe</sub>                      | 🌱 2 files <sub style>or less (per starter)</sub> | 🌱 0 files `~10 lines` <sub style>1 file if Tailwind</sub> <!--section:BREAK--> |
| **_🌳_ Other minimal starters:**                                                                                                                                                                |                                                                                                                           |                                                                      |                                                               |                                                   |                                                                                 |
| https://github.com/danurbanowicz/eleventy-netlify-boilerplate <sub style>A template for building a blog with the Eleventy static site generator and Decap CMS</sub>                             | <img src="https://img.shields.io/github/languages/code-size/danurbanowicz/eleventy-netlify-boilerplate?label=">           | ♻️ 7 pkgs                                                            | 5-10 files                                                    | 10-20 files                                       | ♻️ 1 file `~200 lines`                                                          |
| https://github.com/11ty/eleventy-base-blog <sub style>A starter repository for a blog web site using the Eleventy static site generator</sub>                                                   | <img src="https://img.shields.io/github/languages/code-size/11ty/eleventy-base-blog?label=">                              | 10 pkgs                                                              | 5-10 files                                                    | 5-10 files                                        | ♻️ 3 files `~300 lines`                                                         |
| https://github.com/mwdelaney/zeropoint <sub style>A modern, opinionated, bare-bones website starter that gets you "up to zero"</sub>                                                            | <img src="https://img.shields.io/github/languages/code-size/MWDelaney/zeropoint?label=">                                  | 10-20 pkgs                                                           | 10-20 files                                                   | 10 files                                          | ♻️ 3 files `~200 lines` <sub style>`⚠️ .scss`</sub>                             |
| **_⚠️_ Not so minimal starters:**                                                                                                                                                               |                                                                                                                           |                                                                      |                                                               |                                                   |                                                                                 |
| https://github.com/ttntm/11ty-landing-page                                                                                                                                                      | <img src="https://img.shields.io/github/languages/code-size/ttntm/11ty-landing-page?label=">                              | ♻️ 7 pkgs                                                            | 4 files <sub style>`⚠️ tailwind.config.cjs ~1000 lines`</sub> | 10-20 files                                       | ♻️ 4 files                                                                      |
| https://github.com/matthiasott/eleventy-plus-vite                                                                                                                                               | <img src="https://img.shields.io/github/languages/code-size/matthiasott/eleventy-plus-vite?label=">                       | ⚠️ 20+ pkgs                                                          | 5-10 files                                                    | 10-20 files                                       | ⚠️ 20+ files                                                                    |
| https://github.com/nhoizey/pack11ty                                                                                                                                                             | <img src="https://img.shields.io/github/languages/code-size/nhoizey/pack11ty?label=">                                     | 10-20 pkgs                                                           | 10-20 files                                                   | 10-20 files                                       | ⚠️ 30+ files                                                                    |
| https://github.com/adamstddrd/grease                                                                                                                                                            | <img src="https://img.shields.io/github/languages/code-size/adamstddrd/grease?label=&color=yellow">                       | ♻️ 4 pkgs                                                            | 10-20 files                                                   | 10-20 files                                       | ⚠️ 20+ files                                                                    |
| https://github.com/madrilene/eleventy-excellent                                                                                                                                                 | <img src="https://img.shields.io/github/languages/code-size/madrilene/eleventy-excellent?label=&color=yellow">            | ⚠️ 40+ pkgs                                                          | ⚠️ 30+ files                                                  | ⚠️ 40+ files                                      | ⚠️ 40+ files                                                                    |
| https://github.com/scottsweb/elva                                                                                                                                                               | <img src="https://img.shields.io/github/languages/code-size/scottsweb/elva?label=&color=yellow">                          | ⚠️ 20+ pkgs                                                          | ⚠️ 30+ files                                                  | ⚠️ 20+ files                                      | 5-10 files                                                                      |
| https://github.com/rothsandro/eleventy-notes                                                                                                                                                    | <img src="https://img.shields.io/github/languages/code-size/rothsandro/eleventy-notes?label=&color=orange">               | 10-20 pkgs                                                           | ⚠️ 50+ files                                                  | 10-20 files                                       | ⚠️ 30+ files                                                                    |
| https://github.com/googlechrome/starter-extended-blog                                                                                                                                           | <img src="https://img.shields.io/github/languages/code-size/googlechrome/starter-extended-blog?label=&color=orange">      | ⚠️ 20+ pkgs                                                          | ⚠️ 50+ files                                                  | 10-20 files                                       | ♻️ 4 files                                                                      |
| **_📦_ Outdated starters:** {#outdated}                                                                                                                                                         |                                                                                                                           |                                                                      |                                                               |                                                   |                                                                                 |
| https://github.com/5t3ph/11ty-sass-skeleton `⚠️ 11ty v2`                                                                                                                                        | <img src="https://img.shields.io/github/languages/code-size/5t3ph/11ty-sass-skeleton?label=&color=green" >                |
| https://github.com/surjithctly/neat-starter `⚠️ 11ty v1`                                                                                                                                        | <img src="https://img.shields.io/github/languages/code-size/surjithctly/neat-starter?label=" >                            |
| https://github.com/ixartz/eleventy-starter-boilerplate `⚠️ 11ty v0`                                                                                                                             | <img src="https://img.shields.io/github/languages/code-size/ixartz/eleventy-starter-boilerplate?label=">                  |
| https://github.com/daflh/vredeburg `⚠️ 11ty v2`                                                                                                                                                 | <img src="https://img.shields.io/github/languages/code-size/daflh/vredeburg?label=" >                                     |
| https://github.com/5t3ph/11ty-netlify-jumpstart `⚠️ 11ty v2`                                                                                                                                    | <img src="https://img.shields.io/github/languages/code-size/5t3ph/11ty-netlify-jumpstart?label=">                         |
| https://github.com/yinkakun/eleventy-duo `⚠️ 11ty v2`                                                                                                                                           | <img src="https://img.shields.io/github/languages/code-size/yinkakun/eleventy-duo?label=">                                |
| https://github.com/tryghost/eleventy-starter-ghost `⚠️ 11ty v0`                                                                                                                                 | <img src="https://img.shields.io/github/languages/code-size/tryghost/eleventy-starter-ghost?label=">                      |
| https://github.com/11ta/11ta-template `⚠️ 11ty v2`                                                                                                                                              | <img src="https://img.shields.io/github/languages/code-size/11ta/11ta-template?label=&color=yellow">                      |
| https://github.com/google/eleventy-high-performance-blog `⚠️ 11ty v2`                                                                                                                           | <img src="https://img.shields.io/github/languages/code-size/google/eleventy-high-performance-blog?label=&color=yellow">   |
| https://github.com/oak-harbor-kits/starter-kit-v4-eleventy `⚠️ 11ty v1`                                                                                                                         | <img src="https://img.shields.io/github/languages/code-size/oak-harbor-kits/starter-kit-v4-eleventy?label=&color=orange"> |

{.striped}

<style>
  td:first-child strong > em {
    float: left; margin-left: -2ch; font-style: normal;
  }
  tr:has(#outdated) {
    &, & ~ tr {
      opacity: 50%;
      &:hover { opacity: 100% }
    }
  }
</style>

---

## <sup style>Featured by</sup>

- [@thefulcrum](https://bsky.app/profile/thefulcrum.eurosky.social/post/3mnk64fhwpq2l)
