---
title: Random <small>tricks</small>
canonical: https://blades.ninja/random/
---

## Terminal

### Find all symlinks 

```sh
find . -type l -ls

# excluding folder:
find . -not -path '*/node_modules/*' -type l -ls
```

### Check HTTP headers with `curl`

```sh
curl --head HTTP_URL

# or simply:
curl -I HTTP_URL
```

The `-I` flag (shorthand for `--head`) fetches only the HTTP headers from a server. This is the fastest way to inspect status codes, content types, and server metadata without downloading the actual page content.

---

## Regular Expressions {#regex}

Find all lines ending with `**`:

```
\*\*$\n
```

---

## JS

### Delete all HTML elements by class in pure JS

```js
document.getElementsByClassName('...').forEach(function(el){ el.parentElement.removeChild(el) })
```

---

## Ruby

Run Ruby projects locally on macOS without breaking system's Ruby:

### Install `rbenv` {#rbenv}

Assuming you already have Homebrew:

```sh
brew install rbenv

# Then list available Ruby versions, and install one:
rbenv install -l
rbenv install 3.2.10

# Set it for current project/folder:
rbenv local 3.2.10
```

Finally, add it to your shell's configuration file so it executes automatically:

```{data-caption=~/.zshrc}
eval "$(rbenv init -)"
```

### [GitHub Pages' Jekyll locally](/jekyll/)

### Slate Docs locally

Assuming you already [installed `rbenv`](#rbenv):

```sh
bundle install
bundle exec middleman build
```

> For the official version of Slate (v2.13.1), the best and most stable Ruby version is Ruby 3.1.
> While older documentation mentions Ruby 2.6 or 2.7, Slate officially dropped support for Ruby 2.5 and added formal support for Ruby 3.1 in its 2022 releases. Newer versions of Ruby (3.2+) can sometimes cause dependency conflicts with Slate's core engine, middleman, specifically regarding the nokogiri gem.

More info: https://github.com/slatedocs/slate/wiki/Using-Slate-Natively#installing-dependencies-on-macos
