---
layout: post
title: "如何使用 InVid-WeVerify：数字信息验证的 瑞士军刀 - iYouPort"
date: 2021-04-28T16:04:32+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8-invid-weverify%ef%bc%9a%e6%95%b0%e5%ad%97%e4%bf%a1%e6%81%af%e9%aa%8c%e8%af%81%e7%9a%84-%e7%91%9e%e5%a3%ab%e5%86%9b%e5%88%80/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-15916 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-osint category-67 tag-information-verification tag-investigations tag-osint tag-technology tag-tools tag-verification" id="post-15916">
 <header class="entry-header">
  <h1 class="entry-title">
   如何使用 InVid-WeVerify：数字信息验证的 “瑞士军刀”
  </h1>
 </header>
 <div class="entry-meta">
  <span class="byline">
   <a href="https://www.iyouport.org/author/gabrielfornard/" rel="author" title="由Gabriel Fornard发布">
    Gabriel Fornard
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
   <a href="https://www.iyouport.org/category/%e7%bb%99%e8%a1%8c%e5%8a%a8%e8%80%85%e7%9a%84%e6%8a%a4%e8%ba%ab%e7%ac%a6%e5%92%8c%e6%ad%a6%e5%99%a8/" rel="category tag">
    给行动者的护身符和武器
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-04-29T00:04:32+08:00">
    2021年4月29日
   </time>
   <time class="updated" datetime="2021-01-31T22:59:11+08:00">
    2021年1月31日
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
       非常方便，多种功能集于一身
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="584" data-image-id="0*kKBVxygAi3rKMdDp.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*kKBVxygAi3rKMdDp.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="639" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*kKBVxygAi3rKMdDp.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="584" data-image-id="0*kKBVxygAi3rKMdDp.png" data-recalc-dims="1" data-width="639" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*kKBVxygAi3rKMdDp.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   大赦国际证据实验室向所有开源情报调查人员推荐的主要工具之一是
   <a class="markup--anchor markup--p-anchor" data-href="https://chrome.google.com/webstore/detail/fake-video-news-debunker/mhccpoafgdgbhnjfhkcmgknndkeenfhe?hl=en" href="https://chrome.google.com/webstore/detail/fake-video-news-debunker/mhccpoafgdgbhnjfhkcmgknndkeenfhe?hl=en" rel="noopener" target="_blank">
    Chrome
   </a>
   或
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/AFP-Medialab/invid-weverify-firefox" href="https://github.com/AFP-Medialab/invid-weverify-firefox" rel="noopener" target="_blank">
    Firefox
   </a>
   适用的 InVid-WeVerify 网络浏览器插件。它的构建就像一把事实核查的瑞士军刀，在一个地方包含了多个工具，包括视频的关键帧提取器、照片和视频的元数据提取器、关键帧的反向图像搜索、照片的放大工具，以及 Twitter 高级搜索的整洁界面。
  </p>
  <p class="graf graf--p">
   这篇文章将解释其中许多功能是如何工作的。
  </p>
  <p class="graf graf--p">
   这个工具是由欧盟资助的 InVid（
   <a class="markup--anchor markup--p-anchor" data-href="https://www.invid-project.eu/" href="https://www.invid-project.eu/" rel="noopener" target="_blank">
    In Video Veritas
   </a>
   ）和
   <a class="markup--anchor markup--p-anchor" data-href="https://weverify.eu/" href="https://weverify.eu/" rel="noopener" target="_blank">
    WeVerify
   </a>
   合作的结果。其目标是帮助公民调查者、人权维护者和其他研究人员验证社交网络上的内容。
  </p>
  <p class="graf graf--p">
   安装该工具后，浏览器顶部会出现一个小的启动器图标。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="146" data-image-id="1*pVunFkdcxSDMrgJrtcsK9g.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*pVunFkdcxSDMrgJrtcsK9g.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1148" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*pVunFkdcxSDMrgJrtcsK9g.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="146" data-image-id="1*pVunFkdcxSDMrgJrtcsK9g.png" data-recalc-dims="1" data-width="1148" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*pVunFkdcxSDMrgJrtcsK9g.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     启动 InVid-WeVerify
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   点击后，启动器会给用户提供三个选项：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    打开InVID 启动插件；
   </li>
   <li class="graf graf--li">
    Video Urls 显示网页上的视频网址；
   </li>
   <li class="graf graf--li">
    Image Urls 显示网页上的图像的网址。
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="594" data-image-id="1*stNJYJVdlW6uxA433dKE8w.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*stNJYJVdlW6uxA433dKE8w.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="934" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*stNJYJVdlW6uxA433dKE8w.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="594" data-image-id="1*stNJYJVdlW6uxA433dKE8w.png" data-recalc-dims="1" data-width="934" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*stNJYJVdlW6uxA433dKE8w.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   如果照片或视频被嵌入到新闻网站中，后两个选项会特别有用。当打开 InVid-WeVerify 时，复制并粘贴这些URLs即可使用。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     打开 InVid-WeVerify
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   打开工具后，用户会看到几个标签：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="484" data-image-id="1*79t92yiWD7q6dioRFoUx2A.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*79t92yiWD7q6dioRFoUx2A.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2042" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*79t92yiWD7q6dioRFoUx2A.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="484" data-image-id="1*79t92yiWD7q6dioRFoUx2A.png" data-recalc-dims="1" data-width="2042" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*79t92yiWD7q6dioRFoUx2A.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   下面将讨论这些选项卡中的每一个（Video Rights 选项卡除外，该选项卡针对的是处理版权问题的记者）。
  </p>
  <p class="graf graf--p">
   1、
   <strong class="markup--strong markup--p-strong">
    分析选项卡
   </strong>
   — — 是一个针对 YouTube、Twitter 和 Facebook 公开视频的增强型
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e9%83%bd%e6%98%af%e5%b7%a5%e5%85%b7%ef%bc%8c%e4%bb%8e%e8%87%aa%e6%88%91%e4%bf%9d%e6%8a%a4%e5%88%b0%e6%9c%89%e6%95%88%e5%88%a9%e7%94%a8%e2%80%8a-%e4%ba%a6%e6%ad%a3%e4%ba%a6%e9%82%aa/" href="https://www.iyouport.org/%e9%83%bd%e6%98%af%e5%b7%a5%e5%85%b7%ef%bc%8c%e4%bb%8e%e8%87%aa%e6%88%91%e4%bf%9d%e6%8a%a4%e5%88%b0%e6%9c%89%e6%95%88%e5%88%a9%e7%94%a8%e2%80%8a-%e4%ba%a6%e6%ad%a3%e4%ba%a6%e9%82%aa/" rel="noopener" target="_blank">
    元数据
   </a>
   查看器。它允许用户检索背景信息、位置（如果检测到）、最有趣的评论，并应用
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e6%90%9c%e5%9b%be%e5%8a%9f%e8%83%bd%e5%93%aa%e5%ae%b6%e5%bc%ba%ef%bc%9f%e5%9b%be%e5%83%8f%e9%aa%8c%e8%af%81%e6%96%b9%e6%b3%95%e7%9a%84%e8%83%bd%e5%8a%9b%e5%af%b9%e6%af%94/" href="https://www.iyouport.org/%e6%90%9c%e5%9b%be%e5%8a%9f%e8%83%bd%e5%93%aa%e5%ae%b6%e5%bc%ba%ef%bc%9f%e5%9b%be%e5%83%8f%e9%aa%8c%e8%af%81%e6%96%b9%e6%b3%95%e7%9a%84%e8%83%bd%e5%8a%9b%e5%af%b9%e6%af%94/" rel="noopener" target="_blank">
    反向图像搜索
   </a>
   检查发布该视频的推文（在YouTube上）。对于 Facebook，用户需要登录 Facebook 账户才能处理链接。
  </p>
  <p class="graf graf--p">
   2、
   <strong class="markup--strong markup--p-strong">
    关键帧选项卡
   </strong>
   — — 允许用户复制视频网址（来自 YouTube、Twitter、Facebook、Daily Motion 或 Dropbox）或上传本地视频文件（mp4、webm、avi、mov、wmv、ogv、mpg、flv 和 mkv 格式都可以），以便将视频分割成关键帧。一旦被分割，关键帧可以通过点击 Google 图像搜索或通过菜单（右键点击）搜索 Google、Yandex、Tineye、Bing、Karma Decay（针对 Reddit）和百度图像。
  </p>
  <p class="graf graf--p">
   3、
   <strong class="markup--strong markup--p-strong">
    YouTube 缩略图选项
   </strong>
   — — 允许用户在 Google、Bing、Tineye 或 Yandex Images 上快速触发反向图像搜索，并从 YouTube 视频中提取四个缩略图。最多四个（根据可用缩略图的数量）会在浏览器中自动打开反向图像搜索的结果，同时四个缩略图也会显示在插件页面中。这个选项卡与分析选项卡可以做的事情有很多，如果用户需要查找一个 YouTube 视频是否曾经被发布过，那么这个选项卡是非常快速高效的。
  </p>
  <p class="graf graf--p">
   4、
   <strong class="markup--strong markup--p-strong">
    Twitter 搜索选项卡
   </strong>
   — — 这是一个增强的 Twitter 关键字或标签的
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e4%bb%8e%e6%8e%a8%e7%89%b9%e4%b8%ad%e6%8c%96%e6%8e%98%e7%9c%9f%e7%9b%b8%e4%b8%8d%e9%9c%80%e8%a6%81%e5%a4%aa%e5%a4%8d%e6%9d%82%e7%9a%84%e5%b7%a5%e5%85%b7%ef%bc%9a%e4%b8%80%e4%b8%aa%e5%b8%b8%e7%94%a8/" href="https://www.iyouport.org/%e4%bb%8e%e6%8e%a8%e7%89%b9%e4%b8%ad%e6%8c%96%e6%8e%98%e7%9c%9f%e7%9b%b8%e4%b8%8d%e9%9c%80%e8%a6%81%e5%a4%aa%e5%a4%8d%e6%9d%82%e7%9a%84%e5%b7%a5%e5%85%b7%ef%bc%9a%e4%b8%80%e4%b8%aa%e5%b8%b8%e7%94%a8/" rel="noopener" target="_blank">
    高级搜索
   </a>
   ，运算符可以将查询的时间间隔缩小到一分钟之内。它自动将日历日期、小时和分钟翻译成unix
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e6%b7%b1%e6%8c%96%e6%8e%a8%e7%89%b9%ef%bc%9a%e5%a6%82%e4%bd%95%e4%bb%8e%e6%8e%a8%e6%96%87%e4%b8%ad%e6%8f%90%e5%8f%96%e5%87%86%e7%a1%ae%e7%9a%84%e5%85%83%e6%95%b0%e6%8d%ae%ef%bc%9f/" href="https://www.iyouport.org/%e6%b7%b1%e6%8c%96%e6%8e%a8%e7%89%b9%ef%bc%9a%e5%a6%82%e4%bd%95%e4%bb%8e%e6%8e%a8%e6%96%87%e4%b8%ad%e6%8f%90%e5%8f%96%e5%87%86%e7%a1%ae%e7%9a%84%e5%85%83%e6%95%b0%e6%8d%ae%ef%bc%9f/" rel="noopener" target="_blank">
    时间戳
   </a>
   ，以方便查询，例如，在
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e7%aa%81%e5%8f%91%e4%ba%8b%e4%bb%b6%e6%9d%a5%e4%ba%86%ef%bc%8c%e5%a6%82%e4%bd%95%e8%bf%9b%e8%a1%8c%e5%85%a8%e9%9d%a2%e7%9a%84%e8%a7%86%e9%a2%91%e4%bf%a1%e6%81%af%e9%87%87%e9%9b%86%ef%bc%9fosint/" href="https://www.iyouport.org/%e7%aa%81%e5%8f%91%e4%ba%8b%e4%bb%b6%e6%9d%a5%e4%ba%86%ef%bc%8c%e5%a6%82%e4%bd%95%e8%bf%9b%e8%a1%8c%e5%85%a8%e9%9d%a2%e7%9a%84%e8%a7%86%e9%a2%91%e4%bf%a1%e6%81%af%e9%87%87%e9%9b%86%ef%bc%9fosint/" rel="noopener" target="_blank">
    突发事件
   </a>
   刚发生后的时间范围内出现的第一张图片或第一个视频。该选项还包括 Twitter 高级搜索的其他功能，如地理编码、附近*、来自*、语言和各种过滤操作符。
  </p>
  <p class="graf graf--p">
   5、
   <strong class="markup--strong markup--p-strong">
    “放大镜” 选项卡
   </strong>
   — — 允许用户通过网址显示图像，并在图像上放大或应用放大镜，以帮助解读和阅读图像中
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%ae%a9%e6%a8%a1%e7%b3%8a%e5%9b%be%e5%83%8f%e5%8f%98%e6%b8%85%e6%99%b0%ef%bc%9f-%e5%bc%80%e6%ba%90%e6%83%85%e6%8a%a5%e5%88%9d%e7%ba%a7%e5%a4%84%e7%90%86%e5%b7%a5%e5%85%b7/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%ae%a9%e6%a8%a1%e7%b3%8a%e5%9b%be%e5%83%8f%e5%8f%98%e6%b8%85%e6%99%b0%ef%bc%9f-%e5%bc%80%e6%ba%90%e6%83%85%e6%8a%a5%e5%88%9d%e7%ba%a7%e5%a4%84%e7%90%86%e5%b7%a5%e5%85%b7/" rel="noopener" target="_blank">
    难以看到的细节
   </a>
   — — 如汽车牌照、军徽、标志和横幅。用户可以输入图像的网址，或者使用本地文件按钮从本地上传图像。然后你就可以谷歌、Yandex、Tineye 和百度对其进行反向图像搜索，或使用下面解释的图像取证选项。该选项卡中的其他工具包括锐化、图像翻转和裁剪。
  </p>
  <p class="graf graf--p">
   6、
   <strong class="markup--strong markup--p-strong">
    元数据选项卡
   </strong>
   — — 允许用户查看 jpeg 图片的Exif数据，或者 mp4/m4v 格式的视频的元数据。这可以通过一个链接或一个本地文件来实现。
  </p>
  <p class="graf graf--p">
   7、
   <strong class="markup--strong markup--p-strong">
    取证选项卡
   </strong>
   — — 提供了八种不同的图像滤波，帮助用户检测数字图像
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%bf%ab%e9%80%9f%e5%8f%91%e7%8e%b0%e8%a2%abps%e8%bf%87%e7%9a%84%ef%bc%88%e7%be%8e%e5%a5%b3%ef%bc%89%e7%85%a7%e7%89%87%ef%bc%9f/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%bf%ab%e9%80%9f%e5%8f%91%e7%8e%b0%e8%a2%abps%e8%bf%87%e7%9a%84%ef%bc%88%e7%be%8e%e5%a5%b3%ef%bc%89%e7%85%a7%e7%89%87%ef%bc%9f/" rel="noopener" target="_blank">
    被篡改的痕迹
   </a>
   ：例如使用 Photoshop 编辑软件的篡改。这需要高级的图像滤波工作知识，所以不建议开源调查的初学者使用该选项。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     情境菜单
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   InVid-WeVerify 插件还为您的浏览器带来一个背景菜单。当在线时，右键点击图片或视频网址即可激活该插件。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="562" data-image-id="1*tL1Uqmi_EeBLrfUg2H_vhg.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*tL1Uqmi_EeBLrfUg2H_vhg.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1484" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*tL1Uqmi_EeBLrfUg2H_vhg.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="562" data-image-id="1*tL1Uqmi_EeBLrfUg2H_vhg.png" data-recalc-dims="1" data-width="1484" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*tL1Uqmi_EeBLrfUg2H_vhg.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   该菜单允许用户在静态图像或 YouTube 视频链接上触发该插件。在图像上，右键单击将建议在图像放大镜中打开图片，以便更仔细地检查它，或对该图像进行取证分析或反向图像搜索。在一个视频链接上，右键将提议 InVID-WeVerify 视频分析或 YouTube 缩略图反向搜索。
  </p>
  <p class="graf graf--p">
   来试试看吧。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://citizenevidence.org/2019/12/11/how-to-use-invid-the-swiss-army-knife-of-digital-verification/" href="https://citizenevidence.org/2019/12/11/how-to-use-invid-the-swiss-army-knife-of-digital-verification/" rel="noopener" target="_blank">
    How to: Use InVid-WeVerify — the ‘Swiss Army Knife’ of Digital Verification
   </a>
  </p>
  <div id="atatags-1611829871-60afa29c97cd6">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-15916" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8-invid-weverify%ef%bc%9a%e6%95%b0%e5%ad%97%e4%bf%a1%e6%81%af%e9%aa%8c%e8%af%81%e7%9a%84-%e7%91%9e%e5%a3%ab%e5%86%9b%e5%88%80/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-15916" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8-invid-weverify%ef%bc%9a%e6%95%b0%e5%ad%97%e4%bf%a1%e6%81%af%e9%aa%8c%e8%af%81%e7%9a%84-%e7%91%9e%e5%a3%ab%e5%86%9b%e5%88%80/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到 Facebook （在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-end">
      </li>
     </ul>
    </div>
   </div>
  </div>
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-15916-60afa29c982a2" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=15916&amp;origin=www.iyouport.org&amp;obj_id=161182987-15916-60afa29c982a2" id="like-post-wrapper-161182987-15916-60afa29c982a2">
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
    <a href="https://www.iyouport.org/tag/information-verification/" rel="tag">
     Information verification
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/investigations/" rel="tag">
     Investigations
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/osint/" rel="tag">
     OSINT
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/technology/" rel="tag">
     Technology
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/tools/" rel="tag">
     tools
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/verification/" rel="tag">
     verification
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-04-29T00:04:32+08:00">
    2021年4月29日
   </time>
   <time class="updated" datetime="2021-01-31T22:59:11+08:00">
    2021年1月31日
   </time>
  </div>
 </div>
</article>

