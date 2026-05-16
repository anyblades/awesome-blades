### Render subnavigation (subpages)

Using https://www.11ty.dev/docs/plugins/navigation/#example-get-just-one-branch :

```jinja2
{% set _ = collections.all
  | eleventyNavigation(eleventyNavigation.key) %}{# child becomes parent here :) #}
{{ _ | eleventyNavigationToHtml }}
```



### Include and render `.md` file w/o its Front Matter

```jinja2 {data-caption=Nunjucks}
{# first, get the raw content using `html` as plain-text engine #}
{% set _eval = "{% renderFile './YOUR_FILE.md', {}, 'html' %}" %}
{% set _raw_md = _eval | renderContent('njk') %}

{# then, remove the front matter using regex, and render using `md` #}
{{ _raw_md | replace(r/^---[\s\S]*?---/, '') | renderContent('md') | safe }}
```

### Render content inline with global 11ty processors

```liquid {data-caption=Liquid}
{% capture _ %}
...
{% endcapture %}
{{ _ | markdownify | renderTransforms: page | replace: '...', '...' }}
```
