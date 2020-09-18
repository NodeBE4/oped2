---
layout: post
title: "黑客如何使用dorks - iYouPort"
date: 2020-09-17T16:03:40+00:00
author: iYouPort
from: https://www.iyouport.org/%e9%bb%91%e5%ae%a2%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8dorks/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-14472 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-osint category-54 category-67 tag-dorks tag-googledorking tag-hacker tag-hacktivist tag-technique tag-technology" id="post-14472">
 <header class="entry-header">
  <h1 class="entry-title">
   黑客如何使用dorks
  </h1>
 </header>
 <div class="entry-meta">
  <span class="byline">
   <a href="https://www.iyouport.org/author/don-evans/" rel="author" title="由McCaffrey发布">
    McCaffrey
   </a>
  </span>
  <span class="cat-links">
   <a href="https://www.iyouport.org/category/knowledge-node/" rel="category tag">
    Knowledge Node
   </a>
   ,
   <a href="https://www.iyouport.org/category/osint/" rel="category tag">
    OSINT
   </a>
   ,
   <a href="https://www.iyouport.org/category/%e6%8a%80%e6%9c%af%e9%98%b2%e8%ba%ab-%e8%87%aa%e6%88%91%e4%bf%9d%e6%8a%a4%e6%96%b9%e6%b3%95/" rel="category tag">
    技术防身/自我保护方法
   </a>
   ,
   <a href="https://www.iyouport.org/category/%e7%bb%99%e8%a1%8c%e5%8a%a8%e8%80%85%e7%9a%84%e6%8a%a4%e8%ba%ab%e7%ac%a6%e5%92%8c%e6%ad%a6%e5%99%a8/" rel="category tag">
    给行动者的护身符和武器
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2020-09-18T00:03:40+08:00">
    2020年9月18日
   </time>
   <time class="updated" datetime="2020-09-18T00:03:23+08:00">
    2020年9月18日
   </time>
  </span>
  <span class="word-count">
   1 Minute
  </span>
 </div>
 <div class="entry-content">
  <ul>
   <li class="graf graf--p">
    <span style="color: #00ccff;">
     <em>
      <strong>
       本文介绍一些基本方向，您可以尽情发挥创意。创造力是永无止境的
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <p>
   <img alt="" class="aligncenter size-full wp-image-14473 jetpack-lazy-image" data-lazy-sizes="(max-width: 1100px) 100vw, 1100px" data-lazy-src="https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=1100%2C618&amp;is-pending-load=1#038;ssl=1" data-lazy-srcset="https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?w=1280&amp;ssl=1 1280w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=300%2C169&amp;ssl=1 300w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=1024%2C575&amp;ssl=1 1024w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=768%2C431&amp;ssl=1 768w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=1100%2C618&amp;ssl=1 1100w" data-recalc-dims="1" height="618" src="https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=1100%2C618&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1100"/>
   <noscript>
    <img alt="" class="aligncenter size-full wp-image-14473" data-recalc-dims="1" height="618" sizes="(max-width: 1100px) 100vw, 1100px" src="https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=1100%2C618&amp;ssl=1" srcset="https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?w=1280&amp;ssl=1 1280w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=300%2C169&amp;ssl=1 300w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=1024%2C575&amp;ssl=1 1024w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=768%2C431&amp;ssl=1 768w, https://i2.wp.com/www.iyouport.org/wp-content/uploads/2020/06/00-7.jpeg?resize=1100%2C618&amp;ssl=1 1100w" width="1100"/>
   </noscript>
  </p>
  <p class="graf graf--p">
   GoogleHacking 的概念最早由 Johnny long 引入；而 Google Dork 最初是指无法保护在线内容的那种人。 Google 可以很容易地挖掘出这种无能。后来这个词的含义逐渐随着时间而改变，目前它指的是，从 Google 获得机密信息的人。
  </p>
  <p class="graf graf--p">
   我们已经多次介绍过 dorking 的用法，它是开源情报收集的支柱之一。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%94%bb%e9%98%b2%e7%9a%86%e5%8f%af%e7%94%a8%ef%bc%9agoogledorking-%e9%ab%98%e7%ba%a7%e8%bf%90%e7%ae%97%e7%ac%a6%e5%ae%8c%e6%95%b4%e5%88%97%e8%a1%a8/" href="https://www.iyouport.org/%e6%94%bb%e9%98%b2%e7%9a%86%e5%8f%af%e7%94%a8%ef%bc%9agoogledorking-%e9%ab%98%e7%ba%a7%e8%bf%90%e7%ae%97%e7%ac%a6%e5%ae%8c%e6%95%b4%e5%88%97%e8%a1%a8/" rel="noopener noreferrer" target="_blank">
     攻防皆可用：GoogleDorking 高级运算符完整列表
    </a>
    》
   </li>
   <li class="graf graf--li">
    实践《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%b7%a7%e7%94%a8%e4%ba%92%e8%81%94%e7%bd%91%ef%bc%8c%e4%bb%a5%e6%89%be%e5%88%b0%e6%82%a8%e6%9c%80%e6%83%b3%e8%a6%81%e7%9a%84%e4%bf%a1%e6%81%af%ef%bc%9a%e6%90%9c%e7%b4%a2%e6%80%9d%e7%bb%b4%e6%98%af/" href="https://www.iyouport.org/%e5%b7%a7%e7%94%a8%e4%ba%92%e8%81%94%e7%bd%91%ef%bc%8c%e4%bb%a5%e6%89%be%e5%88%b0%e6%82%a8%e6%9c%80%e6%83%b3%e8%a6%81%e7%9a%84%e4%bf%a1%e6%81%af%ef%bc%9a%e6%90%9c%e7%b4%a2%e6%80%9d%e7%bb%b4%e6%98%af/" rel="noopener noreferrer" target="_blank">
     巧用互联网，以找到您最想要的信息：搜索思维作为基本功
    </a>
    》
   </li>
   <li class="graf graf--li">
    实践《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e7%a4%be%e4%ba%a4%e7%bd%91%e7%ab%99%e4%b8%8a%e8%bf%9b%e8%a1%8c%e6%96%b0%e9%97%bb%e6%94%b6%e9%9b%86%e5%92%8c%e7%9b%91%e8%a7%86%e7%9a%84%e5%9f%ba%e6%9c%ac%e6%8c%87%e5%8d%97/" href="https://www.iyouport.org/%e7%a4%be%e4%ba%a4%e7%bd%91%e7%ab%99%e4%b8%8a%e8%bf%9b%e8%a1%8c%e6%96%b0%e9%97%bb%e6%94%b6%e9%9b%86%e5%92%8c%e7%9b%91%e8%a7%86%e7%9a%84%e5%9f%ba%e6%9c%ac%e6%8c%87%e5%8d%97/" rel="noopener noreferrer" target="_blank">
     社交网站上进行新闻收集和监视的基本指南
    </a>
    》
   </li>
  </ul>
  <p class="graf graf--p">
   不论是针对目标个人还是组织的深入挖掘、不论是对目标网络的窥探还是搜罗机密信息，Google Dork 都是一个强大的工具 — — 完全免费，任何人都可以使用。
  </p>
  <p class="graf graf--p">
   我们上传过一份手册介绍了 GoogleHacking 的白色、灰色、黑色情报的操作方法，简单易懂。您可以在这里下载：
   <a class="markup--anchor markup--p-anchor" data-href="https://www.patreon.com/posts/ai-zi-shi-zhi-de-38193081" href="https://www.patreon.com/posts/ai-zi-shi-zhi-de-38193081" rel="noopener noreferrer" target="_blank">
    https://www.patreon.com/posts/ai-zi-shi-zhi-de-38193081
   </a>
  </p>
  <p class="graf graf--p">
   获取那种不会引起道德和法律关注的数据的方法被称为 &lt;开源白色情报&gt;，包括搜索已删除的和存档的页面、搜索有关目标人的某些信息、以及其他实质性信息等。
  </p>
  <p class="graf graf--p">
   &lt;灰色情报&gt; 指的是那些引起道德关注的信息 — — 包括获取网站的作者和所有者（无意识地）留下的信息，有关网站结构的信息、以及服务器的配置参数等等。
  </p>
  <p class="graf graf--p">
   所谓的 &lt;黑色情报&gt; — — 指的是比较激进的玩法，比如通过挖掘以获得内幕和机密信息、敏感的个人数据、以及程序和设备的配置参数的潜力。
  </p>
  <p class="graf graf--p">
   总之，GoogleHacking 都能做到。
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    并且不仅谷歌有 dork，其他搜索引擎包括社交媒体平台搜索引擎，在此大同小异
   </strong>
   ；比如我们介绍过的 tweetdeck 中使用的锁定目标方法等等。
  </p>
  <p class="graf graf--p">
   今天介绍的是黑客在攻击前的侦查阶段使用的 dorks，也就是上述的灰色玩法。
  </p>
  <p class="graf graf--p">
   这些技术在
   <strong class="markup--strong markup--p-strong">
    手动侦查
   </strong>
   中非常有用，可以找到有关任何目标组织的关键信息，这些信息可能由于某些操作不当的后果而被遗漏在互联网上了。
  </p>
  <p class="graf graf--p">
   这里有一个视频：
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="421" src="//www.youtube.com/embed/cFOBUYaxdWI" width="750">
   </iframe>
  </p>
  <p class="graf graf--p">
   这是 Google Hacking Database（GHDB）的官方链接：
   <a class="markup--anchor markup--p-anchor" data-href="https://www.exploit-db.com/google-hacking-database" href="https://www.exploit-db.com/google-hacking-database" rel="noopener noreferrer" target="_blank">
    GHDB
   </a>
  </p>
  <p class="graf graf--p">
   您永远都可以创造新的独特 Dork，可以发布它，将其添加到整个数据库中让大众受益。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    Google Dorks 的公式
   </strong>
  </h3>
  <p class="graf graf--p graf--startsWithDoubleQuote">
   “inurl:.“domain”/“dorks” ”
  </p>
  <p class="graf graf--p">
   通常这样理解：“inurl” = input URL；“domain” =您想要的域。例如，.gov或.edu等，取决于您的目标；“dorks” = 您选择的dork。
  </p>
  <p class="graf graf--p">
   您可以使用以下单词代替 inurl：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    intitle:
   </li>
   <li class="graf graf--li">
    inurl:
   </li>
   <li class="graf graf--li">
    intext:
   </li>
   <li class="graf graf--li">
    define:
   </li>
   <li class="graf graf--li">
    site:
   </li>
   <li class="graf graf--li">
    phonebook:
   </li>
   <li class="graf graf--li">
    maps:
   </li>
   <li class="graf graf--li">
    book:
   </li>
   <li class="graf graf--li">
    froogle:
   </li>
   <li class="graf graf--li">
    info:
   </li>
   <li class="graf graf--li">
    movie:
   </li>
   <li class="graf graf--li">
    weather:
   </li>
   <li class="graf graf--li">
    related:
   </li>
   <li class="graf graf--li">
    link:
   </li>
  </ul>
  <p class="graf graf--p">
   上面的列表只是一些典型的示例，您可以深入研究它们并使用您选择的任何Dork，以相应地产生结果。
  </p>
  <p class="graf graf--p">
   请务必理解，不仅限于 Google，
   <strong class="markup--strong markup--p-strong">
    Dorks 在 Bing、Duck Duck Go、AOL 和 Yahoo 等众多搜索引擎上都是有效的。
   </strong>
  </p>
  <p class="graf graf--p">
   赏金猎人使用 Dorks 的主要原因之一是为了寻找第三方来源。组织和公司在日常运营中会使用 Pastebin，Jira，Github，Trello，Coggle 等等网站。在某些情况下，通常会将硬编码凭据存储在这样的公共平台上。
  </p>
  <p class="graf graf--p">
   寻找第三方来源的 dork 看起来像这样：
  </p>
  <p class="graf graf--p">
   site: &lt; third party vendor &gt; &lt; Organization name &gt;
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="http://ulogx.com" href="http://ulogx.com" rel="noopener noreferrer" target="_blank">
    Ulogx
   </a>
   总结了一份清单您可以参考。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Codepad
   </li>
  </ul>
  <p class="graf graf--p">
   site: codepad.co “Organization name”
  </p>
  <p class="graf graf--p">
   Codepad 是一个在线编译器/解释器，有时您可以在此处找到硬编码的凭据。您可以查找关键密钥、密码、访问密钥、uuid、特殊URL等。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Gitlab
   </li>
  </ul>
  <p class="graf graf--p">
   inurl: gitlab “Organization name”
  </p>
  <p class="graf graf--p">
   Gitlab 就像 github 一样用于存储源代码。您通常可以在此处找到内部源代码，有时还包括其他敏感信息。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Scribd
   </li>
  </ul>
  <p class="graf graf--p">
   site: scribd.com “Organization name”
  </p>
  <p class="graf graf--p">
   Scribd 通常包含书籍和电子书，但是您有时也能在此找到员工上传的内部文件，其中包含密码或密钥。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Atlassian
   </li>
  </ul>
  <p class="graf graf--p">
   site: * .atlassian.net “Organization name”
  </p>
  <p class="graf graf--p">
   这个Dork 可用于查找 confluence、Jira 和其他可能包含敏感信息的东西。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    NPM
   </li>
  </ul>
  <p class="graf graf--p">
   site: npm.runkit.com “Organization name”
  </p>
  <p class="graf graf--p">
   site: npmjs.com “Organization name”
  </p>
  <p class="graf graf--p">
   这可以用来查找公司使用的 NodeJs 源码。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Libraries IO
   </li>
  </ul>
  <p class="graf graf--p">
   site: libraries.io “Organization name”
  </p>
  <p class="graf graf--p">
   Libraries.io 是一个Web服务，是给开发人员的开源搜索引擎，并提醒开发人员所使用的软件库的新版本。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Coggle
   </li>
  </ul>
  <p class="graf graf--p">
   site: coggle.it “Organization name”
  </p>
  <p class="graf graf--p">
   Coggle 是用于创建思维导图的。于是您可以在这里找到内部流程图，其中可能包含凭证或其他关键信息。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Papaly
   </li>
  </ul>
  <p class="graf graf--p">
   site: papaly.com “Organization name”
  </p>
  <p class="graf graf--p">
   Papaly 用于保存书签和链接。有时您可以找到内部链接、文档和凭证。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Trello
   </li>
  </ul>
  <p class="graf graf--p">
   site: trello.com “Organization name”
  </p>
  <p class="graf graf--p">
   Trello 是基于Web的看板。可用于查找公司的凭证和内部链接。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Prezi
   </li>
  </ul>
  <p class="graf graf--p">
   site: prezi.com “Organization name”
  </p>
  <p class="graf graf--p">
   该平台用于演示，所以可能包含内部链接和可能的凭证。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    JSdeliver
   </li>
  </ul>
  <p class="graf graf--p">
   site: jsdeliver.net “Organization name”
  </p>
  <p class="graf graf--p">
   它是 NPM &amp; Github 的内容分发网络（CDN）。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Pastebin
   </li>
  </ul>
  <p class="graf graf--p">
   site: pastebin.com “Organization name”
  </p>
  <p class="graf graf--p">
   可能包含共享的关键信息。黑客以匿名方式共享信息。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Repl
   </li>
  </ul>
  <p class="graf graf--p">
   Site: repl.it “Organization name”
  </p>
  <p class="graf graf--p">
   Repl是一个在线编译器。您可以在用户脚本中找到硬编码的凭据。有时包含非常有用的信息。不要忽略它。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Gitter
   </li>
  </ul>
  <p class="graf graf--p">
   site: gitter.im “Organization name”
  </p>
  <p class="graf graf--p">
   Gitter 是一个开源消息传递平台。有时您可能会在这里找到包含凭据、内部链接和其他信息的私人消息。
  </p>
  <p class="graf graf--p">
   基本就是这样。如果您有任何新的发现，欢迎分享给大家。别忘了打开创意，创造力是永无止境的。⚪️
  </p>
  <div id="atatags-1611829871-5f646fbc19b68">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-14472" href="https://www.iyouport.org/%e9%bb%91%e5%ae%a2%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8dorks/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Twitter 上共享">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击以在 Twitter 上共享（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-14472" href="https://www.iyouport.org/%e9%bb%91%e5%ae%a2%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8dorks/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Facebook 上共享">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击以在 Facebook 上共享（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-end">
      </li>
     </ul>
    </div>
   </div>
  </div>
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-14472-5f646fbc1a4bf" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=14472&amp;origin=www.iyouport.org&amp;obj_id=161182987-14472-5f646fbc1a4bf" id="like-post-wrapper-161182987-14472-5f646fbc1a4bf">
   <h3 class="sd-title">
    赞过：
   </h3>
   <div class="likes-widget-placeholder post-likes-widget-placeholder" style="height: 55px;">
    <span class="button">
     <span>
      赞
     </span>
    </span>
    <span class="loading">
     正在加载……
    </span>
   </div>
   <span class="sd-text-color">
   </span>
   <a class="sd-link-color">
   </a>
  </div>
  <div class="jp-relatedposts" id="jp-relatedposts">
   <h3 class="jp-relatedposts-headline">
    <em>
     相关
    </em>
   </h3>
  </div>
 </div>
 <div class="entry-footer">
  <ul class="post-tags light-text">
   <li>
    Tagged
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/dorks/" rel="tag">
     dorks
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/googledorking/" rel="tag">
     GoogleDorking
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/hacker/" rel="tag">
     hacker
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/hacktivist/" rel="tag">
     hacktivist
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/technique/" rel="tag">
     technique
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/technology/" rel="tag">
     Technology
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2020-09-18T00:03:40+08:00">
    2020年9月18日
   </time>
   <time class="updated" datetime="2020-09-18T00:03:23+08:00">
    2020年9月18日
   </time>
  </div>
 </div>
</article>

