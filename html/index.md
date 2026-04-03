---
permalink: /html/
title: <sup>Nunjucks / Liquid</sup> HTML blades <sub>for 11ty/Build Awesome, Jekyll, etc.</sub>
summary: Nunjucks/Liquid batteries included (for 11ty/Build Awesome, Jekyll, etc.) 🥷
includes:
  - text: |-
      ---
      ## Base HTML {#base}
  - section: docs,code
    path: https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/_includes/blades/html.njk
  - section: docs,code
    path: https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/_includes/blades/html.liquid
  - text: |-
      ---
      ## Links
  - section: docs,code
    path: https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/_includes/blades/links.liquid
  - text: |-
      ---
      ## Sitemap 🆕
      https://github.com/anydigital/blades/blob/main/_includes/blades/sitemap.xml.njk
  - text: |-
      ---
      ## Google Tag Manager (GTM) {#gtm}
  - section: docs,code
    path: https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/_includes/blades/gtm.njk
  - section: docs,code
    path: https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/_includes/blades/gtm.liquid
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

```sh
npm install @anydigital/blades
cd ./_includes  # your includes dir
ln -s ../node_modules/@anydigital/blades/_includes/blades
```

That's it! Now you can use HTML blades in your templates like this:

<mark>In Nunjucks:</mark>

```jinja2
{% extends 'blades/html.njk' %}
{% include 'blades/gtm.njk' %}
```

<mark>In Liquid:</mark>

```liquid
{% include blades/html.liquid %}
{% include blades/gtm.liquid for_body=true %}
{% render blades/links, links: site.links, current_url: page.url %}
```
