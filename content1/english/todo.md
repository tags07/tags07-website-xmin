---
title: Yihui's TODO List
slug: todo
---

This page contains my TODO items, which I try to update every day. I guess I will never be able to finish all the work, so I will appreciate your help with any of the items on this page (fixing bugs, answering questions, or implementing features). Please feel free to let me know if you want to work on anything, and I will be happy to assist you.

Looking at these items, you may make a better decision on whether to ask questions on a public forum before [emailing me](/en/about/#contact-me), according to my current status below. Please feel free to email me anyway if you do not need a prompt response, and please forgive my slow response.

## Status

At the moment, I have **152** emails in my inbox to be dealt with (the earliest that I have not replied to was from _Nov 21, 2018_), **25** unread Github issues/PRs, and about **30** tabs open in my browser.

I just came back from vacation on July 14, 2021. I'm catching up on Github issues and emails.

## TODO

1. Update jQuery in bookdown: https://github.com/rstudio/bookdown/issues/1118 https://github.com/rstudio/bookdown/pull/882 https://github.com/rstudio/bookdown/pull/693
1. Revert inline CSS to `<style>`: https://github.com/rstudio/bookdown/issues/1170
1. Questions to be answered:
    - https://stackoverflow.com/q/67853909/559676 Why is the image not rendered?
    - https://community.rstudio.com/t/106550 Why shortcode doesn't work in `.Rmd -> .html`
    - https://community.rstudio.com/t/106243 How to read a chunk from an external Rmd? Perhaps I need to export the parser from **knitr**, although there is a **parsermd** package, which I haven't taken a close look yet
1. blogdown book PRs: https://github.com/rstudio/blogdown/pull/619 https://github.com/rstudio/blogdown/pull/620 https://github.com/rstudio/blogdown/pull/623 
1. Read and probably respond to a few posts related to blogdown:
    - https://solomonkurz.netlify.app/post/2021-05-03-blogdown-updates-prompted-a-website-overhaul-these-are-my-notes/ Overhaul a blogdown site
    - https://www.jumpingrivers.com/blog/moving-to-hugo-tips-tricks-optimisation/ Hugo tips and tricks
    - https://shilaan.rbind.io/post/building-your-website-using-r-blogdown/ A blogdown guide
    - https://seth-dobson.github.io/r-blogging-on-a-chromebook/ Need to tell the author that Hugo could be installed inside the website project by setting [the global option `blogdown.hugo.dir`](https://bookdown.org/yihui/blogdown/more-global-options.html).
    - https://clauswilke.com/blog/2020/09/08/a-blogdown-post-for-the-ages/ Not sure if the author knows that blogdown no longer re-knits Rmd posts by default. Similarly, need to double check https://yutani.rbind.io/post/2017-10-25-blogdown-custom/.
    - https://sharleenw.rbind.io/2020/09/02/how-to-remake-a-blogdown-blog-from-scratch/ Need to learn more about her pain with blogdown.
    - https://portfolio.peter-baumgartner.net/2018/07/19/blogdown-using-themes/ Learn more about his lessons.
    - https://drmowinckels.io/blog/2020-05-25-changing-you-blogdown-workflow/ I guess most of her problems have been addressed in the latest version of blogdown, but needs to double check.
    - https://www.datalorax.com/post/new-website-theme/ Choosing themes.
    - https://www.garrickadenbuie.com/blog/add-a-generated-table-of-contents-anywhere-in-rmarkdown/ TOC
    - https://themockup.blog/posts/2020-08-01-building-a-blog-with-distill/ https://werk.statt.codes/post/2021-02-24-hellodistill/ Learn more about distill.
    - https://education.rstudio.com/blog/2021/02/distill-it-down/
1. Max's [SO question on highlighting inline code](https://stackoverflow.com/q/62629755/559676), which should be solvable via [**highr**](https://github.com/yihui/highr).
1. Replace sundown with **commonmark** in **markdown**: https://github.com/yihui/knitr/issues/1329
1. Optimize images automatically in blogdown
1. Fix relative paths in Hugo's RSS feeds: https://github.com/rstudio/blogdown/issues/384
1. hugo-prose: https://github.com/yihui/hugo-prose/pull/41
1. Scrollama with blogdown/distill: https://github.com/yihui/rolldown/issues/14
1. Watch https://resources.rstudio.com/resources/rstudioglobal-2021/
1. A possible book: Presentation Ninja (xaringan, ioslides, slidy, revealjs, PowerPoint, beamer, shower, etc).
1. A possible book about pagedown and CSS.
1. Reply to https://github.com/yihui/rmarkdown-cookbook/issues/215#issuecomment-633148829
1. Digest https://github.com/rstudio/distill/issues/152.
1. Look into this problem: https://stackoverflow.com/q/60014350/559676. Sounds like a bug introduced by a certain version of bookdown.
1. Review https://github.com/rstudio/DT/pull/836

## Done

This section is cleaned up from time to time.

1. Syntax highlighting of `|>`: https://github.com/rstudio/bookdown/issues/1157
1. `targets` engine in knitr: https://github.com/yihui/knitr/pull/2031
1. Delete the duplicated `config/` dir: https://github.com/rstudio/blogdown/issues/644
1. Release blogdown to CRAN: https://github.com/rstudio/blogdown/releases/tag/v1.4
1. review https://github.com/rstudio/bookdown/pull/1201
1. install arm hugo: https://github.com/rstudio/blogdown/issues/636
1. clean *_files dirs: https://github.com/rstudio/blogdown/issues/632
1. https://github.com/rstudio/rmarkdown/pull/2190
1. https://github.com/rstudio/bookdown/pull/1035
1. https://github.com/yihui/tinytex/pull/318
1. https://github.com/rstudio/rmarkdown/issues/2187
1. bookdown 404 https://github.com/rstudio/bookdown/pull/1035
1. keep the first URL only in citation https://github.com/yihui/knitr/issues/2028
1. Hugo academic theme is broken again: https://github.com/rbind/apreshill/issues/44#issuecomment-873312747 https://github.com/rstudio/blogdown/issues/638
1. A talk in the "My first useR" session at useR 2021 on July 4th, tentatively titled "My journey in writing books and blogging about R".
1. Write out tinytex regexes to json: https://yihui.org/tinytex/regex.tar.gz

## Backlog

1. Support HTML widgets in **pagedown**: https://github.com/rstudio/pagedown/pull/87
1. A Hugo theme based paged.js? https://www.pagedjs.org
1. A Hugo layout for cards? https://apreshill.github.io/postcard/about.html
1. A possible book on small successes. https://www.tiffanymatthe.com/not-extraordinary <!-- https://docs.google.com/document/d/1of3Q0ufUGLQ5ZYoF939qFzBR6rW5XoNhPtVJwoHoGEk/edit# -->
1. Google doc to Markdown? <!-- Then we can even blog with Google doc -->
1. Read Miles's introduction to **drake** and include it in the R Markdown Cookbook: https://milesmcbain.xyz/the-drake-post/ (Update: Will said **targets** would be the new **drake**, so no need to introduce **drake**)
1. Record a video about [CSS selectors for R Markdown users](https://github.com/yihui/rmarkdown-cookbook/pull/239/files).

## Help Needed

If anyone is interested in any of the items below, please feel free to let me know. I'd be happy to explain more, or do a video chat with you.

1. How can users build and install their own version of TinyTeX? Short answer: install [`TinyTeX-0`](https://github.com/yihui/tinytex-releases), use `tlmgr` to install the packages they need, zip the TinyTeX installation directory, and publish it somewhere (e.g., Github Releases, or AppVeyor artifacts). To install this custom version of TinyTeX, I'll need to provide an environment variable to customize the URL in my installation scripts (e.g., not hard-coding yihui.org or github.com/yihui/tinytex-releases in [install-bin-unix.sh](https://github.com/yihui/tinytex/blob/master/tools/install-bin-unix.sh)), so they can be reused by others. 
1. Introduce the easier way to start a **bookdown** project using the RStudio IDE in the book: https://github.com/rstudio/bookdown/issues/225
1. Build **rggobi** on r-universe.dev: https://github.com/ggobi/rggobi/issues/7
1. More accessibility/navigation tags in `knitr::kable_html()`: https://github.com/yihui/knitr/issues/1747
1. Generate the Table of Contents for **xaringan** slides: https://github.com/yihui/xaringan/issues/217
1. How to render math expressions without MathJax? https://stackoverflow.com/q/57121846/559676 Alternative methods are listed here: https://pandoc.org/MANUAL.html#math-rendering-in-html
1. The pain of using **rmarkdown** on network drives: https://github.com/rstudio/rmarkdown/issues/1268
1. BibTeX references showing up twice in **bookdown**: https://github.com/rstudio/bookdown/issues/751
1. Make TinyTeX more portable: https://github.com/yihui/tinytex/issues/133
1. `xfun::numbers_to_words()` for numbers with decimal places: https://github.com/yihui/xfun/issues/18
1. Live code in xaringan: https://github.com/yihui/xaringan/issues/206 The implementation is not totally clear to me, but I imagine users can double click on a code block on a slide to edit the code, and the edit can be sent back to the RStudio IDE or executed.

## Blog

1. What does it mean to be generous? https://github.com/ropensci/targets/issues/503 I don't think I'm generous in this case.
1. https://statmodeling.stat.columbia.edu/2021/05/23/thinking-fast-slow-and-not-at-all-system-3-jumps-the-shark/ https://twitter.com/kjhealy/status/1394729017631285252 Sounds like this new book has got quite a bit of controversy, but I haven't read it.

## Reading

1. JavaScript for R https://book.javascript-for-r.com Seems to be an interesting book on the only two languages that I understand.
1. https://atrebas.github.io/post/2020-06-17-datatable-introduction/ https://martinctc.github.io/blog/comparing-common-operations-in-dplyr-and-data.table/

## 待办事项

1. https://yufree.cn/cn/2018/03/24/blogdown-rss/

## 私人事项

1. 通读 https://yihanxu.github.io/archive/
1. 一堆未读推特消息，从 2020/07/01 开始：<https://t.yihui.org>
1. 这位大人对 knitr 钻研似乎颇深，是个人才，也许可以拉来做点什么事：<https://stackoverflow.com/users/2706569/cl>
1. 家教有关的阅读
    - https://twitter.com/Idzie/status/1247946036733190145
    - https://www.thecut.com/2020/03/unschooling-your-kids-during-coronavirus-quarantine.html
    - https://qz.com/1828551/parents-who-didnt-choose-to-homeschool-this-is-an-opportunity/
1. https://josebrowne.com/on-coding-ego-and-attention/
1. https://fortelabs.co/blog/how-to-take-smart-notes
1. https://www.samuelthomasdavies.com/book-summaries/business/deep-work/
1. https://highexistence.com/5-reasons-modern-life-depression/
1. 黑客与画家 http://idlewords.com/2005/04/dabblers_and_blowhards.htm
1. [教养的迷思](https://book.douban.com/subject/26612510/) https://mp.weixin.qq.com/s/4XmMuUV2XbM-UMD4GJGUMQ
1. [家庭、私有制和国家的起源](https://www.marxists.org/chinese/engels/marxist.org-chinese-engels-1884-3.htm) https://en.wikipedia.org/wiki/The_Origin_of_the_Family,_Private_Property_and_the_State
1. Note-taking/todo app https://d.cosx.org/d/419756/10 https://noteplan.co https://everydaycheck.com https://twitter.com/OilGains/status/1085929376741556230
1. Stoicism: https://dailystoic.com/letters-from-a-stoic/ https://www.lettersfromastoic.net/letter-4/
1. ggplot 灰色背景：https://stats.stackexchange.com/q/25220/10946 https://twitter.com/WilliamsNeuro/status/1318419069968658432
1. 为 XD 和邻居架设网站
1. 用 `IntersectionObserver` 而不是 `scroll` 事件检测评论区是否滚到了当前视图下： https://blog.skk.moe/post/prevent-disqus-from-slowing-your-site/
1. [洛宁蒸肉](https://mp.weixin.qq.com/s/6UGYqfXzvBjBa8xJYPhGFQ)：五花肉、粉丝、玉米面、葱姜蒜、酱油、蚝油、盐。

## 随机事项

1. JS 生成声音：<https://github.com/R4meau/plink-plonk/blob/master/content.js> 暂时不知道用它干啥，但感觉要是跟 Shiny 鬼混在一起也许能玩出什么花样来。
1. https://two.js.org
1. https://github.com/seankross/postcards
1. https://github.com/etiennebacher/docsifier
1. https://twitter.com/Warreningshot/status/1379664918450905089 blogdown 复古主题？

## 日程安排

| 时间 | 事项                                             |
|------|--------------------------------------------------|
| 周一 | 朝九晚五；下午核查团队工作进度 |
| 周二 | 朝九晚五 |
| 周三 | 朝九晚五 |
| 周四 | 朝九晚五 |
| 周五 | 下午非紧急邮件、COS + SO 论坛、Disqus 后台；微博；推特 |
| 周六 |  |
| 周日 | 晚上看 Feedly |

另外，每天下班前一小时：查阅 Github 事项、安排第二天工作。晚 11 点后回复微信。


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
