---
permalink: /jekyll/
title: Jekyll <small>blades</small>
includes:
  - section: jekyll
    path: https://raw.githubusercontent.com/anydigital/blades/refs/heads/main/README.md
  - text: |-
      ---
      ### GitHub Pages' Jekyll locally

      Assuming you already [installed `rbenv`](/random/#rbenv):

      1.  ```rb {data-caption=Gemfile}
          source "https://rubygems.org"

          gem "github-pages", group: :jekyll_plugins
          ```

      2.  ```sh
          bundle install
          bundle exec jekyll serve
          ```

      Living example: https://github.com/anydigital/bladeswitch/blob/main/Gemfile

      More info: https://github.com/github/pages-gem#usage, https://jekyllrb.com/docs/installation/macos/
---
