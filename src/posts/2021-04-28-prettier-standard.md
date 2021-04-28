---
layout: post
title: Prettier and Standard in VSCode
description: The easiest way to use Prettier and Standard together in VSCode
slug: prettier-standard
tags: ['writing', 'vscode', 'tools', javascript]
---
[Prettier](https://prettier.io) is an opinionated tool that helps you format code. I love Prettier, but I don't like its opinions with JavaScript. I prefer using [Standard](https://standardjs.com) for JavaScript because it doesn't have semicolons (which makes the code cleaner to read). 

It used to be complicated to use Prettier and Standard together. We had to [disable Prettier for specific languages](/blog/prettier-disable-languages). Thankfully, there's a simpler way now. 

<!-- more -->

We can use an extension called [Prettier Standard VSCode](https://marketplace.visualstudio.com/items?itemName=numso.prettier-standard-vscode). It changes JavaScript from the Prettier default format into Standard.

I've tested this extension and it continues to work like all other Prettier extensions like `.html` and `.css`. 

The good thing about using Prettier Standard VSCode is we can continue to use Standard in files with mixed syntaxes like HTML and markdown. 

Here's an example where I edited markdown with Prettier:

<figure role="figure">
  <img src="/images/2021/prettier-standard/prettier.gif" alt="Markdown edited with Prettier">
</figure> 

And here's one with Prettier Standard. 

<figure role="figure">
  <img src="/images/2021/prettier-standard/prettier-standard.gif" alt="Markdown edited with Prettier Standard">
</figure> 

For languages that Prettier doesn't support, you can always [overwrite Prettier with a different formatter](https://zellwk.com/blog/prettier-disable-languages#enabling-prettier-globally-but-disabling-it-in-specific-languages), like this: 

```javascript
"[nunjucks]": {
  "editor.defaultFormatter": "okitavera.vscode-nunjucks-formatter"
},
```
I hope this helps you set up your JavaScript environment!