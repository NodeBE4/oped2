---
layout: post
title: "如何在没信号的情况下保持联系：构建离网Wi-Fi语音通信系统的方法 - iYouPort"
date: 2020-10-12T16:04:36+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e6%b2%a1%e4%bf%a1%e5%8f%b7%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e4%bf%9d%e6%8c%81%e8%81%94%e7%b3%bb%ef%bc%9a%e6%9e%84%e5%bb%ba%e7%a6%bb%e7%bd%91wi-fi%e8%af%ad%e9%9f%b3/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-14618 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-opinion category-54 category-67 tag-offline tag-protest tag-raspberry-pi tag-technique tag-technology tag-tools" id="post-14618">
 <header class="entry-header">
  <h1 class="entry-title">
   如何在”没信号”的情况下保持联系：构建离网Wi-Fi语音通信系统的方法
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
   <a href="https://www.iyouport.org/category/opinion/" rel="category tag">
    Opinion
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
   <time class="entry-date published" datetime="2020-10-13T00:04:36+08:00">
    2020年10月13日
   </time>
   <time class="updated" datetime="2020-10-13T00:04:03+08:00">
    2020年10月13日
   </time>
  </span>
  <span class="word-count">
   2 Minutes
  </span>
 </div>
 <div class="entry-content">
  <ul>
   <li class="graf graf--p">
    <span style="color: #00ccff;">
     <em>
      <strong>
       这个方法也许在抗议活动中或敏感行动中会更有用
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <p>
   <img alt="" class="aligncenter size-full wp-image-14619 jetpack-lazy-image" data-lazy-sizes="(max-width: 800px) 100vw, 800px" data-lazy-src="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=800%2C533&amp;is-pending-load=1#038;ssl=1" data-lazy-srcset="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?w=800&amp;ssl=1 800w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=300%2C200&amp;ssl=1 300w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=768%2C512&amp;ssl=1 768w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=272%2C182&amp;ssl=1 272w" data-recalc-dims="1" height="533" src="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=800%2C533&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="800"/>
   <noscript>
    <img alt="" class="aligncenter size-full wp-image-14619" data-recalc-dims="1" height="533" sizes="(max-width: 800px) 100vw, 800px" src="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=800%2C533&amp;ssl=1" srcset="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?w=800&amp;ssl=1 800w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=300%2C200&amp;ssl=1 300w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=768%2C512&amp;ssl=1 768w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/07/00-5.jpeg?resize=272%2C182&amp;ssl=1 272w" width="800"/>
   </noscript>
  </p>
  <p class="graf graf--p">
   在抗议活动出现时，当局会首先倾向于削弱移动信号或干脆断网，以切断活动家之间的联系，从而实现分头打击。
  </p>
  <p class="graf graf--p">
   于是在没信号的情况下如何保持行动力和继续工作，已经成为一个重要课题。不要错过 “如何应对断网” 系列，如下：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%96%ad%e7%bd%91%e5%90%8e%e5%a6%82%e4%bd%95%e8%bf%9b%e8%a1%8c%e6%96%87%e4%bb%b6%e5%85%b1%e4%ba%ab%e5%92%8c%e9%80%9a%e4%bf%a1%ef%bc%9f/" href="https://www.iyouport.org/%e6%96%ad%e7%bd%91%e5%90%8e%e5%a6%82%e4%bd%95%e8%bf%9b%e8%a1%8c%e6%96%87%e4%bb%b6%e5%85%b1%e4%ba%ab%e5%92%8c%e9%80%9a%e4%bf%a1%ef%bc%9f/" rel="noopener noreferrer" target="_blank">
     断网后如何进行文件共享和通信？：如何应对断网（1）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e6%90%9e%e5%ae%9a%e6%82%a8%e7%9a%84%e6%89%8b%e6%9c%ba%e4%bb%a5%e4%be%bf%e8%83%bd%e8%ae%a9%e5%ae%83%e5%ba%94%e4%bb%98%e6%96%ad%e7%bd%91%e7%8a%b6%e6%80%81%ef%bc%9f%ef%bc%9a%e5%a6%82/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e6%90%9e%e5%ae%9a%e6%82%a8%e7%9a%84%e6%89%8b%e6%9c%ba%e4%bb%a5%e4%be%bf%e8%83%bd%e8%ae%a9%e5%ae%83%e5%ba%94%e4%bb%98%e6%96%ad%e7%bd%91%e7%8a%b6%e6%80%81%ef%bc%9f%ef%bc%9a%e5%a6%82/" rel="noopener noreferrer" target="_blank">
     如何搞定您的手机以便能让它应付断网状态？：如何应对断网（2）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%88%91%e5%ba%94%e8%af%a5%e4%bd%bf%e7%94%a8%e8%bf%99%e4%b8%aa%e5%ba%94%e7%94%a8%e7%a8%8b%e5%ba%8f%e4%bf%9d%e5%ad%98%e7%9c%9f%e7%9b%b8%e5%90%97%ef%bc%9f%ef%bc%9a%e5%a6%82%e4%bd%95%e5%ba%94%e5%af%b9/" href="https://www.iyouport.org/%e6%88%91%e5%ba%94%e8%af%a5%e4%bd%bf%e7%94%a8%e8%bf%99%e4%b8%aa%e5%ba%94%e7%94%a8%e7%a8%8b%e5%ba%8f%e4%bf%9d%e5%ad%98%e7%9c%9f%e7%9b%b8%e5%90%97%ef%bc%9f%ef%bc%9a%e5%a6%82%e4%bd%95%e5%ba%94%e5%af%b9/" rel="noopener noreferrer" target="_blank">
     我应该使用这个应用程序保存真相吗？：如何应对断网（3）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%b2%a1%e6%9c%89%e4%ba%92%e8%81%94%e7%bd%91%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e5%a6%82%e4%bd%95%e9%aa%8c%e8%af%81%e8%a7%86%e8%a7%89%e4%bf%a1%e6%81%af%e7%9a%84%e7%9c%9f%e4%bc%aa%ef%bc%9a%e5%a6%82/" href="https://www.iyouport.org/%e6%b2%a1%e6%9c%89%e4%ba%92%e8%81%94%e7%bd%91%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e5%a6%82%e4%bd%95%e9%aa%8c%e8%af%81%e8%a7%86%e8%a7%89%e4%bf%a1%e6%81%af%e7%9a%84%e7%9c%9f%e4%bc%aa%ef%bc%9a%e5%a6%82/" rel="noopener noreferrer" target="_blank">
     没有互联网的情况下如何验证视觉信息的真伪：如何应对断网（4）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e6%b2%a1%e6%9c%89%e4%ba%92%e8%81%94%e7%bd%91%e6%88%96%e8%ae%a1%e7%ae%97%e6%9c%ba%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e5%a4%87%e4%bb%bd%e6%89%8b%e6%9c%ba%e4%b8%ad%e7%9a%84/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e6%b2%a1%e6%9c%89%e4%ba%92%e8%81%94%e7%bd%91%e6%88%96%e8%ae%a1%e7%ae%97%e6%9c%ba%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e5%a4%87%e4%bb%bd%e6%89%8b%e6%9c%ba%e4%b8%ad%e7%9a%84/" rel="noopener noreferrer" target="_blank">
     如何在没有互联网或计算机的情况下备份手机中的媒体文档？：如何应对断网（5）
    </a>
    》
   </li>
  </ul>
  <p class="graf graf--p">
   null-byte 介绍了一个方法，帮助您和队友之间保持通信。当然，在任何 “没信号” 的情况下都可以使用这种方法。
  </p>
  <p class="graf graf--p">
   当您无法获得稳定的蜂窝信号或无法立即访问Wi-Fi、但需要与周围的人进行通信时，可以使用 Raspberry Pi 和 Android 应用程序建立离网语音通信网络。
  </p>
  <p class="graf graf--p">
   有些应用程序（例如
   <a class="markup--anchor markup--p-anchor" data-href="https://bridgefy.me/demo-app/" href="https://bridgefy.me/demo-app/" rel="noopener noreferrer" target="_blank">
    Bridgefy
   </a>
   ）可以创建一个网状网络，以通过蓝牙与其他设备进行通信。但是，当您的行动是车队、并想与其他车子上的人打交道时，你们之间隔着的所有金属都会形成阻碍。即使在露天的情况下，也有很多阻碍蓝牙信号的障碍物。所以您最好还是使用其他东西。
  </p>
  <p class="graf graf--p">
   如果一个热点路由器的功能不足以连接所有人，那么带有体面的无线网络适配器的 Raspberry Pi 可以提供帮助。
  </p>
  <p class="graf graf--p">
   有了它，并在上面运行了 PirateBox 服务器，
   <strong class="markup--strong markup--p-strong">
    只要每个人都连接到其Wi-Fi热点，你就可以匿名共享图像、视频、音频文件、文档、语音通信和其他内容。
   </strong>
  </p>
  <p class="graf graf--p">
   随着抗议活动在世界各地发生，某些地区的执法部门会尝试禁用该地区的手机连接，以防止示威者彼此交谈。今年，抗议活动从美国开始席卷了很多国家，这种情况下移动通信可能陷入瘫痪或阻塞。
  </p>
  <p class="graf graf--p">
   本文中介绍的技巧可以帮助解决这类情况。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    你需要什么
   </strong>
  </h3>
  <p class="graf graf--p">
   1、
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/CanaKit-Raspberry-Complete-Starter-Kit/dp/B01C6Q2GSY/?tag=whtnb-20" href="https://www.amazon.com/CanaKit-Raspberry-Complete-Starter-Kit/dp/B01C6Q2GSY/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    <strong class="markup--strong markup--p-strong">
     Raspberry Pi 3
    </strong>
   </a>
   ：因为较新的 Raspberry Pi 4 还没有 PirateBox 映像（这是一个匿名离线移动文件共享和通信系统）。但只要您有一个
   <a class="markup--anchor markup--p-anchor" data-href="https://nulb.app/x45qf" href="https://nulb.app/x45qf" rel="noopener noreferrer" target="_blank">
    Wi-Fi加密狗
   </a>
   ，其他任何 Pi 都可以使用。
  </p>
  <p class="graf graf--p">
   具体来说，这里使用的是
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/CanaKit-Raspberry-Starter-Premium-Black/dp/B07BCC8PK7/?tag=whtnb-20" href="https://www.amazon.com/CanaKit-Raspberry-Starter-Premium-Black/dp/B07BCC8PK7/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    Raspberry Pi 3 B+
   </a>
   模型。
  </p>
  <p class="graf graf--p">
   2、
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/exec/obidos/ASIN/B00DYQYITG/?tag=whtnb-20" href="https://www.amazon.com/exec/obidos/ASIN/B00DYQYITG/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    <strong class="markup--strong markup--p-strong">
     USB闪存驱动器
    </strong>
   </a>
   ：需要一个闪存驱动器作为 PirateBox 的硬驱。大小将取决于您的使用方式，因此大点儿的更好。
  </p>
  <p class="graf graf--p">
   如果您预计将传输大量的照片和视频，请尝试使用
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/Seagate-Expansion-Portable-External-STEA1000400/dp/B00TKFEEAS/?tag=whtnb-20" href="https://www.amazon.com/Seagate-Expansion-Portable-External-STEA1000400/dp/B00TKFEEAS/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    1 TB 的
   </a>
   外部硬盘驱动器，您将永远不必担心。
  </p>
  <p class="graf graf--p">
   3、
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/dp/B06XWN9Q99/?tag=whtnb-20" href="https://www.amazon.com/dp/B06XWN9Q99/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    <strong class="markup--strong markup--p-strong">
     MicroSD卡
    </strong>
   </a>
   ：确保其容量为16 GB或更大。为了安全起见，建议至少32 GB。
  </p>
  <p class="graf graf--p">
   4、
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/Vanja-standard-Connector-Notebooks-Smartphones/dp/B00W02VHM6/?tag=whtnb-20" href="https://www.amazon.com/Vanja-standard-Connector-Notebooks-Smartphones/dp/B00W02VHM6/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    <strong class="markup--strong markup--p-strong">
     MicroSD读卡器
    </strong>
   </a>
   ：有很多选择，基本上任何一个都可以。
  </p>
  <p class="graf graf--p">
   5、
   <strong class="markup--strong markup--p-strong">
    电源
   </strong>
   ：Raspberry Pi 单元需要此电源。
  </p>
  <p class="graf graf--p">
   6、
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/exec/obidos/ASIN/B00N2VILDM/?tag=whtnb-20" href="https://www.amazon.com/exec/obidos/ASIN/B00N2VILDM/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    <strong class="markup--strong markup--p-strong">
     以太网电缆
    </strong>
   </a>
   ：使用它来将您的 Raspberry Pi 连接到路由器，以进行全部设置。此后将不再需要。
  </p>
  <p class="graf graf--p">
   7、
   <strong class="markup--strong markup--p-strong">
    带有高增益天线的
   </strong>
   <a class="markup--anchor markup--p-anchor" data-href="https://nulb.app/x45qf" href="https://nulb.app/x45qf" rel="noopener noreferrer" target="_blank">
    <strong class="markup--strong markup--p-strong">
     无线网络适配器
    </strong>
   </a>
   ：如果您想获得更强的信号，则需要一个好的Wi-Fi适配器（
   <a class="markup--anchor markup--p-anchor" data-href="https://www.amazon.com/Alfa-Tube-U-Waterproof-High-Gain-Long-Rang/dp/B0052NP3C0/?tag=whtnb-20" href="https://www.amazon.com/Alfa-Tube-U-Waterproof-High-Gain-Long-Rang/dp/B0052NP3C0/?tag=whtnb-20" rel="noopener noreferrer" target="_blank">
    Alfa Tube-U
   </a>
   是一个不错的选择），带有不错的大型全向天线，专为室外使用而设计，例如用于房车和海上。
  </p>
  <p class="graf graf--p">
   确保它可与 Kali Linux 一起使用，以便在需要时可以将其用于其他目的。另外，这样做几乎可以保证它能与 PirateBox 一起使用。此外，Wi-Fi增强器可以帮助确保所有人保持连接状态。
  </p>
  <p class="graf graf--p">
   如果您想要花哨点的话，可以搞一个带有平板天线的适配器，然后将其指向目标，把它置于通信区域的中间位置（例如，中间位置的汽车），这是车队或大篷车的理想选择。
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="449" src="//www.youtube.com/embed/clWJ78N1new" width="800">
   </iframe>
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤1：设定 PirateBox
   </strong>
  </h3>
  <p class="graf graf--p">
   PirateBox 是一个非常酷的工具，您可以将其加载到充当离线通信盒子的 Raspberry Pi 上，在这里您可以连接到无线网络并在附近的设备上使用其聊天、文件服务器和其他功能。
  </p>
  <p class="graf graf--p">
   尤其是它基于开源路由器技术，应具有您进行语音通信所需要的所有交换。
  </p>
  <p class="graf graf--p">
   对于 PirateBox 的设置，可以
   <a class="markup--anchor markup--p-anchor" data-href="https://nulb.app/z46pi" href="https://nulb.app/z46pi" rel="noopener noreferrer" target="_blank">
    参见这里
   </a>
   。为了方便起见，下面嵌入了 null-byte 的网络武器实验室视频。基本在本案例的目的上您只需将 PirateBox 映像加载到 Raspberry Pi 上，通电，然后就应该能够连接到其Wi-Fi网络，在其中通过SSH登录。
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="449" src="//www.youtube.com/embed/3sYP19Ts48w" width="800">
   </iframe>
  </p>
  <p class="graf graf--p">
   因此建议您先下载 Raspberry Pi 3 的 PirateBox 映像，然后继续将其刷到 Raspberry Pi 的SD卡上，然后，一旦打开电源，您就应该能够连接到它所建立的Wi-Fi网络，然后通过SSH登录。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤2：连接到 PirateBox
   </strong>
  </h3>
  <p class="graf graf--p">
   要找出 PirateBox Pi 的IP地址是什么，使用一个
   <strong class="markup--strong markup--p-strong">
    arp-scan
   </strong>
   。在下面可以看到其中的一个确实是 Raspberry Pi，如果您没有其他Pi的话，很可能就是您的 PirateBox Pi。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ arp-scan -l

Interface: en0, datalink type: EN10MB (Ethernet)
Starting arp-scan 1.9.5 with 256 hosts (https://github.com/royhills/arp-scan)
192.168.77.1    b8:27:eb:4d:1f:f2       Raspberry Pi Foundation
192.168.77.128  b4:f1:da:ec:4c:e7       (Unknown)

516 packets received by filter, 0 packets dropped by kernel
Ending arp-scan 1.9.5: 256 hosts scanned in 1.858 seconds (137.78 hosts/sec). 2 responded</code></pre>
  <p class="graf graf--p">
   现在测试一下以确保没错。确保将Pi的地址换成下面命令中的地址。当要求连接时选择 “是”，然后输入您的 PirateBox Pi 的密码。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ ssh <a class="__cf_email__" data-cfemail="02636e63706f42333b302c33343a2c35352c33" href="/cdn-cgi/l/email-protection">[email protected]</a>

The authenticity of host '192.168.77.1 (192.168.77.1)' can't be established.
ECDSA key fingerprint is SHA256xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added '192.168.77.1' (ECDSA) to the list of known hosts.
<a class="__cf_email__" data-cfemail="86e7eae7f4ebc6b7bfb4a8b7b0bea8b1b1a8b7" href="/cdn-cgi/l/email-protection">[email protected]</a>'s password:</code></pre>
  <p class="graf graf--p">
   当您看到 PirateBox 屏幕时就成功了。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">____________________.__               __        __________
\______   \______   \__|___________ _/  |_  ____\______   \ _______  ___
 |       _/|     ___/  \_  __ \__  \\   __\/ __ \|    |  _//  _ \  \/  /
 |    |   \|    |   |  ||  | \// __ \|  | \  ___/|    |   (  &lt; &gt; &gt;    &lt;
 |____|_  /|____|   |__||__|  (____  /__|  \___  &gt;______  /\____/__/\_ \
        \/                         \/          \/       \/            \/

Website: http://piratebox.cc                 PirateBox Version: 1.1.4
Forum:   http://forum/piratebox.cc           Build date: 11-05-2018
IRC:     #piratebox irc.freenode.net         Be open  --  Share freely!

First Steps After Flashing
1. Change password of alarm user
 &gt; passwd
2. Change password of root user
 &gt; sudo password root
3. Enable Fake-Timeservice
 3.1 Set date and time
  # Disable network time sync
  &gt; sudo timedatectl set-ntp false
  # Set time to "Mon May 23 17:42:00" (Format: CCYYMMDD hhmm)
  &gt; sudo date -s "20170523 1742"
  &gt; cd /opt/piratebox &amp;&amp; sudo ./bin/timesave.sh ./conf/piratebox.conf install
 3.2 Enable on startup
  &gt; sudo systemctl enable timesave
4. Enable the Kareha Image and Discussion Board
  &gt; sudo /opt/piratebox/bin/board-autoconf.sh
5. Enable USB thumb drive share OR extend SDCard
 USB: &gt; sudo /opt/piratebox/rpi/bin/usb_share.sh
 SDCard: &gt; sudo /opt/piratebox/rpi/bin/sdcard_share.sh
6. Enable UPnP Media Server
  &gt; sudo cp /etc/minidlna.conf /etc/minidlna.conf.bkp
  &gt; sudo cp /opt/piratebox/src/linux.example.minidlna.conf /etc/minidlna.conf
  &gt; sudo systemctl stsart minidlna
  &gt; sudo systemctl enable minidlna
7. Enable RealTimeClock timekeeping (needs DS3231 or 1307 RTC module!)
  &gt; sudo systemctl enable rpi_hwclock
[<a class="__cf_email__" data-cfemail="aecfc2cfdcc3eecfc2cfdcc3dec7" href="/cdn-cgi/l/email-protection">[email protected]</a> ~]$</code></pre>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤3：更换Wi-Fi网卡（可选）
   </strong>
  </h3>
  <p class="graf graf--p">
   现在已经位于 PirateBox Pi 中了，如果您使用的是外部Wi-Fi适配器，则需要更改 /boot/wifi_card.conf 文件中的一个变量，以将其内部卡切换为您需要使用的卡。首先需要找到卡的名字，因此使用
   <strong class="markup--strong markup--p-strong">
    ifconfig
   </strong>
   。
  </p>
  <pre class="graf graf--pre"><code>[<a class="__cf_email__" data-cfemail="c0a1aca1b2ad80a1aca1b2adb0a9" href="/cdn-cgi/l/email-protection">[email protected]</a> ~]$ ifconfig</code></pre>
  <p class="graf graf--p">
   如果您只看到一个卡例如 wlan1，则需要
   <strong class="markup--strong markup--p-strong">
    ip a
   </strong>
   扫描一下，然后您可能会看到 wlan1 和 wlan0，那就对了。
  </p>
  <pre class="graf graf--pre"><code>[<a class="__cf_email__" data-cfemail="c9a8a5a8bba489a8a5a8bba4b9a0" href="/cdn-cgi/l/email-protection">[email protected]</a> ~]$ ip a</code></pre>
  <p class="graf graf--p">
   要启动并运行第二张卡，请使用以下命令，用您自己的卡名代替。然后输入您的密码。这时候您再返回去使用
   <strong class="markup--strong markup--p-strong">
    ifconfig
   </strong>
   ，就应该可以看到两张卡。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">[<a class="__cf_email__" data-cfemail="51303d30233c11303d30233c2138" href="/cdn-cgi/l/email-protection">[email protected]</a> ~]$ sudo ifconfig wlan0 up

[sudo] password for alarm:</code></pre>
  <p class="graf graf--p">
   现在，打开前面在nano中提到的配置文件，并确保它说出您正在使用的Wi-Fi适配器的名称。在键盘上按 Control-X 退出nano。如果更改了名称，请单击Y，然后按 Enter 以保存它。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">[<a class="__cf_email__" data-cfemail="82e3eee3f0efc2e3eee3f0eff2eb" href="/cdn-cgi/l/email-protection">[email protected]</a> ~]$ sudo nano /boot/wifi_card.conf

GNU nano 2.9.6              /boot/wifi_card.config

wlan1</code></pre>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤4：安装对讲机并连接到 PirateBox
   </strong>
  </h3>
  <p class="graf graf--p">
   现在，需要在将要使用 PirateBox Pi 相互通信的所有 Android 设备上下载并安装用于通信的应用程序。该应用程序称为 “
   <a class="markup--anchor markup--p-anchor" data-href="https://play.google.com/store/apps/details?id=com.androidintercom" href="https://play.google.com/store/apps/details?id=com.androidintercom" rel="nofollow noopener noreferrer" target="_blank">
    Intercom for Android
   </a>
   ”。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    <strong class="markup--strong markup--li-strong">
     Play Store Link:
    </strong>
    <a class="markup--anchor markup--li-anchor" data-href="https://play.google.com/store/apps/details?id=com.androidintercom" href="https://play.google.com/store/apps/details?id=com.androidintercom" rel="nofollow noopener noreferrer" target="_blank">
     <strong class="markup--strong markup--li-strong">
      Intercom for Android
     </strong>
    </a>
    <strong class="markup--strong markup--li-strong">
     (free)
    </strong>
   </li>
  </ul>
  <p class="graf graf--p">
   应用准备就绪后，要测试下，请断开 Android 手机上的移动数据网络连接，然后打开Wi-Fi设置，找到你的 PirateBox Pi，并连接到它。
  </p>
  <p class="graf graf--p">
   您的手机可能会警告您没有网络可用，别理它。当连接到 PirateBox 后，PirateBox 页面应该会马上打开，但现在对 PirateBox 界面不感兴趣。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="2880" data-image-id="0*Jmg6cg0n9Rdnfuv_.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Jmg6cg0n9Rdnfuv_.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1367" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Jmg6cg0n9Rdnfuv_.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="2880" data-image-id="0*Jmg6cg0n9Rdnfuv_.jpg" data-recalc-dims="1" data-width="1367" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Jmg6cg0n9Rdnfuv_.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="2880" data-image-id="0*DEIvGHKBdcjDxu_u.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*DEIvGHKBdcjDxu_u.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1367" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*DEIvGHKBdcjDxu_u.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="2880" data-image-id="0*DEIvGHKBdcjDxu_u.jpg" data-recalc-dims="1" data-width="1367" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*DEIvGHKBdcjDxu_u.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="2880" data-image-id="0*in4vTgY2hiaY1p45.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*in4vTgY2hiaY1p45.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1367" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*in4vTgY2hiaY1p45.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="2880" data-image-id="0*in4vTgY2hiaY1p45.jpg" data-recalc-dims="1" data-width="1367" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*in4vTgY2hiaY1p45.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤5：在同一 Wi-Fi 网络上与其他人交谈
   </strong>
  </h3>
  <p class="graf graf--p">
   现在，打开 Intercom for Android。您应该看到连接到 PirateBox Pi 的设备的列表。
  </p>
  <p class="graf graf--p">
   如果没有看到，请摸摸那个指南针，看会不会出现。如果不起作用，您可能首先需要通过蓝牙连接到其他设备，这似乎会拖慢应用程序识别它们的速度。希望对大多数人而言不会出现这种情况，因为理论上任何人都无需其他工作即可轻松连接。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="2880" data-image-id="0*1fwrOfEYRffinLQq.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*1fwrOfEYRffinLQq.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1367" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*1fwrOfEYRffinLQq.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="2880" data-image-id="0*1fwrOfEYRffinLQq.jpg" data-recalc-dims="1" data-width="1367" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*1fwrOfEYRffinLQq.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="2880" data-image-id="0*vMNxKH4WvjQkoEzG.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*vMNxKH4WvjQkoEzG.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1367" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*vMNxKH4WvjQkoEzG.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="2880" data-image-id="0*vMNxKH4WvjQkoEzG.jpg" data-recalc-dims="1" data-width="1367" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*vMNxKH4WvjQkoEzG.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   在本案例中现在可以看到一个设备，如果您点击Wi-Fi图标，它会发出声音以告知您已连接并可以通信。
  </p>
  <p class="graf graf--p">
   按住 “随按即说 PTT” 按钮就可以开始和其他人交谈。如果所有连接的设备的应用程序也都打开了，那他们就应该会听到您的声音。
  </p>
  <p class="graf graf--p">
   或者，您可以点击上方的圆点图标来切换模式。这样做将启用语音检测，因此您不必一直按着那个按钮。只需讲话，它就会听到您的声音并将通信传输给同一网络上的其他人。要切换回按键模式，只需点击评论框图标。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="2880" data-image-id="0*zA9hpwyE27OKYUua.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*zA9hpwyE27OKYUua.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1367" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*zA9hpwyE27OKYUua.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="2880" data-image-id="0*zA9hpwyE27OKYUua.jpg" data-recalc-dims="1" data-width="1367" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*zA9hpwyE27OKYUua.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="2880" data-image-id="0*FJ12v33zDruU4EtV.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*FJ12v33zDruU4EtV.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1367" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*FJ12v33zDruU4EtV.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="2880" data-image-id="0*FJ12v33zDruU4EtV.jpg" data-recalc-dims="1" data-width="1367" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*FJ12v33zDruU4EtV.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   完成了！这样一来即使没有蜂窝网络，您也应该能够将多部 Android 手机连接在一起。很酷是吧？
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    您可以执行更多高级操作
   </strong>
  </h3>
  <p class="graf graf--p">
   此项目有一些限制，但通常如果您想进一步深入，可以使用
   <a class="markup--anchor markup--p-anchor" data-href="https://openwrt.org/toh/raspberry_pi_foundation/raspberry_pi" href="https://openwrt.org/toh/raspberry_pi_foundation/raspberry_pi" rel="noopener noreferrer" target="_blank">
    OpenWrt
   </a>
   加载 Raspberry Pi。这是一款很酷的开源路由器固件，可让您深入研究选项并做各种有趣的事。
  </p>
  <p class="graf graf--p">
   但它设置起来有点复杂。于是本指南应该对初学者来说更合适些。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://null-byte.wonderhowto.com/how-to/build-off-grid-wi-fi-voice-communication-system-with-android-raspberry-pi-0296270/" href="https://null-byte.wonderhowto.com/how-to/build-off-grid-wi-fi-voice-communication-system-with-android-raspberry-pi-0296270/" rel="noopener noreferrer" target="_blank">
    Build an Off-Grid Wi-Fi Voice Communication System with Android &amp; Raspberry Pi
   </a>
  </p>
  <div id="atatags-1611829871-5f8511611bdd0">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-14618" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e6%b2%a1%e4%bf%a1%e5%8f%b7%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e4%bf%9d%e6%8c%81%e8%81%94%e7%b3%bb%ef%bc%9a%e6%9e%84%e5%bb%ba%e7%a6%bb%e7%bd%91wi-fi%e8%af%ad%e9%9f%b3/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Twitter 上共享">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击以在 Twitter 上共享（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-14618" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e6%b2%a1%e4%bf%a1%e5%8f%b7%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e4%bf%9d%e6%8c%81%e8%81%94%e7%b3%bb%ef%bc%9a%e6%9e%84%e5%bb%ba%e7%a6%bb%e7%bd%91wi-fi%e8%af%ad%e9%9f%b3/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Facebook 上共享">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-14618-5f8511611c7f2" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=14618&amp;origin=www.iyouport.org&amp;obj_id=161182987-14618-5f8511611c7f2" id="like-post-wrapper-161182987-14618-5f8511611c7f2">
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
    <a href="https://www.iyouport.org/tag/offline/" rel="tag">
     offline
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/protest/" rel="tag">
     protest
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/raspberry-pi/" rel="tag">
     Raspberry Pi
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
   <li>
    <a href="https://www.iyouport.org/tag/tools/" rel="tag">
     tools
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2020-10-13T00:04:36+08:00">
    2020年10月13日
   </time>
   <time class="updated" datetime="2020-10-13T00:04:03+08:00">
    2020年10月13日
   </time>
  </div>
 </div>
</article>

