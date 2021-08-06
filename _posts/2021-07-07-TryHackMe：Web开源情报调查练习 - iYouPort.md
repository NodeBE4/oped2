---
layout: post
title: "TryHackMe：Web开源情报调查练习 - iYouPort"
date: 2021-07-07T16:03:17+00:00
author: iYouPort
from: https://www.iyouport.org/tryhackme%ef%bc%9aweb%e5%bc%80%e6%ba%90%e6%83%85%e6%8a%a5%e8%b0%83%e6%9f%a5%e7%bb%83%e4%b9%a0/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16475 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-osint tag-hacking tag-osint tag-technology tag-tryhackme" id="post-16475">
 <header class="entry-header">
  <h1 class="entry-title">
   TryHackMe：Web开源情报调查练习
  </h1>
 </header>
 <div class="entry-meta">
  <span class="byline">
   <a href="https://www.iyouport.org/author/gabrielfornard/" rel="author" title="文章作者 Gabriel Fornard">
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
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-07-08T00:03:17+08:00">
    2021年7月8日
   </time>
   <time class="updated" datetime="2021-08-06T15:20:10+08:00">
    2021年8月6日
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
       亲自尝试一下很重要
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1084" data-image-id="1*Dy99y7VJLaXWUD-tsvLVaQ.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Dy99y7VJLaXWUD-tsvLVaQ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2696" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Dy99y7VJLaXWUD-tsvLVaQ.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1084" data-image-id="1*Dy99y7VJLaXWUD-tsvLVaQ.png" data-recalc-dims="1" data-width="2696" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Dy99y7VJLaXWUD-tsvLVaQ.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   开源情报收集对于安全研究人员、道德黑客、渗透测试人员、安全分析师，当然还有黑帽黑客来说，都是至关重要的。开源情报有助于收集和分析来自公开可用资源的信息，以达到情报目的。
  </p>
  <p class="graf graf--p">
   为了了解开源情报收集是什么样的，本文将通过
   <a class="markup--anchor markup--p-anchor" data-href="https://tryhackme.com/room/webosint" href="https://tryhackme.com/room/webosint" rel="noopener" target="_blank">
    TryHackMe 的 “Web OSINT”
   </a>
   来尝试一个调查。这个平台的目标是收集与网站相关的信息。
  </p>
  <p class="graf graf--p">
   P.S：强烈建议大家亲自尝试一下，您将能够提升您的侦察技能，填补您缺乏的空白。
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    目标：
   </strong>
  </p>
  <p class="graf graf--p">
   使用不同的工具收集与目标网站相关的一切信息。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     任务1：当一个网站不存在时
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   在寻找与企业相关的所需信息时，人们通常会使用google。考虑一个场景，您必须找到一些信息，而目标网站已经不存在了。您会怎么做？当您在这里尝试解决这个特殊的挑战时，您就会知道这一点。我们必须收集一些与一个名为 “RepublicOfKoffee.com” 的网站相关的数据，当试图导航到这个网站时，google搜索显示以下内容：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="623" data-image-id="0*zwx5UGGootWUQLB2.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zwx5UGGootWUQLB2.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1154" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zwx5UGGootWUQLB2.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="623" data-image-id="0*zwx5UGGootWUQLB2.png" data-recalc-dims="1" data-width="1154" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zwx5UGGootWUQLB2.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   该网站不存在，但即使它不存在，您也可能会调出一些信息。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     任务2: 域名注册
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   直接搜索目标网站没有找到任何信息，但还是可以通过一个叫
   <a class="markup--anchor markup--p-anchor" data-href="https://lookup.icann.org/lookup" href="https://lookup.icann.org/lookup" rel="noopener" target="_blank">
    lookup.icann.org
   </a>
   的工具找到目标网站的相关信息。还有很多其他的工具也可以从中提取出一些信息，比如域名的主人是谁、名称服务器、电话号码、电子邮件地址、城市/国家等。
  </p>
  <p class="graf graf--p">
   导航到上面提到的在线工具，找到所需的信息，即 网站注册的公司名称、电话号码、名称服务器、注册人的名字和注册人所在的国家。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="503" data-image-id="0*IYLoCUOjW48J2khE.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*IYLoCUOjW48J2khE.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="959" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*IYLoCUOjW48J2khE.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="503" data-image-id="0*IYLoCUOjW48J2khE.png" data-recalc-dims="1" data-width="959" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*IYLoCUOjW48J2khE.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   从这里了解到，该域名是由一家叫 NAMECHEAP INC 的公司所有的。
  </p>
  <p class="graf graf--p">
   同样，您也可以找到电话号码、名称服务器、注册人的名字和注册人的国家，如下图所示：
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 1067px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="419" data-image-id="0*bCOxMzkva9wjvkep.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*bCOxMzkva9wjvkep.png?resize=1067%2C328&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1363" height="328" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*bCOxMzkva9wjvkep.png?resize=1067%2C328&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1067"/>
     <noscript>
      <img alt="" class="graf-image" data-height="419" data-image-id="0*bCOxMzkva9wjvkep.png" data-recalc-dims="1" data-width="1363" height="328" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*bCOxMzkva9wjvkep.png?resize=1067%2C328&amp;ssl=1" width="1067"/>
     </noscript>
     <figcaption class="wp-caption-text">
      注册的电话号码
     </figcaption>
    </figure>
   </p>
  </figure>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 504px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="262" data-image-id="0*RMo1P2Epv-i6aIot.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*RMo1P2Epv-i6aIot.png?resize=504%2C262&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="504" height="262" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*RMo1P2Epv-i6aIot.png?resize=504%2C262&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="504"/>
     <noscript>
      <img alt="" class="graf-image" data-height="262" data-image-id="0*RMo1P2Epv-i6aIot.png" data-recalc-dims="1" data-width="504" height="262" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*RMo1P2Epv-i6aIot.png?resize=504%2C262&amp;ssl=1" width="504"/>
     </noscript>
     <figcaption class="wp-caption-text">
      名称服务器
     </figcaption>
    </figure>
   </p>
  </figure>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 1067px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="333" data-image-id="0*Di8O4ldnCCLcSQwF.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*Di8O4ldnCCLcSQwF.png?resize=1067%2C262&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1351" height="262" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*Di8O4ldnCCLcSQwF.png?resize=1067%2C262&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1067"/>
     <noscript>
      <img alt="" class="graf-image" data-height="333" data-image-id="0*Di8O4ldnCCLcSQwF.png" data-recalc-dims="1" data-width="1351" height="262" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*Di8O4ldnCCLcSQwF.png?resize=1067%2C262&amp;ssl=1" width="1067"/>
     </noscript>
     <figcaption class="wp-caption-text">
      注册人
     </figcaption>
    </figure>
   </p>
  </figure>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 1067px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="88" data-image-id="0*j18FND54iBo3C5h4.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*j18FND54iBo3C5h4.png?resize=1067%2C69&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1344" height="69" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*j18FND54iBo3C5h4.png?resize=1067%2C69&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1067"/>
     <noscript>
      <img alt="" class="graf-image" data-height="88" data-image-id="0*j18FND54iBo3C5h4.png" data-recalc-dims="1" data-width="1344" height="69" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*j18FND54iBo3C5h4.png?resize=1067%2C69&amp;ssl=1" width="1067"/>
     </noscript>
     <figcaption class="wp-caption-text">
      注册国家
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     任务3：目标网站过去的幽灵
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在，您已经从公开的工具中提取了与目标网站相关的基本信息。现在您就可以尝试找出网站的样子，即使网站已经不存在。
  </p>
  <p class="graf graf--p">
   这里要利用的是
   <a class="markup--anchor markup--p-anchor" data-href="https://web.archive.org/" href="https://web.archive.org/" rel="noopener" target="_blank">
    waybackmachine
   </a>
   ，它保存着一年中不同时期的网站档案。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="621" data-image-id="0*bsPVJeUixg-krIdF.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*bsPVJeUixg-krIdF.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1365" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*bsPVJeUixg-krIdF.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="621" data-image-id="0*bsPVJeUixg-krIdF.png" data-recalc-dims="1" data-width="1365" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*bsPVJeUixg-krIdF.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   需要找到目标网站上第一个博客的作者姓名。导航到时光机器时间轴上找到的第一个存档：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="694" data-image-id="0*96R6CG1MQGt1gc1f.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*96R6CG1MQGt1gc1f.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1364" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*96R6CG1MQGt1gc1f.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="694" data-image-id="0*96R6CG1MQGt1gc1f.png" data-recalc-dims="1" data-width="1364" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*96R6CG1MQGt1gc1f.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   博客作者：Steve
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="697" data-image-id="0*loEzZosslLhNiUUT.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*loEzZosslLhNiUUT.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1355" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*loEzZosslLhNiUUT.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="697" data-image-id="0*loEzZosslLhNiUUT.png" data-recalc-dims="1" data-width="1355" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*loEzZosslLhNiUUT.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   接下来需要找到作者写作的国家。您已经知道了博客中提到的城市名称和地方，做一点研究就能找到地点  — — 韩国光州。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="608" data-image-id="0*z1BIZn1s4Var6Q8m.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*z1BIZn1s4Var6Q8m.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="480" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*z1BIZn1s4Var6Q8m.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="608" data-image-id="0*z1BIZn1s4Var6Q8m.png" data-recalc-dims="1" data-width="480" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*z1BIZn1s4Var6Q8m.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   导航到下一个博客，需要在其中找到作者所参观的寺庙的名称：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="663" data-image-id="0*i3CnOG47HK95Nsjx.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*i3CnOG47HK95Nsjx.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="825" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*i3CnOG47HK95Nsjx.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="663" data-image-id="0*i3CnOG47HK95Nsjx.png" data-recalc-dims="1" data-width="825" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*i3CnOG47HK95Nsjx.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   对博客中提到的地方进行一些检查就很容易发现寺庙名是：证心寺。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="655" data-image-id="0*sL7X98zrvXcNnFBK.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*sL7X98zrvXcNnFBK.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="751" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*sL7X98zrvXcNnFBK.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="655" data-image-id="0*sL7X98zrvXcNnFBK.png" data-recalc-dims="1" data-width="751" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*sL7X98zrvXcNnFBK.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     任务4：深入研究DNS
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   到目前为止，您已经收集到了足够的信息，可以用来得出一些结论。现在您需要找到更多与网站相关的技术细节，如IP地址、网站使用的主机类型。
  </p>
  <p class="graf graf--p">
   使用 ViewDns 信息，我们可以收集到很多与网站相关的信息。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="657" data-image-id="0*GEbrMOoiyfiKz2rW.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*GEbrMOoiyfiKz2rW.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1019" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*GEbrMOoiyfiKz2rW.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="657" data-image-id="0*GEbrMOoiyfiKz2rW.png" data-recalc-dims="1" data-width="1019" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*GEbrMOoiyfiKz2rW.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   接下来需要查找的是截至2016年10月的 RepublicOfKoffee.com 的IP地址。使用IP历史记录提取所需的信息：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="449" data-image-id="0*zDIlMnLBnIUzx7da.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zDIlMnLBnIUzx7da.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1015" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zDIlMnLBnIUzx7da.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="449" data-image-id="0*zDIlMnLBnIUzx7da.png" data-recalc-dims="1" data-width="1015" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zDIlMnLBnIUzx7da.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   现在您需要找出目标网站使用的托管服务。使用反向查找来达到这个目的。有一长串的域名与之前找到的IP相关联。这说明目标网站所有者使用的是共享托管服务，因为它的成本比专用托管服务低很多。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="656" data-image-id="0*T02MkeaksjnuJ5iU.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*T02MkeaksjnuJ5iU.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="694" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*T02MkeaksjnuJ5iU.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="656" data-image-id="0*T02MkeaksjnuJ5iU.png" data-recalc-dims="1" data-width="694" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*T02MkeaksjnuJ5iU.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   回溯IP历史，在该域名历史上，IP地址变化过4次。这就回答了这个任务的最后一个答案。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     任务5
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在有一个新的目标域名 heat.net。需要找到辅助名称服务器：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="686" data-image-id="0*HSuCmSVD1RXtpUgq.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*HSuCmSVD1RXtpUgq.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1052" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*HSuCmSVD1RXtpUgq.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="686" data-image-id="0*HSuCmSVD1RXtpUgq.png" data-recalc-dims="1" data-width="1052" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*HSuCmSVD1RXtpUgq.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   截至2011年12月列出的该域的IP地址：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="346" data-image-id="0*T6s3sdLsX-Wze_bT.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*T6s3sdLsX-Wze_bT.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1000" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*T6s3sdLsX-Wze_bT.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="346" data-image-id="0*T6s3sdLsX-Wze_bT.png" data-recalc-dims="1" data-width="1000" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*T6s3sdLsX-Wze_bT.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   域名所有者正在使用的托管服务
  </p>
  <p class="graf graf--p">
   域名所有者正在使用的共享主机服务
  </p>
  <p class="graf graf--p">
   互联网档案馆捕获的第一个网站的日期
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="695" data-image-id="0*SZjqpCkdYt0Lm8qu.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*SZjqpCkdYt0Lm8qu.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1364" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*SZjqpCkdYt0Lm8qu.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="695" data-image-id="0*SZjqpCkdYt0Lm8qu.png" data-recalc-dims="1" data-width="1364" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*SZjqpCkdYt0Lm8qu.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   第一段的第一句摘自2001年的最终捕获：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="564" data-image-id="0*I1H4fGDx53fhYWov.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*I1H4fGDx53fhYWov.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="737" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*I1H4fGDx53fhYWov.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="564" data-image-id="0*I1H4fGDx53fhYWov.png" data-recalc-dims="1" data-width="737" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*I1H4fGDx53fhYWov.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   SegaSoft是负责该网站原始版本的公司。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="667" data-image-id="0*lCTNQhJ8R-jciSDZ.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*lCTNQhJ8R-jciSDZ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1150" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*lCTNQhJ8R-jciSDZ.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="667" data-image-id="0*lCTNQhJ8R-jciSDZ.png" data-recalc-dims="1" data-width="1150" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*lCTNQhJ8R-jciSDZ.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     任务6
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   要找到规律，必须考虑被调查对象的每一个方面。长时间休眠的网站，在重新上线后，会引起不同的关注。要验证网站是否合法，需要记住一些要点，如网站的语言、用户界面和设计等。
  </p>
  <p class="graf graf--p">
   有些时候开发人员会在源代码中留下注释，可以通过分析这些注释来收集更多关于目标的信息。外链和内链可以用来将信息连接起来。
  </p>
  <p class="graf graf--p">
   在这里，您将被指示导航到一个链接，并找出以下内容。
  </p>
  <p class="graf graf--p">
   本案例中的内链数：5
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="691" data-image-id="0*X2m8LfCaDZoK4FDQ.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*X2m8LfCaDZoK4FDQ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="931" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*X2m8LfCaDZoK4FDQ.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="691" data-image-id="0*X2m8LfCaDZoK4FDQ.png" data-recalc-dims="1" data-width="931" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*X2m8LfCaDZoK4FDQ.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   外链数：1
  </p>
  <p class="graf graf--p">
   外链地址：purchase.org
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="700" data-image-id="0*RkQICgjCXvWY13ML.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*RkQICgjCXvWY13ML.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1354" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*RkQICgjCXvWY13ML.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="700" data-image-id="0*RkQICgjCXvWY13ML.png" data-recalc-dims="1" data-width="1354" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*RkQICgjCXvWY13ML.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   链接到该网站的 Google Analytics 代码：
  </p>
  <p class="graf graf--p">
   使用文章上的查看页面源代码，并找到如下所示的Google Analytics 代码
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="661" data-image-id="0*zOtCREHz3BNUCXgr.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zOtCREHz3BNUCXgr.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1177" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zOtCREHz3BNUCXgr.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="661" data-image-id="0*zOtCREHz3BNUCXgr.png" data-recalc-dims="1" data-width="1177" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*zOtCREHz3BNUCXgr.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   为了查明此 Google analytic 代码是否已在其他任何网站上用过，使用
   <a class="markup--anchor markup--p-anchor" data-href="https://www.nerdydata.com/" href="https://www.nerdydata.com/" rel="noopener" target="_blank">
    nerdydata.com
   </a>
   。该在线工具将搜索网页，并告诉您是否在其他任何网站中找到了该查询；
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="542" data-image-id="0*lj0DVh3kOiD_UhbX.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*lj0DVh3kOiD_UhbX.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1165" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*lj0DVh3kOiD_UhbX.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="542" data-image-id="0*lj0DVh3kOiD_UhbX.png" data-recalc-dims="1" data-width="1165" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*lj0DVh3kOiD_UhbX.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   这个案例中没有找到任何其他网站。您可以通过查看href的内容来寻找此类链接。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     任务7
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   在这个任务中，您需要找到目标网站即 heat.net 和外链之间的联系。重新查看IP历史工具，你会发现外链(purchase.org)与 heat.net 是相同的所有者。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="509" data-image-id="0*O7W_vJoYh8RBX66y.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*O7W_vJoYh8RBX66y.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1004" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*O7W_vJoYh8RBX66y.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="509" data-image-id="0*O7W_vJoYh8RBX66y.png" data-recalc-dims="1" data-width="1004" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*O7W_vJoYh8RBX66y.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     收尾工作
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   如前，您发现这两个网站的所有权是相同的。当看到 heat.net 时，并没有发现该网站非常有趣或吸引人，也没有产生那么多的流量，而另一方面，purchase.org 是一个电子商务网站，可能比 heat.net 产生更多的收入。从这里您可以得出的结论是，业主正在运行一个私人博客网络(PBN)，以说服搜索引擎将他们的主网站排到更高的位置，这是一种常用的SEO优化手段。也就是说，Heat.net 只是为了诱骗搜索引擎将 purchase.org 排到更高的位置。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://www.secjuice.com/tryhackmeweb-osint/" href="https://www.secjuice.com/tryhackmeweb-osint/" rel="noopener" target="_blank">
    TryHackMe: Web OSINT Writeup
   </a>
  </p>
  <div id="atatags-1611829871-610d3c74d925d">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16475" href="https://www.iyouport.org/tryhackme%ef%bc%9aweb%e5%bc%80%e6%ba%90%e6%83%85%e6%8a%a5%e8%b0%83%e6%9f%a5%e7%bb%83%e4%b9%a0/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16475" href="https://www.iyouport.org/tryhackme%ef%bc%9aweb%e5%bc%80%e6%ba%90%e6%83%85%e6%8a%a5%e8%b0%83%e6%9f%a5%e7%bb%83%e4%b9%a0/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16475-610d3c74d9b3c" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16475&amp;origin=www.iyouport.org&amp;obj_id=161182987-16475-610d3c74d9b3c" data-title="点赞或转载" id="like-post-wrapper-161182987-16475-610d3c74d9b3c">
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
    <a href="https://www.iyouport.org/tag/hacking/" rel="tag">
     hacking
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
    <a href="https://www.iyouport.org/tag/tryhackme/" rel="tag">
     TryHackMe
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-07-08T00:03:17+08:00">
    2021年7月8日
   </time>
   <time class="updated" datetime="2021-08-06T15:20:10+08:00">
    2021年8月6日
   </time>
  </div>
 </div>
</article>

