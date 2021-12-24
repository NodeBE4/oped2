---
layout: post
title: "黑客如何用树莓派入侵ATM机 - iYouPort"
date: 2021-12-10T08:06:27+00:00
author: iYouPort
from: https://www.iyouport.org/%e9%bb%91%e5%ae%a2%e5%a6%82%e4%bd%95%e7%94%a8%e6%a0%91%e8%8e%93%e6%b4%be%e5%85%a5%e4%be%b5atm%e6%9c%ba/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-17472 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-289 tag-atm tag-hacking tag-security" id="post-17472">
 <header class="entry-header">
  <h1 class="entry-title">
   黑客如何用树莓派入侵ATM机
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
   <a href="https://www.iyouport.org/category/%e6%8a%80%e6%9c%af/" rel="category tag">
    技术
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-12-10T16:06:27+08:00">
    2021年12月10日
   </time>
   <time class="updated" datetime="2021-12-24T16:09:01+08:00">
    2021年12月24日
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
       看着机器疯狂吐钞票，就像中大奖一样……
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-468-728" href="https://i2.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F1516345e-11fa-4bd7-a6d7-7648c80e75eb_832x468.jpeg?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/1516345e-11fa-4bd7-a6d7-7648c80e75eb_832x468.jpeg","fullscreen":null,"height":468,"width":832,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F1516345e-11fa-4bd7-a6d7-7648c80e75eb_832x468.jpeg?resize=728%2C468&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="468" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F1516345e-11fa-4bd7-a6d7-7648c80e75eb_832x468.jpeg?resize=728%2C468&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/1516345e-11fa-4bd7-a6d7-7648c80e75eb_832x468.jpeg","fullscreen":null,"height":468,"width":832,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="468" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F1516345e-11fa-4bd7-a6d7-7648c80e75eb_832x468.jpeg?resize=728%2C468&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   网络犯罪分子正在对银行发动一场战争，清空 ATM 机上的钱。他们选择的工具是恶意软件、来自 eBay 的钥匙和树莓派。以下是他们的做法。
  </p>
  <h3>
   <strong>
    中大奖了
   </strong>
  </h3>
  <p>
   自从已故黑客和网络安全研究员巴纳比·杰克（Barnaby Michael Douglas Jack）向一个陶醉的听众展示他如何入侵自动取款机以来，已经过去了十多年了。杰克的演示发生在2010年7月28日，在拉斯维加斯的黑帽大会上。与拉斯维加斯著名的老虎机不同，杰克在舞台上演示的两台自动取款机里被塞满现金，直到它们被清空  — — 每次都是如此。反复。
  </p>
  <p>
   在这个可能是世界上最著名的赌城创造出 jackpotting 这个术语是很恰当的。它被用来描述针对自动取款机并清空它们的攻击。另一种常见的ATM攻击是盗刷，即 用户的PIN码和他们的卡上的数据被复制并用于创建克隆卡。
  </p>
  <p>
   这种现象只是在增加，每年都造成数千万美元的损失。一些估计说，
   <strong>
    自2016年以来，30个国家的100家不同银行的无数自动取款机中招，各种威胁者净赚10亿美元。
   </strong>
  </p>
  <p>
   这些大规模的行动是复杂的。它们需要计划、监视、一小支地面部队做配合、足够的知识、恰当的恶意软件和必要的设备。把自动取款机拴在卡车上然后开走的日子已经过去了。
  </p>
  <p>
   现在您可以使用树莓派来做这件事。
  </p>
  <h3>
   <strong>
    操作方式
   </strong>
  </h3>
  <p>
   自动取款机实际上是一台装在强化外壳中的计算机，与装满钱的抽屉相连。遗憾的是，计算机的操作系统并不像其外壳那样坚固。
   <strong>
    这类计算机大多数运行在 Windows 7 上，甚至 Windows XP 都很常见。这些都是过时的操作系统，早就应该退役了。它们的漏洞很多，而且被网络犯罪分子充分了解。
   </strong>
  </p>
  <p>
   恶意软件包可以直接在暗网上买到，以利用这些操作系统的漏洞并与自动取款机软件互动。它们的名字有 atmspitter、cutlet maker、green dispenser、fast cash 和 pylon 等；价格从200美元左右到1000美元不等，取决于你所针对的ATM机的品牌和型号。一些恶意软件包甚至包含属于自动取款机制造商的受损的专有软件。
  </p>
  <p>
   你还将花费约150美元购买你需要的设备，包括树莓派。
  </p>
  <h4>
   <strong>
    步骤1：目标在哪？
   </strong>
  </h4>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-550-728" href="https://i2.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F13f6fa2d-3df7-412f-92b9-d57331ac04ea_1067x550.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/13f6fa2d-3df7-412f-92b9-d57331ac04ea_1067x550.png","fullscreen":null,"height":550,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F13f6fa2d-3df7-412f-92b9-d57331ac04ea_1067x550.png?resize=728%2C550&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="550" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F13f6fa2d-3df7-412f-92b9-d57331ac04ea_1067x550.png?resize=728%2C550&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/13f6fa2d-3df7-412f-92b9-d57331ac04ea_1067x550.png","fullscreen":null,"height":550,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="550" src="https://i1.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2F13f6fa2d-3df7-412f-92b9-d57331ac04ea_1067x550.png?resize=728%2C550&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   首先要对一个城市的自动取款机进行绘制和研究。好的目标是那些使用率高的ATM机，因为它们装的钱最多。理想的目标是位于监控不足的或没有监控的地区的高价值自动提款机。
  </p>
  <p>
   攻击通常安排在黑色星期五或情人节等日子，这些日子里自动取款机中的钱会比平时多出20%。在圣诞节前的几周，自动取款机也会装上额外的钱，因为许多人在工资单中会收到年终奖或圣诞奖金。
  </p>
  <h4>
   <strong>
    步骤2：ATM机的品牌和型号是什么？
   </strong>
  </h4>
  <p>
   对自动取款机硬件的了解可以帮你购买适当的恶意软件和适当的钥匙来打开自动取款机的外壳。一些制造商将他们的名字写在ATM机的某个地方，这使得识别更加容易。制造ATM机的大公司有 Diebold Nixdorf, Wincor Nixdorf, NCR, Triton, 和 Hitachi-Omron。
  </p>
  <p>
   拍下自动取款机的照片可以让你从暗网联系人或谷歌图片搜索中获得帮助，以确定其品牌和型号。一旦掌握了你要搞的自动取款机的版本，你就可以在暗网市场 — — 甚至在阿里巴巴和eBay等网购渠道  — — 搜索到自动取款机的维修钥匙。
  </p>
  <p>
   这些钥匙的价格从10美元起步，一直到50美元左右不等。你可以用钥匙打开自动取款机并访问USB端口。
  </p>
  <h4>
   <strong>
    步骤3：安装恶意软件
   </strong>
  </h4>
  <p>
   自动取款机上的USB端口是受限的，只接受键盘或鼠标的连接。这是为了让维修人员对这些设备进行维护。把恶意软件加载到你的树莓派上，要有一个电池，以便它可以作为一个便携式装置运行。
  </p>
  <p>
   恶意软件的编写方式是让ATM相信树莓派是一个键盘。存储的命令从树莓派中进入到自动取款机中，而自动取款机则尽职尽责地执行这些命令。
  </p>
  <h4>
   <strong>
    步骤4：中奖啦
   </strong>
  </h4>
  <div class="captioned-image-container">
   <figure>
    <a class="image-link image2 image2-574-728" href="https://i0.wp.com/cdn.substack.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fddc7ba5a-7998-4c1d-bda5-22f55d56d27f_1067x574.png?ssl=1" rel="nofollow noopener" target="_blank">
     <img alt="" class="sizing-default aligncenter jetpack-lazy-image" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ddc7ba5a-7998-4c1d-bda5-22f55d56d27f_1067x574.png","fullscreen":null,"height":574,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-lazy-src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fddc7ba5a-7998-4c1d-bda5-22f55d56d27f_1067x574.png?resize=728%2C574&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" height="574" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fddc7ba5a-7998-4c1d-bda5-22f55d56d27f_1067x574.png?resize=728%2C574&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="728"/>
     <noscript>
      <img alt="" class="sizing-default aligncenter" data-attrs='{"src":"https://bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com/public/images/ddc7ba5a-7998-4c1d-bda5-22f55d56d27f_1067x574.png","fullscreen":null,"height":574,"width":1067,"resizeWidth":null,"bytes":null,"alt":null,"title":null,"type":null,"href":null}' data-recalc-dims="1" height="574" src="https://i2.wp.com/cdn.substack.com/image/fetch/w_1100,c_limit,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fbucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com%2Fpublic%2Fimages%2Fddc7ba5a-7998-4c1d-bda5-22f55d56d27f_1067x574.png?resize=728%2C574&amp;ssl=1" width="728"/>
     </noscript>
    </a>
   </figure>
  </div>
  <p>
   有可能让自动取款机以20秒左右40张钞票的速度吐钱，或者一分钟内大约120张。如果是100美元的钞票，那就是每分钟12000美元。
  </p>
  <p>
   确实就像中了大奖。
  </p>
  <h3>
   <strong>
    进深
   </strong>
  </h3>
  <p>
   大规模的攻击可以一次性击中多台自动取款机，这意味着你需要有很多合作者在街上进行这些攻击，并把钱带给你。这些人是犯罪谱系中低端的廉价马仔。通过一些指导和培训，这些低级别的马仔就有能力完成攻击的物理部分，其余的由恶意软件完成。
  </p>
  <p>
   给马仔们配备树莓派比笔记本电脑更便宜，而且树莓派足够小，更容易藏在身上。有时树莓派被安装了一个70美元的全球移动通信系统（GSM）接收器，这样它就可以通过短信接受命令。
  </p>
  <p>
   另一个变种是将USB记忆棒插入自动取款机，并通过记忆棒中的操作系统重新启动它。当自动取款机启动后，你可以将恶意软件直接安装到自动取款机当前休眠的操作系统中。当你使用常规操作系统重新启动自动取款机时，你可以通过插入一张特别制作的卡，或通过自动取款机键盘上的秘密组合键来控制恶意软件。
  </p>
  <p>
   自动取款机包含远程访问软件，因此可以对其进行远程支持和维护。如果你能破坏这个软件，你就可以远程控制你瞄准的自动提款机。你的马仔所要做的就是在正确的时间出现在正确的地点，以取钱。
  </p>
  <h3>
   <strong>
    我们不知道真正的规模有多大
   </strong>
  </h3>
  <p>
   有一种观点认为，很多ATM盗窃案都没有被报告，所以我们并不真正了解这种攻击的真实规模。然而，我们确实知道两件事：1、我们所知道的这类情况已经很严重；2、它将继续增长。
  </p>
  <p>
   在ATM制造商认真对待ATM安全性之前，网络犯罪分子会继续将ATM视为装满钱的盒子，随时等待被清空。⚫️
  </p>
  <p>
   <a href="https://www.cloudsavvyit.com/11402/how-hackers-are-using-raspberry-pi-to-hack-atms/" rel="">
    How Hackers Are Using Raspberry Pi to Hack ATMs
   </a>
  </p>
  <div id="atatags-1611829871-61c5cf1eed8b3">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-17472" href="https://www.iyouport.org/%e9%bb%91%e5%ae%a2%e5%a6%82%e4%bd%95%e7%94%a8%e6%a0%91%e8%8e%93%e6%b4%be%e5%85%a5%e4%be%b5atm%e6%9c%ba/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-17472" href="https://www.iyouport.org/%e9%bb%91%e5%ae%a2%e5%a6%82%e4%bd%95%e7%94%a8%e6%a0%91%e8%8e%93%e6%b4%be%e5%85%a5%e4%be%b5atm%e6%9c%ba/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-17472-61c5cf1eedec6" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=17472&amp;origin=www.iyouport.org&amp;obj_id=161182987-17472-61c5cf1eedec6" data-title="点赞或转载" id="like-post-wrapper-161182987-17472-61c5cf1eedec6">
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
    <a href="https://www.iyouport.org/tag/atm/" rel="tag">
     ATM
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/hacking/" rel="tag">
     hacking
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/security/" rel="tag">
     Security
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-12-10T16:06:27+08:00">
    2021年12月10日
   </time>
   <time class="updated" datetime="2021-12-24T16:09:01+08:00">
    2021年12月24日
   </time>
  </div>
 </div>
</article>

