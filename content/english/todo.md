---
title: Gopi's TODO List
slug: todo
---

List of thins to od


## Status

this is **bold**

## TODO

1. Update jQuery in bookdown: https://github.com/rstudio/bookdown/issues/1118 https://github.com/rstudio/bookdown/pull/882 https://github.com/rstudio/bookdown/pull/693
1. Revert inline CSS to `<style>`: https://github.com/rstudio/bookdown/issues/1170

## Done

This section is cleaned up from time to time.

1. Syntax highlighting of `|>`: https://github.com/rstudio/bookdown/issues/1157
1. `targets` engine in knitr: https://github.com/yihui/knitr/pull/2031
1. Delete the duplicated `config/` dir: https://github.com/rstudio/blogdown/issues/644
1. Record a video about [CSS selectors for R Markdown users](https://github.com/yihui/rmarkdown-cookbook/pull/239/files).



<script>
document.querySelectorAll('.main a').forEach(function(el) {
  var t = el.innerText;
  if (!/^https:/.test(t)) return;
  el.innerText = t.replace(/^https:\/\/(www\.)?/, '')
    .replace(/#.*/, '')
    .replace(/^github.com\/([^\/]+)\/([^\/]+)\/(issues|pull)\/(\d+).*/, '$1/$2#$4')
    .replace(/^github.com\/([^\/]+)\/([^\/]+)\/(releases)\/tag\/([^\/]+).*/, '$1/$2@$4')
    .replace(/^stackoverflow.com\/q\/(\d+).*/, 'SO/$1')
    .replace(/^community.rstudio.com\/t\/(\d+).*/, 'RC/$1')
    .replace(/^twitter.com\/([^\/]+)\/([^\/]+)\/(\d+).*/, 'twitter/$3')
    .replace(/^github.com/, 'GH');
});
</script>
