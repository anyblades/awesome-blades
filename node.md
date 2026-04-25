---
title: Node.js <small>nvm, npm tricks</small>
canonical: http://blades.ninja/node/

includes:
  - path: https://raw.githubusercontent.com/anyblades/eleventy-blades/refs/heads/main/src/do/README.md
---

## `nvm`

Install: https://github.com/nvm-sh/nvm#install--update-script

| Command <hr class="x2">               | Action                                                                                                                     |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| <kbd>nvm ls</kbd>                     | see the Node.js versions you have installed via nvm                                                                        |
| <kbd>nvm install --lts</kbd>          | install LTS version (Long Term Support) — recommended for most users and production environments because it is more stable |
| <kbd>nvm alias default 'lts/\*'</kbd> | set the LTS (Long Term Support) version as your global default so it persists across new terminal sessions                 |

## `npm`

### `npm link` auto-completion with @namespaces support

`~/.zshrc`:

```
# Initialize zsh completion system
autoload -Uz compinit
compinit

# Enable npm link completion for scoped packages
_npm_link_completion() {
  local -a pkgs
  pkgs=($(
    {
      find -L "$(npm root -g)" -mindepth 1 -maxdepth 1 -type d ! -name "@*"; \
      find -L "$(npm root -g)/@"* -mindepth 1 -maxdepth 1 -type d; \
    } | sed "s|$(npm root -g)/||"
  ))
  _describe 'npm packages' pkgs
}

# Enable completion for 'npm link'
compdef _npm_link_completion npm link
```

### Install local package with its dependencies

```sh
npm i <local-path> --install-links
```

---

See also:

- https://blades.ninja/jsdelivr/#purge-cache
