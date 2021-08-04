---
title: 最近一则让我有意回复邮件的例子
date: '2018-11-07'
slug: email-reply
---

现在翻我博客的人[应该基本都知道](/cn/2018/09/inbox-zero/)，我回复陌生人邮件的概率已经比较渺茫，但这并不代表我会忽略所有陌生人的邮件。其实我回不回陌生人邮件只取决于一条原则：你是否展示了你的用心。我前面说的邮件需要到“催人泪下”的程度是开玩笑的。

昨天 COS 微信群里依含大人发了一个邮件例子，结果引起了大家的热烈讨论。以太云为首的不拘小节的温和派觉得这邮件写得还可以，而还有些人（尤其是学术界人士）觉得这邮件写得完全不及格，收到就该扔进垃圾桶，不用回复。我是倾向后者的，因为那邮件写得太含混不清，不知具体要问什么，让人无法作答。其它问题如称呼、落款、标点符号对我来说算是次要的。还有个小问题很有意思，就是发送者称呼依含大人为“小姐姐”；在这个问题上，大家又分成两派，有人觉得没什么不妥、很欢乐啊，有人觉得太不正式。当然，我也是倾向于后者。如果是第一次给别人发邮件，你宁可过于正式，也不要贸然耍宝开玩笑。前者不会有任何风险，收件人讲究与不讲究都可以接受；后者要是碰到讲究的人就完蛋了。

在《深度工作》一书中的最后，作者有句话让我终于觉得可以卸下邮件重担而不必对别人负疚。他说是否能得到回复主要是发件人的责任，发件人应该自己想办法提高获得回复的可能性。我们为什么要回复写得不好的邮件呢？从发件人的角度来看，我觉得很多人可能都没有想过，自己的一封邮件出去会在别人的邮箱里排多长的队，也就是需要跟多少其它邮件竞争、获得收件人的注意。邮件这种形式总让我们感觉像电话一样是一对一的私人沟通、从而觉得对方一定会应答，但它的异步性决定了它跟电话有本质区别。

前几天有人给我发邮件问一个跟我的一个 R 包有关的问题，按惯例这种邮件我是不会回复的，但这位小主开篇就说“我看过你的博客，知道你不回答这样的问题”，接下来详细描述了其失败尝试，并告诉我这件事已经耗费了很长时间，但限于数据敏感性而无法造出可重现的例子。我看了描述，事情确实是很诡异，而且发件人显得很认真，所以我二话没说就回复了。在一来一去七个回合之后，伊终于造出了一个可重现的例子，然后我一眼就看出了问题所在；虽然这问题解释起来有点费劲（需要额外的背景知识），但我还是吭哧吭哧把原因尽量详述了一番，并给出了解决方案。下面总结一下我为什么回复这邮件：

1. 当我知道发件人已经了解我的邮件标准时，就可以移除其陌生人属性了，何况还伊解释了为什么这问题无法发到公开的论坛上（如 Stack Overflow）；起码人家尝试过了解我的原则，这是用心的体现。

1. 伊没有给我施加任何回复的压力（没有“急！”“求助！”“你是我[唯一的希望](/cn/2015/10/only-hope/)！”），让我感觉即使不回复也会得到谅解，这种情况下反而会让我更有意回复。

1. 第一遍问题描述我并没有完全看懂，但我得到的信息是，这问题相当诡异，伊可以对天发誓这是真实存在的问题，后来还发来了截图为证。这激起了我的好奇心。相比起写代码，其实我对代码查错更有兴趣，我特别喜欢研究为什么代码不能按预期运行这种问题，这样的过程有种侦探感。

在我的标准下，这邮件的中英混杂程度略超标，但在上面三个前提条件下，这一点小问题根本不算什么，我乐意放弃这条个人原则。

颜大站长在上面的微信群中最后的总结很到位：邮件就是时间交换，而双方的单位时间很多时候都不等价（这么说又政治不正确了）。所以发件人需要估摸一下，用自己多少单位的时间能交换到对方一单位的时间。