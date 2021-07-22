---
layout: post
title: "如何将Kali Linux安装为U盘，以便在任何计算机上进行渗透测试和黑客攻击 - iYouPort"
date: 2021-07-21T16:04:47+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%b0%86kali-linux%e5%ae%89%e8%a3%85%e4%b8%bau%e7%9b%98%ef%bc%8c%e4%bb%a5%e4%be%bf%e5%9c%a8%e4%bb%bb%e4%bd%95%e8%ae%a1%e7%ae%97%e6%9c%ba%e4%b8%8a%e8%bf%9b%e8%a1%8c/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16687 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-289 tag-hacking tag-kali-linux tag-pentesting tag-technology tag-tools" id="post-16687">
 <header class="entry-header">
  <h1 class="entry-title">
   如何将Kali Linux安装为U盘，以便在任何计算机上进行渗透测试和黑客攻击
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
   <time class="entry-date published" datetime="2021-07-22T00:04:47+08:00">
    2021年7月22日
   </time>
   <time class="updated" datetime="2021-05-03T16:13:17+08:00">
    2021年5月3日
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
       便携的更方便
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="465" data-image-id="0*WiK2p2Wj__nQE7o5.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*WiK2p2Wj__nQE7o5.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="620" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*WiK2p2Wj__nQE7o5.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="465" data-image-id="0*WiK2p2Wj__nQE7o5.jpg" data-recalc-dims="1" data-width="620" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*WiK2p2Wj__nQE7o5.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   Kali Linux 是渗透测试和道德黑客的首选 Linux 发行版。但是，它不被推荐日常使用，如回复电子邮件、玩游戏或查看Facebook等。这就是为什么最好从USB驱动器运行您的 Kali Linux 系统。
  </p>
  <p class="graf graf--p">
   这个对黑客友好的基于Debian的发行版确实在2019年底进行了重大更新，将默认的桌面环境从重量级的 Gnome 改为了更轻量级的 Xfce，使Kali整体上更加敏捷和易响应。但仍然不能推荐它作为您的日常系统，除非您一天24小时一周7天只做黑客。
  </p>
  <p class="graf graf--p">
   如果您有一台专门的机器，在双启动的情况下使用Kali是个不错的选择，但如果想更便携一些，U盘上的版本才是您想要的东西。如果您有一台闲置的电脑，而您只打算用来做白帽工作，那么是的，通过各种手段，把Kali安装成主系统，这样您就可以充分利用电脑的硬件。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #000000;">
    <strong class="markup--strong markup--p-strong">
     您需要什么
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   您需要一个USB闪存驱动器。可以用一个小到4GB的U盘做基础，或者8GB的U盘，如果您想坚持的话，但一个更大的U盘可能会很方便，特别是如果您想保存数据的话。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.com.au/Centon-Valuepack-DataStick-Flash-Drive/dp/B076N2JKC9/?tag=wnbau-22" href="https://www.amazon.com.au/Centon-Valuepack-DataStick-Flash-Drive/dp/B076N2JKC9/?tag=wnbau-22" rel="nofollow noopener" target="_blank">
     Centon DataStick Pro 8 GB USB 3.0 (5-PK) — Up to 80 MB/s
    </a>
    ($24.99)
   </li>
   <li class="graf graf--li">
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.com.au/SanDisk-16GB-Ultra-Flash-Drive/dp/B077Y149DL/?tag=wnbau-22" href="https://www.amazon.com.au/SanDisk-16GB-Ultra-Flash-Drive/dp/B077Y149DL/?tag=wnbau-22" rel="nofollow noopener" target="_blank">
     SanDisk Ultra Fit 16 GB USB 3.1 — Up to 130 MB/s
    </a>
    ($6.32)
   </li>
   <li class="graf graf--li">
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7SX9NS/?tag=wnbau-22" href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7SX9NS/?tag=wnbau-22" rel="nofollow noopener" target="_blank">
     Samsung FIT Plus 32 GB USB 3.1 — Up to 200 MB/s
    </a>
    ($9.93)
   </li>
   <li class="graf graf--li">
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7P4SY4/?tag=wnbau-22" href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7P4SY4/?tag=wnbau-22" rel="nofollow noopener" target="_blank">
     Samsung FIT Plus 64 GB USB 3.1 — Up to 300 MB/s
    </a>
    ($12.49)
   </li>
   <li class="graf graf--li">
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7PDLXC/?tag=wnbau-22" href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7PDLXC/?tag=wnbau-22" rel="nofollow noopener" target="_blank">
     Samsung FIT Plus 128 GB USB 3.1 — Up to 400 MB/s
    </a>
    ($22.99)
   </li>
   <li class="graf graf--li">
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7Q41PM/?tag=wnbau-22" href="https://www.amazon.com.au/Samsung-MUF-128AB-AM-Plus-128GB/dp/B07D7Q41PM/?tag=wnbau-22" rel="nofollow noopener" target="_blank">
     Samsung FIT Plus 256 GB USB 3.1 — Up to 400 MB/s
    </a>
    ($41.99)
   </li>
  </ul>
  <p class="graf graf--p">
   您还需要 Kali Live ISO 文件和一个镜像程序，例如 Etcher 或 Rufus，下面将进行概述。
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="449" src="//www.youtube.com/embed/_PGJ980upPQ" width="800">
   </iframe>
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤1: 下载正确的 Kali Linux 版本
   </strong>
  </h3>
  <p class="graf graf--p">
   虽然有许多不同类型的 Kali Linux 镜像，但这里需要的是 “Live” 下载。您可以选择AMD的64位（适用于英特尔芯片），ARM64的64位（如较新的Mac中的M1芯片），以及i386的32位（您可能永远不会使用，因为它太过时了）。
  </p>
  <p class="graf graf--p">
   访问
   <a class="markup--anchor markup--p-anchor" data-href="https://www.kali.org/downloads" href="https://www.kali.org/downloads" rel="noopener" target="_blank">
    kali.org/downloads
   </a>
   并下载相应的Live镜像。由于这里使用的是M1 Mac，所以将使用ARM64的64位版本。无论您选择哪一个，您将只能使用Xfce桌面环境，而且不能指定额外的（元）数据包来安装。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1499" data-image-id="0*GLfSbQv5vVDgFES7.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*GLfSbQv5vVDgFES7.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*GLfSbQv5vVDgFES7.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1499" data-image-id="0*GLfSbQv5vVDgFES7.jpg" data-recalc-dims="1" data-width="1456" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*GLfSbQv5vVDgFES7.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤2: 安装一个USB格式化工具
   </strong>
  </h3>
  <p class="graf graf--p">
   在Linux和macOS电脑上，您可以使用dd命令将 Kali Live 镜像复制到USB驱动器上，但总是有选错驱动器的风险，并且由于覆盖了一个重要的驱动器而陷入困境。正因为如此，建议使用USB格式化工具。如果您在Windows上，Rufus是一个很好的工具，但
   <a class="markup--anchor markup--p-anchor" data-href="https://www.balena.io/etcher/" href="https://www.balena.io/etcher/" rel="noopener" target="_blank">
    Etcher
   </a>
   适用于Linux、macOS 和 Windows，下面将使用Etcher。
  </p>
  <p class="graf graf--p">
   前往
   <a class="markup--anchor markup--p-anchor" data-href="https://www.balena.io/etcher" href="https://www.balena.io/etcher" rel="noopener" target="_blank">
    balena.io/etcher
   </a>
   ，点击 “下载” 按钮，它应该能检测出您在哪个系统上，并给您正确的版本。如果没有，点击旁边的下拉按钮，选择您的操作系统。下载后，像安装其他应用程序一样安装它。例如，在macOS上，打开DMG，将 balenaEtcher 拖到您的应用程序文件夹。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="763" data-image-id="0*POSwSdvSernnNDSm.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*POSwSdvSernnNDSm.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*POSwSdvSernnNDSm.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="763" data-image-id="0*POSwSdvSernnNDSm.jpg" data-recalc-dims="1" data-width="1456" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*POSwSdvSernnNDSm.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤3：保存 Kali Live 镜像
   </strong>
  </h3>
  <p class="graf graf--p">
   打开Etcher，然后点击 “选择镜像”。您可能会看到 “从文件中闪存” 和 “从URL中闪存” 的选项，请选择 “从文件中闪存” 。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="873" data-image-id="0*k4D-1FtfxC7IlD3i.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*k4D-1FtfxC7IlD3i.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*k4D-1FtfxC7IlD3i.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="873" data-image-id="0*k4D-1FtfxC7IlD3i.jpg" data-recalc-dims="1" data-width="1456" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*k4D-1FtfxC7IlD3i.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   导航到您在步骤1中下载的Kali镜像，并选择它。然后，您需要点击 “选择目标” 来选择您的U盘。通过查看驱动器名称和可用空间，反复检查您是否选择了正确的驱动器。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="873" data-image-id="0*S_4q97MO2znHvBaw.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*S_4q97MO2znHvBaw.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*S_4q97MO2znHvBaw.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="873" data-image-id="0*S_4q97MO2znHvBaw.jpg" data-recalc-dims="1" data-width="1456" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*S_4q97MO2znHvBaw.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   现在剩下要做的就是单击 “ Flash！”。这将重新格式化您的闪存驱动器，以便所有内容都将被 Kali Live 镜像删除并覆盖。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="873" data-image-id="0*e6etVAEjxe5g5PIX.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*e6etVAEjxe5g5PIX.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*e6etVAEjxe5g5PIX.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="873" data-image-id="0*e6etVAEjxe5g5PIX.jpg" data-recalc-dims="1" data-width="1456" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*e6etVAEjxe5g5PIX.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   您可能会被要求输入密码。然后，Etcher 会显示一个进度条，表明还剩多少时间。当它完成时，您会看到一个 “Flash Complete” 的消息。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="873" data-image-id="0*Lgkh8vhhh6zlZcem.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Lgkh8vhhh6zlZcem.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Lgkh8vhhh6zlZcem.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="873" data-image-id="0*Lgkh8vhhh6zlZcem.jpg" data-recalc-dims="1" data-width="1456" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Lgkh8vhhh6zlZcem.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤4: 从 Kali Live USB 启动
   </strong>
  </h3>
  <p class="graf graf--p">
   现在是时候启动新的 Kali Live USB 了，但这个过程会根据电脑品牌、操作系统和处理器的不同而不同。在上面的 Cyber Weapons Lab 视频中，Nick展示了在 Linux 机器上启动华硕UEFI BIOS Utility 时发生的情况，如果您想让 Kali Live 在不选择它的情况下启动，就要改变启动顺序。
  </p>
  <p class="graf graf--p">
   在macOS上，这就容易多了。如果您有苹果M1芯片，只需关闭Mac的电源，然后打开它，按住电源按钮，直到您看到启动窗口。在基于英特尔的Mac上，在开机或重启电脑后立即按Option键，直到看到启动窗口。然后，只需选择 Kali Live 闪存驱动器来启动。
  </p>
  <p class="graf graf--p">
   要想知道如何进入BIOS和改变启动设置，和/或加载启动菜单，请为您的电脑型号和操作系统搜索 “从USB驱动器启动” 并找到相应的说明。这里有太多的说明了，网上有很多关于从外部磁盘启动的手册。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤5: 选择您想启动Kali的方式
   </strong>
  </h3>
  <p class="graf graf--p">
   一旦您启动了 Kali Live USB，您应该看到几个不同的选项来选择您想加载的Kali的版本。它们可能包括：
  </p>
  <p class="graf graf--p">
   Live系统：这将启动 Kali Live。在这种模式下，您不能保存任何更改。没有报告，没有日志，没有其他数据 — — 这些变化都不会被保存。这样，您每次启动 Kali Live 时，都是以一个全新的 Kali Live 开始。数据只保存在RAM中。
  </p>
  <p class="graf graf--p">
   Live系统（故障安全模式）：与Live系统相同，但在系统发生故障时是一个更强大的版本。这样一来，失败的系统就不会毁掉您的闪存盘。如果您需要对有问题的电脑进行故障排除，这是一个不错的选择。
  </p>
  <p class="graf graf--p">
   Live系统（取证模式）：与Live系统相同，带有取证友好工具，这样您就可以在主机上恢复文件，收集证据，并执行其他取证任务。内部硬盘永远不会被触动，外部设备和媒体也不会自动挂载，这样您就可以完全控制您可以连接到什么。
  </p>
  <p class="graf graf--p">
   Live系统（持久性）：与Live系统相同，只有变化会被保存，它将允许您检查主系统而不用担心正在运行的或锁定的进程。
  </p>
  <p class="graf graf--p">
   Live系统（加密的持久性）：只是用LUKS加密，所以其他人更难访问您的数据。
  </p>
  <p class="graf graf--p">
   Start installer：这可以让您启动安装程序，将Kali安装在一个内部驱动器上。
  </p>
  <p class="graf graf--p">
   高级选项：包括诸如 MemTest、Hardware Detection 等选项。
  </p>
  <p class="graf graf--p">
   要在不保存任何修改的情况下启动它，只需选择 “Live系统” 选项，这将使您作为非root用户直接进入新的Xfce桌面环境。然而，如果您想保存您的修改，请使用 “Live系统（持久性）” 或 “Live系统（加密持久性）”启动。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤6：在Kali Live上设置持久性
   </strong>
  </h3>
  <p class="graf graf--p">
   选择其中一个持久性选项并不意味着它可以开箱即用。首先要进行一些配置，主要是创建一个新的分区来保存您的所有数据。Kali有一些关于这样做的
   <a class="markup--anchor markup--p-anchor" data-href="https://www.kali.org/docs/usb/usb-persistence" href="https://www.kali.org/docs/usb/usb-persistence" rel="noopener" target="_blank">
    出色说明
   </a>
   。
  </p>
  <p class="graf graf--p">
   要在 Kali Live 分区之上创建一个分区，以7GB为终点，在终端窗口中以kali用户身份发出以下三个命令，这将在7GB的分区中保留Live选项，腾出其余的分区用于存储数据。请确保您是在刚刚启动的Kali Live系统中做这个动作。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ end=7GiB
~$ read start _ &lt; &lt;(du -bcm kali-linux-2021.1-live-arm64.iso | tail -1); echo $start
~$ parted /dev/sdb mkpart primary ${start}MiB $end</code></pre>
  <p class="graf graf--p">
   完成后，您现在应该有一个标有 /dev/sdb3 或 /dev/disk1s3 这样的第三分区。检查您的卷标识符，因为在这个过程的其余部分您将需要它。
  </p>
  <p class="graf graf--p">
   如果您想增加一些加密，以防有人可能拿到您的硬盘，以 kali 的身份发出以下两个命令。如果被提示要继续覆盖新的分区，就用大写字母输入 “YES”。当被要求输入口令时，选择一个口令并输入两次。如果您不想要加密，可以跳过它。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ cryptsetup --verbose --verify-passphrase luksFormat /dev/sdb3
~$ cryptsetup luksOpen /dev/sdb3 my_usb</code></pre>
  <p class="graf graf--p">
   接下来，以 kali 身份运行以下两个命令来创建一个标记为 “persistence” 的ext3文件系统。如果您选择跳过加密，请使用以下命令：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ mkfs.ext3 -L persistence /dev/sdb3
~$ e2label /dev/sdb3 persistence</code></pre>
  <p class="graf graf--p">
   如果您要加密，请使用：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ mkfs.ext3 -L persistence /dev/mapper/my_usb
~$ e2label /dev/mapper/my_usb persistence</code></pre>
  <p class="graf graf--p">
   接下来，创建一个挂载点，将新的分区挂载到那里，创建一个配置文件以启用持久性，然后卸载该分区。如果您没有对分区进行加密，请使用：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ mkdir -p /mnt/my_usb
~$ mount /dev/sdb3 /mnt/my_usb
~$ echo "/ union" &gt; /mnt/my_usb/persistence.conf
~$ umount /dev/sdb3</code></pre>
  <p class="graf graf--p">
   如果您加密了分区，请使用：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ mkdir -p /mnt/my_usb/
~$ mount /dev/mapper/my_usb /mnt/my_usb
~$ echo "/ union" &gt; /mnt/my_usb/persistence.conf
~$ umount /dev/mapper/my_usb</code></pre>
  <p class="graf graf--p">
   如果您没有加密这个分区，到这里就完成了。如果您加密了，还有一个命令需要以kali的身份发布，这将关闭这个新分区的加密通道：
  </p>
  <pre class="graf graf--pre"><code>~$ cryptsetup luksClose /dev/mapper/my_usb</code></pre>
  <p class="graf graf--p">
   现在，重新启动到 Kali Live 并选择适当的系统，一切都应该准备好了。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    第7步：为root用户添加一个密码
   </strong>
  </h3>
  <p class="graf graf--p">
   在新版本的Kali中，您默认是一个非root用户，但您可以通过使用以下方式以普通用户的身份发布root命令：
  </p>
  <pre class="graf graf--pre"><code>~$ sudo su</code></pre>
  <p class="graf graf--p">
   Kali Live 可能不会给root用户附加一个密码，所以如果您不想让其他人进入您的系统捣乱，您就必须创建一个。使用具有root权限的 passwd root 来做到这一点。输入您选择的密码，然后验证它：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~# passwd root

New password:
Retype new password:

passwd: password updated successfully</code></pre>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    探索您的新 Kali Live 系统
   </strong>
  </h3>
  <p class="graf graf--p">
   现在剩下的就是使用Kali了。您可以查看上面的视频，了解您可以配置什么，
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%bc%80%e5%a7%8b%e4%bd%bf%e7%94%a8-kail-linux%ef%bc%9a2020/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%bc%80%e5%a7%8b%e4%bd%bf%e7%94%a8-kail-linux%ef%bc%9a2020/" rel="noopener" target="_blank">
    以及这里关于安装 Kali 作为您的主系统的指南
   </a>
   ，其中介绍了很多要安装和调整的工具和设置。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://null-byte.wonderhowto.com/how-to/install-kali-linux-as-portable-live-usb-for-pen-testing-hacking-any-computer-0384587/" href="https://null-byte.wonderhowto.com/how-to/install-kali-linux-as-portable-live-usb-for-pen-testing-hacking-any-computer-0384587/" rel="noopener" target="_blank">
    Install Kali Linux as a Portable Live USB for Pen-Testing &amp; Hacking on Any Computer
   </a>
  </p>
  <div id="atatags-1611829871-60f8ce831d576">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16687" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%b0%86kali-linux%e5%ae%89%e8%a3%85%e4%b8%bau%e7%9b%98%ef%bc%8c%e4%bb%a5%e4%be%bf%e5%9c%a8%e4%bb%bb%e4%bd%95%e8%ae%a1%e7%ae%97%e6%9c%ba%e4%b8%8a%e8%bf%9b%e8%a1%8c/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16687" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%b0%86kali-linux%e5%ae%89%e8%a3%85%e4%b8%bau%e7%9b%98%ef%bc%8c%e4%bb%a5%e4%be%bf%e5%9c%a8%e4%bb%bb%e4%bd%95%e8%ae%a1%e7%ae%97%e6%9c%ba%e4%b8%8a%e8%bf%9b%e8%a1%8c/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16687-60f8ce831db5c" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16687&amp;origin=www.iyouport.org&amp;obj_id=161182987-16687-60f8ce831db5c" id="like-post-wrapper-161182987-16687-60f8ce831db5c">
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
    <a href="https://www.iyouport.org/tag/kali-linux/" rel="tag">
     Kali Linux
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/pentesting/" rel="tag">
     pentesting
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
   <time class="entry-date published" datetime="2021-07-22T00:04:47+08:00">
    2021年7月22日
   </time>
   <time class="updated" datetime="2021-05-03T16:13:17+08:00">
    2021年5月3日
   </time>
  </div>
 </div>
</article>

