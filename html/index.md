---
permalink: /html/
eleventyNavigation:
  key: <i class="fa-solid fa-code"></i>
  order: 1
title: <em>Bl</em>ades &nbsp;<small>HTML templates</small>
summary: Nunjucks/Liquid batteries included (for 11ty/Build Awesome, Jekyll, etc.) 🥷
includes:
  - section: install-preconf
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/README.md
  - text: |-
      ---
      ## Base HTML {#base}
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/_includes/blades/html.njk
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/_includes/blades/html.liquid
  - text: |-
      ---
      ## Links
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/_includes/blades/links.liquid
  - text: |-
      ---
      ## Sitemap 🆕
      https://github.com/anyblades/blades/blob/main/_includes/blades/sitemap.xml.njk
  - text: |-
      ---
      ## Google Tag Manager (GTM) {#gtm}
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/_includes/blades/gtm.njk
  - section: docs,code
    path: https://raw.githubusercontent.com/anyblades/blades/refs/heads/main/_includes/blades/gtm.liquid
  - text: ---
  - path: html/_njk.md
  - text: ---
  - path: html/_liquid.md
  - text: |-
      ---
      - Featured by:
        - https://11tybundle.dev/blog/11ty-bundle-83/
        - https://11tybundle.dev/categories/nunjucks-macros/
        - https://github.com/anydigital/awesome-11ty-build-awesome
      - See also:
        - https://buildexcellentwebsit.es/
        - https://blog.jim-nielsen.com/2025/lots-of-little-html-pages/

      {.unlist .columns}
---

## Install

<mark>Via npm:</mark>

```sh
npm install @anyblades/blades
cd ./_includes  # your includes dir
ln -s ../node_modules/@anyblades/blades/_includes/blades
```

That's it! Now you can use HTML blades in your templates like this:

```jinja2 {data-caption=Nunjucks}
{% extends 'blades/html.njk' %}
{% include 'blades/gtm.njk' %}
```

```liquid {data-caption=Liquid}
{% include blades/html.liquid %}
{% include blades/gtm.liquid for_body=true %}
{% render blades/links, links: site.links, current_url: page.url %}
```
