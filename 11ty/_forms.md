### Forms

#### Minform starter

<blockquote>

Minform v0.3.1 released at https://github.com/johnheenan/minform which will work with formsubmit.io above to convert forms to email. This is the Hostfurl independent version of Minformhf.

To work with formsubmit.io the following edits are required in `_data/site.yml`:

```
nohtmx: true
corsprod: true
corsurl: https://formsubmit.co
formpath: /somearbitrarycharacters
```

Demo at https://minform.hostfurl.com

<cite>https://discord.com/channels/741017160297611315/1494619630273298504/1495806652396601444</cite>

</blockquote>

#### Cloudflare Workers, D1, and Turnstile

<blockquote>

I recently implemented forms for recipe reviews and membership signup using Cloudflare Workers, D1, and Turnstile.

Here's an example:
https://marcellosplace.com/recipes/sweet-potato-apple-cake/#new-review

Turnstile invisibly protects form submissions against abuse. Cloudflare Workers process them and store them into D1.

It costs pennies and so far works perfectly.

<cite>https://discord.com/channels/741017160297611315/1494619630273298504/1495698228417658942</cite>

</blockquote>
