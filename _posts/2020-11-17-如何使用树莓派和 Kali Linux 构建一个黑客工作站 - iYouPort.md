---
layout: post
title: "如何使用树莓派和 Kali Linux 构建一个黑客工作站 - iYouPort"
date: 2020-11-17T16:03:45+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8%e6%a0%91%e8%8e%93%e6%b4%be%e5%92%8c-kali-linux-%e6%9e%84%e5%bb%ba%e4%b8%80%e4%b8%aa%e9%bb%91%e5%ae%a2%e5%b7%a5%e4%bd%9c%e7%ab%99/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-15133 post type-post status-publish format-standard has-post-thumbnail hentry category-book-documentary category-knowledge-node category-289 category-54 tag-hacking-station tag-kali-linux tag-raspberry-pi tag-security tag-self-defense tag-technology" id="post-15133">
 <header class="entry-header">
  <h1 class="entry-title">
   如何使用树莓派和 Kali Linux 构建一个黑客工作站
  </h1>
 </header>
 <div class="entry-meta">
  <span class="byline">
   <a href="https://www.iyouport.org/author/gabrielfornard/" rel="author" title="由Gabriel Fornard发布">
    Gabriel Fornard
   </a>
  </span>
  <span class="cat-links">
   <a href="https://www.iyouport.org/category/book-documentary/" rel="category tag">
    Book &amp; Documentary
   </a>
   ,
   <a href="https://www.iyouport.org/category/knowledge-node/" rel="category tag">
    Knowledge Node
   </a>
   ,
   <a href="https://www.iyouport.org/category/%e6%8a%80%e6%9c%af/" rel="category tag">
    技术
   </a>
   ,
   <a href="https://www.iyouport.org/category/%e6%8a%80%e6%9c%af%e9%98%b2%e8%ba%ab-%e8%87%aa%e6%88%91%e4%bf%9d%e6%8a%a4%e6%96%b9%e6%b3%95/" rel="category tag">
    技术防身/自我保护方法
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2020-11-18T00:03:45+08:00">
    2020年11月18日
   </time>
   <time class="updated" datetime="2020-11-18T00:03:08+08:00">
    2020年11月18日
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
       抢在攻击者之前找到您的设备的弱点，并及时修补
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*wu5h8h3UEOMoU8JC.jpeg?w=1100&amp;ssl=1" data-height="600" data-image-id="0*wu5h8h3UEOMoU8JC.jpeg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*wu5h8h3UEOMoU8JC.jpeg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1280" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="600" data-image-id="0*wu5h8h3UEOMoU8JC.jpeg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*wu5h8h3UEOMoU8JC.jpeg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1280" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*wu5h8h3UEOMoU8JC.jpeg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="600" data-image-id="0*wu5h8h3UEOMoU8JC.jpeg" data-recalc-dims="1" data-width="1280" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*wu5h8h3UEOMoU8JC.jpeg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   本文将使用树莓派和 Kali Linux 构建功能强大的便携式黑客工作站，您可以使用该工作站来模拟针对智能设备的网络攻击。
  </p>
  <p class="graf graf--p">
   通过像黑客一样访问智能家居，您可以识别安全漏洞，在任何人有机会利用它们之前关闭这些漏洞。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    负责任地使用您的权力
   </strong>
  </h3>
  <p class="graf graf--p">
   在本教程结束时，您将创建一个网络测试机器，可以使用它来入侵任何智能设备或网络。但是，您应该只使用您的树莓派黑客工作站来访问您自己的网络或至少您有权限访问的网络 —— 例如，如果朋友或同事要求您对他们的网络进行安全测试。
  </p>
  <p class="graf graf--p">
   试图获得对受保护网络或智能设备的未经授权的访问在道德上总是有问题的，并且通常是非法的。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*ih8AMCKH86gPhRUGAuYhxQ.png?w=1100&amp;ssl=1" data-height="1286" data-image-id="1*ih8AMCKH86gPhRUGAuYhxQ.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*ih8AMCKH86gPhRUGAuYhxQ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1308" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="1286" data-image-id="1*ih8AMCKH86gPhRUGAuYhxQ.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*ih8AMCKH86gPhRUGAuYhxQ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1308" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*ih8AMCKH86gPhRUGAuYhxQ.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="1286" data-image-id="1*ih8AMCKH86gPhRUGAuYhxQ.png" data-recalc-dims="1" data-width="1308" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*ih8AMCKH86gPhRUGAuYhxQ.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   <em>
    <span style="color: #ff9900;">
     上图中这本书在这里下载
    </span>
   </em>
   ：
   <a class="markup--anchor markup--p-anchor" data-href="https://www.patreon.com/posts/dong-shou-jiao-40001212" href="https://www.patreon.com/posts/dong-shou-jiao-40001212" rel="nofollow noopener noreferrer" target="_blank">
    https://www.patreon.com/posts/dong-shou-jiao-40001212
   </a>
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    您需要什么
   </strong>
  </h3>
  <p class="graf graf--p">
   要完成本教程，您需要：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    一个树莓派
   </li>
   <li class="graf graf--li">
    与您的树莓派型号兼容的SD卡，例如 Micro SD卡
   </li>
   <li class="graf graf--li">
    一个键盘以及将此键盘连接到树莓派的方法
   </li>
   <li class="graf graf--li">
    一个显示器，以及将此显示器连接到树莓派的方法
   </li>
   <li class="graf graf--li">
    HDMI线缆
   </li>
   <li class="graf graf--li">
    访问将用于下载 Kali Linux 的便携式计算机或台式计算机
   </li>
  </ul>
  <p class="graf graf--p">
   有了这些工具后，就可以开始构建黑客工作站了。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    在树莓派上安装 Kali Linux
   </strong>
  </h3>
  <p class="graf graf--p">
   Kali Linux 是一个专门为渗透测试设计的Linux发行版，即通过模拟网络攻击来评估网络、设备或系统的安全性。
  </p>
  <p class="graf graf--p">
   首先需要将 Kali Linux 系统镜像装到树莓派上。在你的笔记本电脑或台式机上下载以下软件。
  </p>
  <p class="graf graf--p">
   1、前往
   <a class="markup--anchor markup--p-anchor" data-href="https://www.offensive-security.com/kali-linux-arm-images/#1493408272250-e17e9049-9" href="https://www.offensive-security.com/kali-linux-arm-images/#1493408272250-e17e9049-9" rel="noopener noreferrer" target="_blank">
    Offensive Security
   </a>
   网站，根据您的树莓派型号下载正确的 Kali Linux 镜像。您需要一种方法将 Kali Linux 写入SD卡。这里使用的是
   <a class="markup--anchor markup--p-anchor" data-href="https://www.balena.io/etcher/" href="https://www.balena.io/etcher/" rel="noopener noreferrer" target="_blank">
    最新版本的 Etcher
   </a>
   ，因为它是免费、开源和跨平台的。
  </p>
  <p class="graf graf--p">
   2、将SD卡插入笔记本电脑或台式机。
  </p>
  <p class="graf graf--p">
   3、启动 Etcher 应用程序。
  </p>
  <p class="graf graf--p">
   4、在 Etcher 中，单击 “选择镜像”，然后选择您刚刚下载的 Kali Linux 镜像。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*IpE4LZ3RMAXgj5Q3.png?w=1100&amp;ssl=1" data-height="417" data-image-id="0*IpE4LZ3RMAXgj5Q3.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*IpE4LZ3RMAXgj5Q3.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="417" data-image-id="0*IpE4LZ3RMAXgj5Q3.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*IpE4LZ3RMAXgj5Q3.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*IpE4LZ3RMAXgj5Q3.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="417" data-image-id="0*IpE4LZ3RMAXgj5Q3.png" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*IpE4LZ3RMAXgj5Q3.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   5、单击 “选择目标”，然后选择您的SD卡。现在，Etcher 会将 Linux 系统镜像刷入SD卡，这可能需要一段时间。
  </p>
  <p class="graf graf--p">
   6、一旦 Etcher 完成，请取出SD卡并将其插入您的树莓派。
  </p>
  <p class="graf graf--p">
   7、使用 HDMI 线缆将显示器连接到树莓派。
  </p>
  <p class="graf graf--p">
   8、将键盘连接到树莓派设备。
  </p>
  <p class="graf graf--p">
   9、将树莓派插入电源。 现在它应该自动启动。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vo-kxEQPLvNQ9_c0.jpg?w=1100&amp;ssl=1" data-height="378" data-image-id="0*vo-kxEQPLvNQ9_c0.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vo-kxEQPLvNQ9_c0.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="378" data-image-id="0*vo-kxEQPLvNQ9_c0.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vo-kxEQPLvNQ9_c0.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vo-kxEQPLvNQ9_c0.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="378" data-image-id="0*vo-kxEQPLvNQ9_c0.jpg" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vo-kxEQPLvNQ9_c0.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   10、出现提示时，使用默认用户名 “root” 和默认密码 “toor” 登录。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*UyENieTt7v-xhKPB.jpg?w=1100&amp;ssl=1" data-height="797" data-image-id="0*UyENieTt7v-xhKPB.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*UyENieTt7v-xhKPB.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="797" data-image-id="0*UyENieTt7v-xhKPB.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*UyENieTt7v-xhKPB.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*UyENieTt7v-xhKPB.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="797" data-image-id="0*UyENieTt7v-xhKPB.jpg" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*UyENieTt7v-xhKPB.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   11、成功登录 Kali Linux 后，请点击工具栏中的 Wi-Fi 符号并连接到您的网络。
  </p>
  <p class="graf graf--p">
   现在，您已经拥有运行 Kali Linux 的树莓派，并且准备好开始测试您的智能设备和家庭自动化网络了。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    安全测试任何智能设备或网络
   </strong>
  </h3>
  <p class="graf graf--p">
   您可以使用 Kali Linux 执行许多不同的安全性测试，但举例来说，本演示将执行以下操作：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    扫描网络上的设备以查看哪些端口是开放的并且处于活动状态，因此可以接收连接。
   </li>
   <li class="graf graf--li">
    尝试使用在网上公开的密码访问该设备。
   </li>
  </ul>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    使用 nmap 扫描开放端口
   </strong>
  </h3>
  <p class="graf graf--p">
   首先，我将使用 nmap 扫描我的智能设备之一：
  </p>
  <p class="graf graf--p">
   1、选择 Kali 标志
  </p>
  <p class="graf graf--p">
   2、导航到 “Vulnerability Analysis -&gt; nmap”
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*HkT6sRFm1HZzjRfx.jpg?w=1100&amp;ssl=1" data-height="880" data-image-id="0*HkT6sRFm1HZzjRfx.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*HkT6sRFm1HZzjRfx.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="880" data-image-id="0*HkT6sRFm1HZzjRfx.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*HkT6sRFm1HZzjRfx.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*HkT6sRFm1HZzjRfx.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="880" data-image-id="0*HkT6sRFm1HZzjRfx.jpg" data-recalc-dims="1" data-width="700" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*HkT6sRFm1HZzjRfx.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   3、在出现的窗口中，输入：
  </p>
  <pre class="graf graf--pre"><strong class="markup--strong markup--pre-strong">nmap</strong> --top-ports 20 <strong class="markup--strong markup--pre-strong">(</strong>IP address of your IoT device<strong class="markup--strong markup--pre-strong">)</strong></pre>
  <p class="graf graf--p">
   在本示例中，正在扫描的是用于监视前门的无线摄像机，因此命令是：
  </p>
  <pre class="graf graf--pre"><strong class="markup--strong markup--pre-strong">nmap</strong> --top-ports 20 192.168.1.31</pre>
  <p class="graf graf--p">
   nmap 工具现在将扫描此摄像机以查找最重要的20个服务，并显示所有已识别端口的明细。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*6Cv48HSzXjl0wLjy.jpg?w=1100&amp;ssl=1" data-height="469" data-image-id="0*6Cv48HSzXjl0wLjy.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*6Cv48HSzXjl0wLjy.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="469" data-image-id="0*6Cv48HSzXjl0wLjy.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*6Cv48HSzXjl0wLjy.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*6Cv48HSzXjl0wLjy.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="469" data-image-id="0*6Cv48HSzXjl0wLjy.jpg" data-recalc-dims="1" data-width="700" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*6Cv48HSzXjl0wLjy.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   在上面的屏幕截图中可以看到，有三个 open ​​连接。
  </p>
  <p class="graf graf--p">
   本教程将专注于22端口SSH。如果设法获得了这个设备的用户名和密码，那就可以使用SSH远程连接到摄像机并执行命令。
  </p>
  <p class="graf graf--p">
   那么黑客可能会如何尝试访问这个设备呢？
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    下载公开可用的密码
   </strong>
  </h3>
  <p class="graf graf--p">
   在此步骤中，我们将尝试使用词表来识别摄像机的登录详细信息，词表是可在线获取的密码列表。
  </p>
  <p class="graf graf--p">
   这里将使用 Kali Linux 提供的词表：
  </p>
  <p class="graf graf--p">
   1、在 Kali Linux 工具栏中，单击“终端”图标。
  </p>
  <p class="graf graf--p">
   2、在终端中，键入以下命令：
  </p>
  <pre class="graf graf--pre"><strong class="markup--strong markup--pre-strong">sudo</strong> <strong class="markup--strong markup--pre-strong">apt</strong> update</pre>
  <p class="graf graf--p">
   按 Enter 键。此命令将提供所有 Kali 软件包的列表，可能需要几分钟才能完成。
  </p>
  <p class="graf graf--p">
   3、上一个命令运行完毕后，您可以使用以下命令安装密码列表：
  </p>
  <pre class="graf graf--pre"><strong class="markup--strong markup--pre-strong">sudo</strong> <strong class="markup--strong markup--pre-strong">apt</strong> <strong class="markup--strong markup--pre-strong">install</strong> wordlists</pre>
  <p class="graf graf--p">
   这个公开密码列表现在将下载到您的树莓派。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    用 Hydra 破解密码
   </strong>
  </h3>
  <p class="graf graf--p">
   现在，我们可以运行 Hydra，这是一个试图通过快速连续地使用许多不同的密码来攻击设备或网络的方法来识别凭据的应用程序：
  </p>
  <p class="graf graf--p">
   1、在工具栏中，选择 “Kali Linux” 图标
  </p>
  <p class="graf graf--p">
   2、导航至 “Password attacks -&gt; Online attacks -&gt; Hydra.”
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*suDi9NSnMI1Ze_k3.jpg?w=1100&amp;ssl=1" data-height="718" data-image-id="0*suDi9NSnMI1Ze_k3.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*suDi9NSnMI1Ze_k3.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="718" data-image-id="0*suDi9NSnMI1Ze_k3.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*suDi9NSnMI1Ze_k3.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*suDi9NSnMI1Ze_k3.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="718" data-image-id="0*suDi9NSnMI1Ze_k3.jpg" data-recalc-dims="1" data-width="700" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*suDi9NSnMI1Ze_k3.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   3、在出现的窗口中，输入以下命令：
  </p>
  <pre class="graf graf--pre">hydra -l root -P <strong class="markup--strong markup--pre-strong">/</strong>usr<strong class="markup--strong markup--pre-strong">/</strong>share<strong class="markup--strong markup--pre-strong">/</strong>wordlists<strong class="markup--strong markup--pre-strong">/</strong>metasploit<strong class="markup--strong markup--pre-strong">/</strong>unix_passwords.txt -t 6 ssh:<strong class="markup--strong markup--pre-strong">//</strong>192.168.1.31</pre>
  <p class="graf graf--p">
   4、Hydra 现在将尝试使用词表提供的所有密码来访问该摄像机。
  </p>
  <p class="graf graf--p">
   几分钟后，Hydra 应该显示其结果。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-cfsrc="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*QWN3V0fxcPw3WJsO.jpg?w=1100&amp;ssl=1" data-height="525" data-image-id="0*QWN3V0fxcPw3WJsO.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*QWN3V0fxcPw3WJsO.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" style="display:none;visibility:hidden;"/>
   <noscript>
    <img class="graf-image aligncenter jetpack-lazy-image" data-height="525" data-image-id="0*QWN3V0fxcPw3WJsO.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*QWN3V0fxcPw3WJsO.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="700" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*QWN3V0fxcPw3WJsO.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   </noscript>
   <noscript>
    <img class="graf-image aligncenter" data-height="525" data-image-id="0*QWN3V0fxcPw3WJsO.jpg" data-recalc-dims="1" data-width="700" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*QWN3V0fxcPw3WJsO.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   如您在上面的屏幕截图中所见，这个摄像机有一个 root 密码被公开了。
  </p>
  <p class="graf graf--p">
   通过模拟网络攻击，现在已经发现了我的家庭自动化系统中的一个巨大的安全漏洞，第三方可以利用这个漏洞来访问我的摄像头。
  </p>
  <p class="graf graf--p">
   如果您在自己的网络中发现了类似的漏洞，至关重要的是，您要立刻修改为更安全的密码，并修改其他所有您也使用同样密码的设备、应用或账户。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    最后
   </strong>
  </h3>
  <p class="graf graf--p">
   本教程中您可以看到恶意的第三方如何对您的家庭网络发起攻击。通过模拟网络攻击，您可以在攻击者之前发现潜在的安全漏洞。
  </p>
  <p class="graf graf--p">
   这只是一个开始 —— 现在您的 Kali Linux 黑客站已经启动并运行，您将可以使用很多额外的工具和功能来测试您的智能设备和家庭自动化网络。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iottechtrends.com/build-hacking-station-with-raspberry-pi-kali-linux/" href="https://www.iottechtrends.com/build-hacking-station-with-raspberry-pi-kali-linux/" rel="noopener noreferrer" target="_blank">
    How to Build a Hacking Station with Raspberry Pi and Kali Linux
   </a>
  </p>
  <div id="atatags-1611829871-5fdb91f9af098">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-15133" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8%e6%a0%91%e8%8e%93%e6%b4%be%e5%92%8c-kali-linux-%e6%9e%84%e5%bb%ba%e4%b8%80%e4%b8%aa%e9%bb%91%e5%ae%a2%e5%b7%a5%e4%bd%9c%e7%ab%99/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Twitter 上共享">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击以在 Twitter 上共享（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-15133" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8%e6%a0%91%e8%8e%93%e6%b4%be%e5%92%8c-kali-linux-%e6%9e%84%e5%bb%ba%e4%b8%80%e4%b8%aa%e9%bb%91%e5%ae%a2%e5%b7%a5%e4%bd%9c%e7%ab%99/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Facebook 上共享">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-15133-5fdb91f9af84c" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=15133&amp;origin=www.iyouport.org&amp;obj_id=161182987-15133-5fdb91f9af84c" id="like-post-wrapper-161182987-15133-5fdb91f9af84c">
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
    <a href="https://www.iyouport.org/tag/hacking-station/" rel="tag">
     Hacking Station
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/kali-linux/" rel="tag">
     Kali Linux
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/raspberry-pi/" rel="tag">
     Raspberry Pi
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/security/" rel="tag">
     Security
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/self-defense/" rel="tag">
     self defense
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
   <time class="entry-date published" datetime="2020-11-18T00:03:45+08:00">
    2020年11月18日
   </time>
   <time class="updated" datetime="2020-11-18T00:03:08+08:00">
    2020年11月18日
   </time>
  </div>
 </div>
</article>

