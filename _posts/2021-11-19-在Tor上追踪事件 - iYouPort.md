---
layout: post
title: "在Tor上追踪事件 - iYouPort"
date: 2021-11-19T08:48:22+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%9c%a8tor%e4%b8%8a%e8%bf%bd%e8%b8%aa%e4%ba%8b%e4%bb%b6/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-17389 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-osint tag-investigative tag-osint tag-tips tag-tor" id="post-17389">
 <header class="entry-header">
  <h1 class="entry-title">
   在Tor上追踪事件
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
   <time class="entry-date published" datetime="2021-11-19T16:48:22+08:00">
    2021年11月19日
   </time>
   <time class="updated" datetime="2021-12-22T17:04:05+08:00">
    2021年12月22日
   </time>
  </span>
  <span class="word-count">
   1 Minute
  </span>
 </div>
 <div class="entry-content">
  <ul>
   <li>
    <span style="color: #00ccff;">
     <em>
      <strong>
       以及帮您建立最佳的访问路由。
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-535-728" href="https://i0.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F107c137b-04cb-49b9-9fa7-04735fe680b2_1067x535.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/107c137b-04cb-49b9-9fa7-04735fe680b2_1067x535.png","fullscreen":null,"height":535,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F107c137b-04cb-49b9-9fa7-04735fe680b2_1067x535.png?resize=728%2C535&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="535" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F107c137b-04cb-49b9-9fa7-04735fe680b2_1067x535.png?resize=728%2C535&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/107c137b-04cb-49b9-9fa7-04735fe680b2_1067x535.png","fullscreen":null,"height":535,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="535" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F107c137b-04cb-49b9-9fa7-04735fe680b2_1067x535.png?resize=728%2C535&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   TOR是当今最流行的 “暗网”。它因与非法活动有关而闻名，如销售毒品、武器等的论坛和供应商。然而，TOR也有合法的用途，例如避免基于国家的审查制度，或在有争议的环境中进行匿名交流，以获得重要信息。
  </p>
  <p>
   虽然大多数学习和访问TOR的人只是直接使用TOR浏览器，并使用搜索引擎、wiki/index或已知的 .onion 地址，但依旧可以通过退一步查看网络本身来了解世界上正在发生的事。幸运的是，TOR的网络细节是公开的，人们可以查看和分析。
  </p>
  <h3>
   <strong>
    TOR网络
   </strong>
  </h3>
  <p>
   先简单介绍一下TOR网络的工作原理。它是由一系列志愿者维护的中继站组成的，将流量传送到目的地并返回。客户端将连接到所谓的 “入口节点”，通过一系列的 “中继”，然后通过所谓的 “出口节点” 。术语在不同的参考文献中可能有所不同，但只要您理解这个概念，就会产生共鸣，为什么它类似于洋葱上的层（因此而得名）。
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-551-728" href="https://i0.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F9e474096-a1d5-4667-b152-423e600417c0_1067x551.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/9e474096-a1d5-4667-b152-423e600417c0_1067x551.png","fullscreen":null,"height":551,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F9e474096-a1d5-4667-b152-423e600417c0_1067x551.png?resize=728%2C551&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="551" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F9e474096-a1d5-4667-b152-423e600417c0_1067x551.png?resize=728%2C551&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/9e474096-a1d5-4667-b152-423e600417c0_1067x551.png","fullscreen":null,"height":551,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="551" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F9e474096-a1d5-4667-b152-423e600417c0_1067x551.png?resize=728%2C551&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   现在您已经对流量有了基本的了解，下面来看看宏观的网络活动。
  </p>
  <h3>
   <strong>
    网络活动和指标
   </strong>
  </h3>
  <p>
   TOR项目发布了一个网站，让您可以看一下网络的指标。这对于了解网络活动的峰谷波动是很有用的。分析这点的一个关键收获是与地缘政治事件的相关性。当世界上出现内乱或重大事件时，您经常会看到连接到TOR网络的人出现高峰。他们在网络上做什么的确切情况无法通过宏观网络分析查看，但推论对评估还是很有用的。
  </p>
  <div class="captioned-image-container">
   <figure>
    <p>
     <figure class="wp-caption aligncenter" style="width: 728px">
      <img alt="" class="sizing-default jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/b2a4409f-fd87-41d6-bcf8-d3862387b0c2_1067x1123.png","fullscreen":null,"height":1123,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fb2a4409f-fd87-41d6-bcf8-d3862387b0c2_1067x1123.png?resize=728%2C1123&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="1123" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fb2a4409f-fd87-41d6-bcf8-d3862387b0c2_1067x1123.png?resize=728%2C1123&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
      <noscript>
       <img alt="" class="sizing-default" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/b2a4409f-fd87-41d6-bcf8-d3862387b0c2_1067x1123.png","fullscreen":null,"height":1123,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="1123" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fb2a4409f-fd87-41d6-bcf8-d3862387b0c2_1067x1123.png?resize=728%2C1123&amp;ssl=1" width="728"/>
      </noscript>
      <figcaption class="wp-caption-text">
       TOR Metrics (
       <a href="https://metrics.torproject.org/" rel="noopener" target="_blank">
        https://metrics.torproject.org/
       </a>
       )
      </figcaption>
     </figure>
    </p>
   </figure>
  </div>
  <h3>
   <strong>
    用户活动
   </strong>
  </h3>
  <p>
   对于将活动高峰与世界各地的突发事件联系起来，第一个有用的指标是关于有多少用户正在访问该服务。点击 “用户” 选项，可以看到有多少人正在连接到TOR，以及来自哪个国家。当世界上有地缘政治事件发生时，请考虑这一点。它可以推断出一个国家内离散的互联网通信和访问的热门程度，以及在一个有争议的环境中是否有渠道或机会可能存在与民众沟通。
  </p>
  <div class="captioned-image-container">
   <figure>
    <p>
     <figure class="wp-caption aligncenter" style="width: 682px">
      <img alt="" class="sizing-default jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/0baf500e-60ec-4fc0-83b7-f6680e87d48a_682x740.jpeg","fullscreen":null,"height":740,"width":682,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0baf500e-60ec-4fc0-83b7-f6680e87d48a_682x740.jpeg?resize=682%2C740&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="740" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0baf500e-60ec-4fc0-83b7-f6680e87d48a_682x740.jpeg?resize=682%2C740&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="682"/>
      <noscript>
       <img alt="" class="sizing-default" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/0baf500e-60ec-4fc0-83b7-f6680e87d48a_682x740.jpeg","fullscreen":null,"height":740,"width":682,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="740" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0baf500e-60ec-4fc0-83b7-f6680e87d48a_682x740.jpeg?resize=682%2C740&amp;ssl=1" width="682"/>
      </noscript>
      <figcaption class="wp-caption-text">
       Filter options for TOR Users (
       <a href="https://metrics.torproject.org/userstats-relay-country.html" rel="noopener" target="_blank">
        https://metrics.torproject.org/userstats-relay-country.html)
       </a>
      </figcaption>
     </figure>
    </p>
   </figure>
  </div>
  <h3>
   <strong>
    使用案例 — 阿富汗2021年
   </strong>
  </h3>
  <p>
   下面分析的是2020年1月至2021年9月的TOR用户活动，以了解TOR活动在阿富汗境内随时间推移的变化。IP位置来自于中继对客户IP的解析，因为他们通过中继提供了一个地理数据库。与VPN连接的客户有可能混淆这一点，但在规模层面上不太可能，所以依旧有能力依靠这些指标进行分析。
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-571-728" href="https://i1.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F8de7bc2c-46c7-46c8-a8bc-b2c25511a45f_1067x571.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/8de7bc2c-46c7-46c8-a8bc-b2c25511a45f_1067x571.png","fullscreen":null,"height":571,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F8de7bc2c-46c7-46c8-a8bc-b2c25511a45f_1067x571.png?resize=728%2C571&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="571" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F8de7bc2c-46c7-46c8-a8bc-b2c25511a45f_1067x571.png?resize=728%2C571&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/8de7bc2c-46c7-46c8-a8bc-b2c25511a45f_1067x571.png","fullscreen":null,"height":571,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="571" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F8de7bc2c-46c7-46c8-a8bc-b2c25511a45f_1067x571.png?resize=728%2C571&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   如果进一步缩小范围，仅查看 2021 年的活动，我们可以确定活动高峰的关键时期。
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-614-728" href="https://i1.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fccf49885-3f86-405c-b4ee-44ac0645e610_1067x614.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ccf49885-3f86-405c-b4ee-44ac0645e610_1067x614.png","fullscreen":null,"height":614,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fccf49885-3f86-405c-b4ee-44ac0645e610_1067x614.png?resize=728%2C614&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="614" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fccf49885-3f86-405c-b4ee-44ac0645e610_1067x614.png?resize=728%2C614&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ccf49885-3f86-405c-b4ee-44ac0645e610_1067x614.png","fullscreen":null,"height":614,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="614" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fccf49885-3f86-405c-b4ee-44ac0645e610_1067x614.png?resize=728%2C614&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   那么，2021年4月发生了什么？只需要使用标准的开源情报技能和一些先进的谷歌搜索来关联事件。
  </p>
  <p>
   使用搜索查询 “Afghanistan” after:2021/04/01 before:2021/05/01，可以扩大搜索范围，找到相关的事件。
  </p>
  <p>
   【如果您尚未了解 Google dorks 的使用方法，
   <a href="https://iyouport.substack.com/p/googledorking-" rel="">
    看这里
   </a>
   】
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-411-728" href="https://i1.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0f3c0558-0035-47d9-a331-7c50fd921c8c_1067x411.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/0f3c0558-0035-47d9-a331-7c50fd921c8c_1067x411.png","fullscreen":null,"height":411,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0f3c0558-0035-47d9-a331-7c50fd921c8c_1067x411.png?resize=728%2C411&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="411" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0f3c0558-0035-47d9-a331-7c50fd921c8c_1067x411.png?resize=728%2C411&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/0f3c0558-0035-47d9-a331-7c50fd921c8c_1067x411.png","fullscreen":null,"height":411,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="411" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F0f3c0558-0035-47d9-a331-7c50fd921c8c_1067x411.png?resize=728%2C411&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   关键事件是美国正式宣布撤军和阿富汗的未来计划。虽然TOR活动的激增可能有其他潜在的原因，但这可以作为一个例子，说明我们可以在更多的地缘政治背景下分析TOR用户活动。
  </p>
  <ul>
   <li>
    如果您错过了《
    <a href="https://iyouport.substack.com/p/4a5" rel="">
     为什么是塔利班赢了？
    </a>
    》
   </li>
  </ul>
  <h3>
   <strong>
    服务器和客户端
   </strong>
  </h3>
  <p>
   我们可以使用TOR网络分析的另一个有用的方法是确定流量的最快路线。TOR通常比表面上的网络浏览慢很多，所以至少能够挑选出一个最佳的入口和出口节点可能是有用的。此外，虽然您不能控制中继，但有很多关于
   <a href="https://securityaffairs.co/wordpress/107076/hacking/attackers-control-23-tor-exit-nodes.html" rel="">
    威胁者控制出口节点
   </a>
   的报告，您就可能想把流量输送到一个已知的和可信任的出口，例如您自己设置的出口。
  </p>
  <h4>
   <strong>
    服务器
   </strong>
  </h4>
  <p>
   从下图中可以看到，德国和美国是TOR中继的主要来源。也可以使用下面的图表和TOR项目网站上的其他指标来分析速度。如果您想创建一个最佳的速度路线，可以使用这些指标来确定从您的具体位置出发的最佳路线。接下来将详细介绍如何配置您的客户端以指定入口和出口节点，以便在连接到TOR时进行更多的控制。
  </p>
  <div class="captioned-image-container">
   <figure>
    <p>
     <figure class="wp-caption aligncenter" style="width: 728px">
      <img alt="" class="sizing-default jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/82857b8d-b489-41dd-8d9e-bae9fab1990d_1067x609.png","fullscreen":null,"height":609,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F82857b8d-b489-41dd-8d9e-bae9fab1990d_1067x609.png?resize=728%2C609&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="609" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F82857b8d-b489-41dd-8d9e-bae9fab1990d_1067x609.png?resize=728%2C609&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
      <noscript>
       <img alt="" class="sizing-default" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/82857b8d-b489-41dd-8d9e-bae9fab1990d_1067x609.png","fullscreen":null,"height":609,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="609" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F82857b8d-b489-41dd-8d9e-bae9fab1990d_1067x609.png?resize=728%2C609&amp;ssl=1" width="728"/>
      </noscript>
      <figcaption class="wp-caption-text">
       <a href="https://metrics.torproject.org/bubbles.html#country" rel="noopener" target="_blank">
        https://metrics.torproject.org/bubbles.html#country
       </a>
      </figcaption>
     </figure>
    </p>
   </figure>
  </div>
  <p>
   另外一个有意义的指标是看所有中继的总可用带宽。通常可以将其与地缘政治事件联系起来，在这些时间内建立额外的中继或节点。此外，如果TOR的运行速度出乎意料地慢或无法连接，可以把它作为一种故障排除机制。
  </p>
  <div class="captioned-image-container">
   <figure>
    <p>
     <figure class="wp-caption aligncenter" style="width: 728px">
      <img alt="" class="sizing-default jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/630a255e-d1a9-43f3-86db-c52c9acf7eff_797x537.jpeg","fullscreen":null,"height":537,"width":797,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F630a255e-d1a9-43f3-86db-c52c9acf7eff_797x537.jpeg?resize=728%2C537&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="537" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F630a255e-d1a9-43f3-86db-c52c9acf7eff_797x537.jpeg?resize=728%2C537&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
      <noscript>
       <img alt="" class="sizing-default" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/630a255e-d1a9-43f3-86db-c52c9acf7eff_797x537.jpeg","fullscreen":null,"height":537,"width":797,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="537" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F630a255e-d1a9-43f3-86db-c52c9acf7eff_797x537.jpeg?resize=728%2C537&amp;ssl=1" width="728"/>
      </noscript>
      <figcaption class="wp-caption-text">
       <a href="https://metrics.torproject.org/bandwidth.html" rel="noopener" target="_blank">
        https://metrics.torproject.org/bandwidth.html
       </a>
      </figcaption>
     </figure>
    </p>
   </figure>
  </div>
  <h4>
   <strong>
    中继
   </strong>
  </h4>
  <p>
   也可以在TOR网络上搜索中继。如果您正在调查IP并查看主机的路由活动，可以使用中继搜索来找到一个潜在的起点或支点。还可以使用这个功能来识别可能想要配置的中继，以便在后文中进一步配置客户端时进行特定的流量路由。
  </p>
  <div class="captioned-image-container">
   <figure>
    <p>
     <figure class="wp-caption aligncenter" style="width: 728px">
      <img alt="" class="sizing-default jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ca247c00-6e74-4bd1-b26d-1d9b1daf1fee_1067x758.png","fullscreen":null,"height":758,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fca247c00-6e74-4bd1-b26d-1d9b1daf1fee_1067x758.png?resize=728%2C758&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="758" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fca247c00-6e74-4bd1-b26d-1d9b1daf1fee_1067x758.png?resize=728%2C758&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
      <noscript>
       <img alt="" class="sizing-default" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ca247c00-6e74-4bd1-b26d-1d9b1daf1fee_1067x758.png","fullscreen":null,"height":758,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="758" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fca247c00-6e74-4bd1-b26d-1d9b1daf1fee_1067x758.png?resize=728%2C758&amp;ssl=1" width="728"/>
      </noscript>
      <figcaption class="wp-caption-text">
       <a href="https://metrics.torproject.org/rs.html#advanced" rel="noopener" target="_blank">
        https://metrics.torproject.org/rs.html#advanced
       </a>
      </figcaption>
     </figure>
    </p>
   </figure>
  </div>
  <p>
   考虑一个场景，您想找到可能与调查有关的中继。如果您有一个电子邮件地址、昵称或别名，可以使用中继搜索作为一个新的支点，在您通常的开源情报工作流程中找到其他线索。下面专门在澳大利亚搜索使用 @gmail.com 作为联系邮箱的中继。这些是否是合法的邮箱并不是本文的一部分，但它是另一个可以搜索的地方。
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-448-728" href="https://i1.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F798908c1-69c1-4eef-b10f-1b82043eff16_1067x448.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/798908c1-69c1-4eef-b10f-1b82043eff16_1067x448.png","fullscreen":null,"height":448,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F798908c1-69c1-4eef-b10f-1b82043eff16_1067x448.png?resize=728%2C448&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="448" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F798908c1-69c1-4eef-b10f-1b82043eff16_1067x448.png?resize=728%2C448&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/798908c1-69c1-4eef-b10f-1b82043eff16_1067x448.png","fullscreen":null,"height":448,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="448" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F798908c1-69c1-4eef-b10f-1b82043eff16_1067x448.png?resize=728%2C448&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   然后我们可以进入中继，获得更具体的细节，如指纹。这个标识符可以在下面的客户端配置中使用，以允许您将流量导向一个特定的节点。
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-707-728" href="https://i1.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F5a171d71-1f2d-447f-9618-2e937436fdad_1067x707.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/5a171d71-1f2d-447f-9618-2e937436fdad_1067x707.png","fullscreen":null,"height":707,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F5a171d71-1f2d-447f-9618-2e937436fdad_1067x707.png?resize=728%2C707&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="707" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F5a171d71-1f2d-447f-9618-2e937436fdad_1067x707.png?resize=728%2C707&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/5a171d71-1f2d-447f-9618-2e937436fdad_1067x707.png","fullscreen":null,"height":707,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="707" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F5a171d71-1f2d-447f-9618-2e937436fdad_1067x707.png?resize=728%2C707&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <h4>
   <strong>
    客户端配置
   </strong>
  </h4>
  <p>
   基于之前的分析和围绕控制入口和出口节点的评论，现在可以配置TOR浏览器捆绑在一个特定的国家、IP、或节点指纹上。
  </p>
  <p>
   要做到这一点，只需编辑客户端安装位置的 torrc 文件。
  </p>
  <p>
   Windows/Linux：如果在 Windows 或 Linux 上安装了Tor浏览器，torrc 文件是安装目录下的一个文件夹，看起来像这样
   <em>
    Tor Browser\Browser\TorBrowser\Data\Tor
   </em>
  </p>
  <div class="captioned-image-container">
   <figure>
    <p>
     <figure class="wp-caption aligncenter" style="width: 523px">
      <img alt="" class="sizing-default jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/59dab9f6-0653-4677-917d-b93c8eefee21_523x493.jpeg","fullscreen":null,"height":493,"width":523,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F59dab9f6-0653-4677-917d-b93c8eefee21_523x493.jpeg?resize=523%2C493&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="493" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F59dab9f6-0653-4677-917d-b93c8eefee21_523x493.jpeg?resize=523%2C493&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="523"/>
      <noscript>
       <img alt="" class="sizing-default" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/59dab9f6-0653-4677-917d-b93c8eefee21_523x493.jpeg","fullscreen":null,"height":493,"width":523,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="493" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F59dab9f6-0653-4677-917d-b93c8eefee21_523x493.jpeg?resize=523%2C493&amp;ssl=1" width="523"/>
      </noscript>
      <figcaption class="wp-caption-text">
       Windows的例子
      </figcaption>
     </figure>
    </p>
   </figure>
  </div>
  <p>
   如果您使用的是macOS，应该能够找到 torrc 文件在
   <em>
    ~/Library/Application Support/TorBrowser-Data/Tor/Data
   </em>
   目录下（请注意：在撰写本文时无法确认这个位置）
  </p>
  <p>
   Torrc 文件：打开 torrc 文件，只需要根据您想实现的目标添加以下几行：
  </p>
  <p>
   连接到一个特定的IP：（用IP地址替换x的位置）
  </p>
  <p>
   <em>
    ExitNodes xxx.xxx.xxx.xxx
   </em>
  </p>
  <p>
   <em>
    EntryNodes xxx.xxx.xxx.xxx
   </em>
  </p>
  <p>
   连接到一个特定的节点指纹： (用所需的节点替换指纹字符串)
  </p>
  <p>
   <em>
    ExitNodes 02E98BBE0B12570E4E2974E2A7472B297F8D9959
   </em>
  </p>
  <p>
   注：上面的指纹是一个来自现有中继的例子。您可以使用下面讲述的搜索方法找到您想要的中继。
  </p>
  <p>
   只连接到一个特定的国家：
  </p>
  <p>
   <em>
    ExitNodes {us} StrictNodes 1
   </em>
  </p>
  <p>
   <em>
    EntryNodes {us} StrictNodes 1
   </em>
  </p>
  <p>
   只需将 “us” 替换为所选择的 ISO 两位字母国家代码，其中大多数是显而易见的，但您可以在这里找到一个参考列表：
   <a href="https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes" rel="">
    https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes
   </a>
  </p>
  <p>
   如果您想让您的所有流量在美国出入，最终应该得到如下图所示的结果：
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-444-728" href="https://i2.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F7731f353-a642-472a-9663-2b55c9cb7a19_796x444.jpeg?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/7731f353-a642-472a-9663-2b55c9cb7a19_796x444.jpeg","fullscreen":null,"height":444,"width":796,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F7731f353-a642-472a-9663-2b55c9cb7a19_796x444.jpeg?resize=728%2C444&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="444" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F7731f353-a642-472a-9663-2b55c9cb7a19_796x444.jpeg?resize=728%2C444&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/7731f353-a642-472a-9663-2b55c9cb7a19_796x444.jpeg","fullscreen":null,"height":444,"width":796,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="444" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F7731f353-a642-472a-9663-2b55c9cb7a19_796x444.jpeg?resize=728%2C444&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   保存文件，然后连接到 TOR 并通过单击 TOR 浏览器中搜索栏左侧的图标来验证您的路线。下面是例子：
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-620-665" href="https://i2.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fef6761fc-a76e-4383-8122-936543fe0bf9_665x620.jpeg?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ef6761fc-a76e-4383-8122-936543fe0bf9_665x620.jpeg","fullscreen":null,"height":620,"width":665,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fef6761fc-a76e-4383-8122-936543fe0bf9_665x620.jpeg?resize=665%2C620&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="620" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fef6761fc-a76e-4383-8122-936543fe0bf9_665x620.jpeg?resize=665%2C620&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="665"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ef6761fc-a76e-4383-8122-936543fe0bf9_665x620.jpeg","fullscreen":null,"height":620,"width":665,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="620" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fef6761fc-a76e-4383-8122-936543fe0bf9_665x620.jpeg?resize=665%2C620&amp;ssl=1" width="665"/>
     </noscript>
    </a>
   </figure>
  </div>
  <h4>
   <strong>
    网络流量
   </strong>
  </h4>
  <p>
   Unchartered 建立了一个有用的地图和仪表盘来可视化TOR网络流量和带宽。有各种控件可帮您钻研信息，但它的数据也来自TOR项目指标网站的公共数据集。
  </p>
  <div class="captioned-image-container">
   <figure>
    <p>
     <figure class="wp-caption aligncenter" style="width: 728px">
      <img alt="" class="sizing-default jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/485a87f2-8008-4e87-a10e-7c7cb633d4fc_1067x540.jpeg","fullscreen":null,"height":540,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F485a87f2-8008-4e87-a10e-7c7cb633d4fc_1067x540.jpeg?resize=728%2C540&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="540" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F485a87f2-8008-4e87-a10e-7c7cb633d4fc_1067x540.jpeg?resize=728%2C540&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
      <noscript>
       <img alt="" class="sizing-default" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/485a87f2-8008-4e87-a10e-7c7cb633d4fc_1067x540.jpeg","fullscreen":null,"height":540,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="540" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F485a87f2-8008-4e87-a10e-7c7cb633d4fc_1067x540.jpeg?resize=728%2C540&amp;ssl=1" width="728"/>
      </noscript>
      <figcaption class="wp-caption-text">
       <a href="https://torflow.uncharted.software/" rel="noopener" target="_blank">
        https://torflow.uncharted.software/
       </a>
      </figcaption>
     </figure>
    </p>
   </figure>
  </div>
  <p>
   最后，如果您想获得一份所有TOR出口节点的清单，以便输入SIEM，使用工具进行映射，或者整合到您正在建设的项目中，可以在这里查看：
   <a href="https://check.torproject.org/torbulkexitlist" rel="">
    https://check.torproject.org/torbulkexitlist
   </a>
  </p>
  <p>
   还可以使用像 Bulk IP lookup 这样的工具，通过简单地复制和粘贴您想映射的IP（
   <a href="https://app.ipapi.co/bulk" rel="">
    https://app.ipapi.co/bulk
   </a>
   ）来映射节点列表（限于1000个节点），或者用IP查询服务和API建立您自己的工具。
  </p>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-515-728" href="https://i2.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F73d46832-8c61-48ca-b420-8f8e3d1f248b_1067x515.jpeg?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/73d46832-8c61-48ca-b420-8f8e3d1f248b_1067x515.jpeg","fullscreen":null,"height":515,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F73d46832-8c61-48ca-b420-8f8e3d1f248b_1067x515.jpeg?resize=728%2C515&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="515" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F73d46832-8c61-48ca-b420-8f8e3d1f248b_1067x515.jpeg?resize=728%2C515&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/73d46832-8c61-48ca-b420-8f8e3d1f248b_1067x515.jpeg","fullscreen":null,"height":515,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="515" src="https://i0.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F73d46832-8c61-48ca-b420-8f8e3d1f248b_1067x515.jpeg?resize=728%2C515&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <h3>
   <strong>
    结论
   </strong>
  </h3>
  <p>
   通过了解TOR网络，您可以从中学到很多东西，并作为开源情报工作流程的一部分加以利用。无论是将地缘政治事件与活动高峰联系起来，这将有不同的相关性，这取决于你的任务，还是了解网络，以便您可以建立最佳的访问路由。此外，用受信任的TOR节点路由控制您的客户端配置，可能在您的威胁缓解策略中发挥作用，以避免威胁者占据在恶意节点上。⚪️
  </p>
  <p>
   <a href="https://www.osintcombine.com/post/dark-web-part-ii-tor-network" rel="">
    TOR Network
   </a>
  </p>
  <div id="atatags-1611829871-61c32b9fd5d90">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-17389" href="https://www.iyouport.org/%e5%9c%a8tor%e4%b8%8a%e8%bf%bd%e8%b8%aa%e4%ba%8b%e4%bb%b6/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-17389" href="https://www.iyouport.org/%e5%9c%a8tor%e4%b8%8a%e8%bf%bd%e8%b8%aa%e4%ba%8b%e4%bb%b6/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-17389-61c32b9fd6523" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=17389&amp;origin=www.iyouport.org&amp;obj_id=161182987-17389-61c32b9fd6523" data-title="点赞或转载" id="like-post-wrapper-161182987-17389-61c32b9fd6523">
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
    <a href="https://www.iyouport.org/tag/investigative/" rel="tag">
     investigative
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/osint/" rel="tag">
     OSINT
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/tips/" rel="tag">
     tips
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/tor/" rel="tag">
     Tor
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-11-19T16:48:22+08:00">
    2021年11月19日
   </time>
   <time class="updated" datetime="2021-12-22T17:04:05+08:00">
    2021年12月22日
   </time>
  </div>
 </div>
</article>

