---
title: Jekyll世界
date: '2012-02-12'
slug: hello-jekyll
---

一晃三个月过去，这里似乎没了动静。各位大人、路人以及丈人都很好奇，这娃儿究竟干啥去了，于是今天从山沟沟里爬出来解释一下。三个月前我说那是我在WordPress（WP）下写的最后一篇日志，话扔出来了当然不能反悔，尽管中途有几次想写点东西，但都憋回去了。不写日志也好，省点时间写代码。去年[10月份中旬](https://github.com/yihui/knitr/graphs/impact)我鬼使神差开始写一个叫[knitr](http://yihui.org/knitr/)的新包，其实也是我盘算了几年一直没干的一件事，最后对Sweave终于忍到了极点，操起键盘花了三个月革了命。这是题外话，以后再细说。

每个人离开一个软件或一套系统一般都带着负面情绪，比如烦恼抓狂恨，但WP必然不属于这一类系统；我看到的几乎每一个离开WP投奔[Jekyll](http://github.com/mojombo/jekyll/)的人都无一例外大加赞扬WP，这事情就很有趣了，为什么你赞它还要弃用它？我虽然已经换到Jekyll，但也同样赞WP并感恩戴德，过去我已经说过好几次WP是程序设计的上乘之作，它的功能之灵活以及API之清晰别的网站系统很难比拟。然而某些码农的目标只是把事情做完（GTD），某些码农的追求则是无止境的，我就属于极简主义者，理想情况下我希望一套系统只有一个主要功能，把其它枝叶都砍掉，让用户能集中精神只做一件事情。比如博客网站只有写作功能，论坛只有讨论问题功能，聊天软件只有聊天功能。WP基本上符合这个要求了，它和其它的网站系统比，已经大大简化，只要模板设定好，剩下的就是写作；话虽这么说，实际情况却并非如此，我还是要花精力做一些额外的事情，比如我需要上网，要登录后台，要编辑HTML（像我这样的代码洁癖，眼里容不得冗余代码），要管理图片和附件，看着别人的新插件还眼馋（一装就又陷入新的维护陷阱），最要命的是，所有的东西都在数据库中，每次WP出了新版本，我都要颤颤巍巍点那个更新按钮，然后祈祷数据库不要出问题（我懒得导入导出备份）。

Jekyll完全推翻了传统网站的维护方式，它直接回到了“原点”——作者只需要维护文本文件，每一篇日志就是一个文件，程序会根据模板设置自动把这些文本文件翻译为网页。这些文本文件不用HTML，而是用简化版本的Markdown（MD）或者其它可最终翻译为HTML的伪标记语言。MD的哲学深得我心：把[语法](http://daringfireball.net/projects/markdown/)简化90%，去实现大多数常用的HTML标签，牺牲少数不常用的标签（这些标签仍然可以用原始的HTML代码写）。比如要写无序列表的话，在HTML里面要用

```html
<ul>
  <li>hello</li>
  <li>world</li>
</ul>
```

每一项列表项都用`li`标签围起来，而在MD语法里，只需要一行一行写就行了，每一行开头写一个减号 `-` 就足够，就像自己记笔记一样：

```md
- hello
- world
```

一个字符（确切地说是两个，后面还得跟个空格）和一串要重复敲的字符比，哪个简洁显而易见。简洁的MD语法配合几项YAML设置就是一篇日志，扔进Liquid模版系统，Jekyll就把网站编译出来了。

八年前我在用文本文件做网站，八年后我又回到了文本文件，当然事情已经有了本质变化。这次从WP搬家，尽管有一些自动转换程序，但还是费了不少劲，423篇中文，103篇英文，几千评论，搬得我差点没疯掉。比如我做的第一件事情是解决[上一次搬家](/cn/2009/05/php-301-redirect-from-bo-blog-to-wordpress/)的历史遗留问题：从Bo-blog搬到WP的时候，有些评论的嵌套关系乱了，所以我花了一天时间先把评论在数据库中修改对齐，这个过程基本上是手工看评论ID，把父评论和子评论的ID都记下来，然后用R生成几百条SQL语句，扔给数据库执行。评论整完导入Disqus，一个专注于做评论的网站。剩下的日志用一个Python程序从WP的XML文件导出为MD文件，导完又是一片残垣断壁，我只整理了最近的十篇日志，之前的几百篇用R正则表达式简单处理了一下，以后再慢慢手工整理，再往后还想把2004年起的一些老日志也导进来，像王晓伟说的，[记录生活](http://www.blog496.org/2011-2-11-stand-in-the-cross-road.html)。英文[简历页面](/en/vitae/)花了很大功夫整理了一下，主要是那些幻灯片文件，整体挪到GitHub中[下载](https://github.com/yihui/yihui.github.com/downloads)，尽管这样会造成一批404错误，但文件太多，重定向太麻烦，想想算了。

凡事如果能退到文本文件的层面，基本上就意味着可以为所欲为了。就如同LaTeX是纯文本文件，所以很方便和R结合生成动态文档；PHP是纯文本文件，可以任意混合HTML代码。如果我乐意，我可以在MD代码里嵌入R代码，动态生成日志（这个实际上已经在knitr中实现了）。

使用Jekyll的另一大动力当然是GitHub，它提供编译服务，所以用户只需要用GIT管理文本文件就可以了。要写日志就新建一个文本文件，写完推上去完事，由于GIT支持离线工作，随时随地都可以写，不受网络环境限制。

为了找一个中意的模板，我把Jekyll维基上的网站列表扒了几遍，最后找到一个符合我理想中的样式的网站，[作者](http://lhzhang.com)也是极简主义者。这个模板适合日志，但不太适合首页，所以我在[首页](/)用了另一套模板。中文字体使用肖楠介绍过的[冬青黑体](http://www.road2stat.com/cn/tag/hiragino-sans-gb)和微软雅黑，这样苹果和Windows都能看，而我相信Linux用户对中文字体总是有办法的，比如自己调一下文泉驿字体；英文优先使用Google字体中的Galdeano，然后使用其它常见无衬线字体。整个网页使用了一些HTML5标签，所以关于Windows下的IE浏览器我就不用多说了，若版本不够，页面可能会错乱。

日志页面中支持键盘左右方向键或JK键前后导航，这是JavaScript实现的，归功于[Tao Zhang](http://ztpala.com/2012/01/16/jquery-keyboard-navigation/)。文章[RSS订阅](/cn/feed/)依然存在，所有日志的链接也没有变化，只是评论RSS变了，要么订阅[整站评论](http://yihui.disqus.com/latest.rss)，要么订阅单篇文章评论（每个页面的底部）。

一连看几年的文章的感触非常大，就像看一部快速播放的电影，生活在其中一天天过没什么感觉，但呼哧一下看过去，感觉很不一样，我从过去自己的一些评论和文章里总结了我的（至少）四点明显问题：

- 明明年轻却卖老
- 气盛，欺人
- 很多评论非常无聊，为了评论而评论
- 中英混杂

关于这些事，想想有点后背发凉，尤其是第二点，必然伤了一些人；而其中第四点我现如今逮一个批一个，不管是谁（包括师姐在内），不料自己过去其实也是这样的。