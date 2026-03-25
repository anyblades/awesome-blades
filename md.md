---
title: Markdown Tricks
canonical: https://blades.ninja/md/
---

## `markdown-it-attrs`

https://github.com/arve0/markdown-it-attrs

### Long-long link with many-many CSS classes, and still readable!

<!-- prettier-ignore-start -->
```md
[Suggest a Page<i class="fa-brands fa-github ml-1"></i>
](https://github.com/anydigital/awesome-tricks-for-geeks/new/main/tricks
){.text-slate-500 .font-light .decoration-dashed}
```

You can even add list item classes!

```md
- [Suggest a Page<i class="fa-brands fa-github ml-1"></i>
  ](https://github.com/anydigital/awesome-tricks-for-geeks/new/main/tricks
  ){.text-slate-500 .font-light .decoration-dashed} {.list-none}
```
<!-- prettier-ignore-end -->
