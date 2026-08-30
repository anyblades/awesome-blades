---
eleventyNavigation: { parent: More, key: CLI }
title: One CLI
description: https://github.com/buildawesome-one/kit/tree/main/cli
bricks:
  - path: https://raw.githubusercontent.com/buildawesome-one/kit/refs/heads/main/cli/README.md
    section: content
  - md: |-
      ---
      ## <sup style>Appendix</sup>
      How it works:
  - path: "https://raw.githubusercontent.com/buildawesome-one/kit/refs/heads/main/cli/package.json"
    wrap: ["```json\n", "\n```"]
---

### Find and kill 11ty processes

```sh
ps aux | grep eleventy
pkill -f eleventy
```

You can even combine it with other processes hanging around:

```sh
ps aux | grep -E 'eleventy|tailwind|.bin/serve'
pkill -f tailwind
pkill -f .bin/serve
```
