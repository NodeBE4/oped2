---
layout: post
title: "构建自己的吹哨平台：在树莓派上运行OnionShare匿名投递箱 - iYouPort"
date: 2021-06-01T16:03:47+00:00
author: iYouPort
from: https://www.iyouport.org/%e6%9e%84%e5%bb%ba%e8%87%aa%e5%b7%b1%e7%9a%84%e5%90%b9%e5%93%a8%e5%b9%b3%e5%8f%b0%ef%bc%9a%e5%9c%a8%e6%a0%91%e8%8e%93%e6%b4%be%e4%b8%8a%e8%bf%90%e8%a1%8conionshare%e5%8c%bf%e5%90%8d%e6%8a%95%e9%80%92/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16184 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-59 category-54 category-67 tag-activism tag-onionshare tag-raspberry-pi tag-security tag-self-defense tag-technology tag-tools tag-truth tag-whistleblowers" id="post-16184">
 <header class="entry-header">
  <h1 class="entry-title">
   构建自己的吹哨平台：在树莓派上运行OnionShare匿名投递箱
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
   <a href="https://www.iyouport.org/category/%e5%85%b3%e4%ba%8e%e9%80%8f%e6%98%8e%e5%ba%a6%e9%9d%a9%e5%91%bd/" rel="category tag">
    关于透明度革命
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
   <time class="entry-date published" datetime="2021-06-02T00:03:47+08:00">
    2021年6月2日
   </time>
   <time class="updated" datetime="2021-03-05T13:46:22+08:00">
    2021年3月5日
   </time>
  </span>
  <span class="word-count">
   3 Minutes
  </span>
 </div>
 <div class="entry-content">
  <ul>
   <li class="graf graf--p">
    <span style="color: #00ccff;">
     <em>
      <strong>
       您需要足够省钱且足够有效的方法
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1122" data-image-id="1*supxW_4ctys2AcekauWXuw.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*supxW_4ctys2AcekauWXuw.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1504" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*supxW_4ctys2AcekauWXuw.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1122" data-image-id="1*supxW_4ctys2AcekauWXuw.png" data-recalc-dims="1" data-width="1504" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*supxW_4ctys2AcekauWXuw.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   【按】公民组织独立的吹哨平台是透明度革命的基础设施之一，当然，要完成吹哨您所需要的
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%85%ac%e6%b0%91%e8%b0%83%e6%9f%a5%e8%ae%b0%e8%80%85%e5%a6%82%e4%bd%95%e4%b8%8e%e5%90%b9%e5%93%a8%e4%ba%ba%e5%90%88%e4%bd%9c%ef%bc%9a7%e7%82%b9%e6%8f%90%e7%a4%ba/" href="https://www.iyouport.org/%e5%85%ac%e6%b0%91%e8%b0%83%e6%9f%a5%e8%ae%b0%e8%80%85%e5%a6%82%e4%bd%95%e4%b8%8e%e5%90%b9%e5%93%a8%e4%ba%ba%e5%90%88%e4%bd%9c%ef%bc%9a7%e7%82%b9%e6%8f%90%e7%a4%ba/" rel="noopener" target="_blank">
    远不止技术基础
   </a>
   ，但技术基础是最重要的，因为您必需保护吹哨人的匿名安全；如果人们很容易因为说出真相而被捕，我们将无法期待更多人的勇气。
   <strong class="markup--strong markup--p-strong">
    保护吹哨人的安全是您作为吹哨平台负责人的关键职责
   </strong>
   。
  </p>
  <p class="graf graf--p">
   我们介绍过 OnionShare 的基本用法，见《
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e7%ae%80%e6%98%93%e5%90%b9%e5%93%a8%e5%b9%b3%e5%8f%b0%e4%bc%a0%e8%be%93%e6%b3%84%e6%bc%8f%e6%95%b0%e6%8d%ae%ef%bc%9a%e6%b4%8b%e8%91%b1%e6%b1%a4%e6%8c%87%e5%8d%97/" href="https://www.iyouport.org/%e7%ae%80%e6%98%93%e5%90%b9%e5%93%a8%e5%b9%b3%e5%8f%b0%e4%bc%a0%e8%be%93%e6%b3%84%e6%bc%8f%e6%95%b0%e6%8d%ae%ef%bc%9a%e6%b4%8b%e8%91%b1%e6%b1%a4%e6%8c%87%e5%8d%97/" rel="noopener" target="_blank">
    简易吹哨平台传输泄漏数据：洋葱汤指南
   </a>
   》，它可以帮助您匿名投递和接收机密文件的泄漏。公民独立调查组织不可能有足够的资金支持昂贵的基础设施，摆脱基金会也应该作为您的基本追求之一，如果您想要真正独立的话。
  </p>
  <p class="graf graf--p">
   您获取的吹哨泄漏越是敏感度高就越是如此。所以我们需要足够省钱并且足够有效的解决方案。
  </p>
  <p class="graf graf--p">
   Micah Lee 介绍了一种方法，只需要 一个便宜的树莓派就能做到构建自己的匿名机密文件投递箱；它足够省钱，也足够可靠，但有一些注意事项您应该知道。下面是他提供的指南，
  </p>
  <p class="graf graf--p" style="text-align: center;">
   ♦️♦️♦️
  </p>
  <p class="graf graf--p">
   现在，OnionShare 的命令行版本已经
   <a class="markup--anchor markup--p-anchor" data-href="https://micahflee.com/2021/02/onionshare-tabs-anonymous-chat-cli/" href="https://micahflee.com/2021/02/onionshare-tabs-anonymous-chat-cli/" rel="noopener" target="_blank">
    更好地支持
   </a>
   在无头Linux服务器上运行，我想我可以建立一个专门的
   <a class="markup--anchor markup--p-anchor" data-href="https://www.raspberrypi.org/" href="https://www.raspberrypi.org/" rel="noopener" target="_blank">
    树莓派
   </a>
   匿名投递箱服务器。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     找到一个树莓派
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   就我个人而言，我从装满了随机电子设备的纸箱里挖出了一个值得信赖的老式树莓 Pi 3 Model B，毕竟很多人都有多余的树莓派躺在一堆旧电子设备中。如果您确实没有，目前 Raspberry Pi 4 Model B 的成本是 35 美元。
  </p>
  <p class="graf graf--p">
   树莓派使用 microSD 卡作为硬盘，所以您还需要一个 microSD 读卡器，可以把它插到您的电脑上进行设置，一根 micro-USB线为您的树莓派提供电源，还有一个网络连接（以太网是最简单的，但wifi也可以）。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     在树莓派上安装Ubuntu Server 20.04
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   按照
   <a class="markup--anchor markup--p-anchor" data-href="https://ubuntu.com/tutorials/how-to-install-ubuntu-on-your-raspberry-pi#1-overview" href="https://ubuntu.com/tutorials/how-to-install-ubuntu-on-your-raspberry-pi#1-overview" rel="noopener" target="_blank">
    Ubuntu制作的这个教程
   </a>
   在您的树莓派上安装Ubuntu。我使用的是 Ubuntu Server 20.04.2 LTS (RPi 3/4/400) 64位镜像。一旦您进行到了 “4.启动 Ubuntu Server” 的步骤，就可以回到本指南了。
  </p>
  <p class="graf graf--p">
   我不喜欢把HDMI线和USB键盘插到我的树莓派上，所以在插上以太网和电源后，我需要找到我的树莓派的IP地址，这样就可以通过网络远程连接到它。我使用
   <a class="markup--anchor markup--p-anchor" data-href="https://nmap.org/" href="https://nmap.org/" rel="noopener" target="_blank">
    nmap
   </a>
   来完成这个任务。您可以从 Linux 软件包管理器、Mac上的 Homebrew 或 Windows 上的 nmap 网站上安装它。
  </p>
  <p class="graf graf--p">
   因为我的本地网络IP地址是 192.168.1.x，所以我要扫描我的整个子网(192.168.1.0/24) 是否有打开SSH端口(22)的电脑，其中一台必然是我的树莓派。
  </p>
  <pre class="graf graf--pre">$ nmap -p22 --open 192.168.1.0/24
Starting Nmap 7.91 ( https://nmap.org ) at 2021-02-23 17:51 PST
Nmap scan report for 192.168.1.46
Host is up (0.0015s latency).

PORT   STATE SERVICE
22/tcp open  ssh

Nmap done: 256 IP addresses (7 hosts up) scanned in 3.13 seconds</pre>
  <p class="graf graf--p">
   就是这样，我的树莓派的IP地址是 192.168.1.46。所以看看我是否可以SSH进入它。您一定要用您自己的树莓派IP。默认的用户名和密码都是 ubuntu。
  </p>
  <pre class="graf graf--pre">$ ssh <a class="__cf_email__" data-cfemail="3742554259434277060e051906010f1906190301" href="/cdn-cgi/l/email-protection">[email protected]</a>
The authenticity of host '192.168.1.46 (192.168.1.46)' can't be established.
ECDSA key fingerprint is SHA256:tdB9dxpe4dIpFfvbjNdPpPVLeBlpTXaSu6SCaabjyFc.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '192.168.1.46' (ECDSA) to the list of known hosts.
<a class="__cf_email__" data-cfemail="344156415a404174050d061a05020c1a051a0002" href="/cdn-cgi/l/email-protection">[email protected]</a>'s password: 
You are required to change your password immediately (administrator enforced)
Welcome to Ubuntu 20.04.2 LTS (GNU/Linux 5.4.0-1028-raspi aarch64)
[...snip...]</pre>
  <p class="graf graf--p">
   登录后，您会被要求重新设置密码。把它设置为随机的东西，然后保存在您的密码管理器中。
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e4%bb%80%e4%b9%88%e6%98%af%e5%87%ad%e6%8d%ae%e5%a1%ab%e5%85%85%e6%94%bb%e5%87%bb%ef%bc%9f%e4%bb%a5%e5%8f%8a%e5%a6%82%e4%bd%95%e4%bf%9d%e6%8a%a4%e8%87%aa%e5%b7%b1/" href="https://www.iyouport.org/%e4%bb%80%e4%b9%88%e6%98%af%e5%87%ad%e6%8d%ae%e5%a1%ab%e5%85%85%e6%94%bb%e5%87%bb%ef%bc%9f%e4%bb%a5%e5%8f%8a%e5%a6%82%e4%bd%95%e4%bf%9d%e6%8a%a4%e8%87%aa%e5%b7%b1/" rel="noopener" target="_blank">
    <strong class="markup--strong markup--p-strong">
     在这里看到
    </strong>
   </a>
   <strong class="markup--strong markup--p-strong">
    密码管理器的选择方法
   </strong>
   。
  </p>
  <p class="graf graf--p">
   重置密码后，您的连接将被关闭，您需要再次SSH登录。
  </p>
  <pre class="graf graf--pre">[...snip...]
WARNING: Your password has expired.
You must change your password now and login again!
Changing password for ubuntu.
Current password: 
New password: 
Retype new password: 
passwd: password updated successfully
Connection to 192.168.1.46 closed.

$ ssh <a class="__cf_email__" data-cfemail="8df8eff8e3f9f8cdbcb4bfa3bcbbb5a3bca3b9bb" href="/cdn-cgi/l/email-protection">[email protected]</a>
<a class="__cf_email__" data-cfemail="295c4b5c475d5c6918101b07181f110718071d1f" href="/cdn-cgi/l/email-protection">[email protected]</a>'s password: 
Welcome to Ubuntu 20.04.2 LTS (GNU/Linux 5.4.0-1028-raspi aarch64)
[...snip...]
<a class="__cf_email__" data-cfemail="6712051209131227120512091312" href="/cdn-cgi/l/email-protection">[email protected]</a>:~$</pre>
  <p class="graf graf--p">
   已经进来了。继续并通过运行以下命令安装更新：
  </p>
  <pre class="graf graf--pre">sudo apt update
sudo apt upgrade -y</pre>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     安装 OnionShare
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   OnionShare用python编写，您可以使用 pip
   <a class="markup--anchor markup--p-anchor" data-href="https://docs.onionshare.org/2.3.1/en/advanced.html#command-line-interface" href="https://docs.onionshare.org/2.3.1/en/advanced.html#command-line-interface" rel="noopener" target="_blank">
    安装命令行版本
   </a>
   。因此，首先必须安装 pip：
  </p>
  <pre class="graf graf--pre">sudo apt install python3-pip</pre>
  <p class="graf graf--p">
   现在安装 OnionShare：
  </p>
  <pre class="graf graf--pre">pip3 install --user onionshare-cli</pre>
  <p class="graf graf--p">
   当您使用pip安装程序并使用 -user 时，它会将它们安装到 ~/.local/bin 中，默认情况下它不在您的路径中。下次您通过SSH进入树莓派时会自动将 ~/.local/bin 添加到您的路径中：
  </p>
  <pre class="graf graf--pre">echo "PATH=\$PATH:~/.local/bin" &gt;&gt; ~/.bashrc
source ~/.bashrc</pre>
  <p class="graf graf--p">
   好了，现在尝试运行 onionshare-cli。您应该看到下面这样的信息：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1144" data-image-id="0*Dzhf5N6HbkEhSkVl.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Dzhf5N6HbkEhSkVl.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="913" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Dzhf5N6HbkEhSkVl.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1144" data-image-id="0*Dzhf5N6HbkEhSkVl.png" data-recalc-dims="1" data-width="913" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Dzhf5N6HbkEhSkVl.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     测试一下（安装tor）
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   来看一下我们是否可以运行一个聊天服务器：
  </p>
  <pre class="graf graf--pre">$ onionshare-cli --chat
OnionShare 2.3.1 | https://onionshare.org/

                     @@@@@@@@@                      
                @@@@@@@@@@@@@@@@@@@                 
             @@@@@@@@@@@@@@@@@@@@@@@@@              
           @@@@@@@@@@@@@@@@@@@@@@@@@@@@@            
             @@@@@@@@@@@@@@@@@@@@@@@@@@@@@           ___        _               
               @@@@@@         @@@@@@@@@@@@@         / _ \      (_)              
         @@@@    @               @@@@@@@@@@@       | | | |_ __  _  ___  _ __    
       @@@@@@@@                   @@@@@@@@@@       | | | | '_ \| |/ _ \| '_ \   
     @@@@@@@@@@@@                  @@@@@@@@@@      \ \_/ / | | | | (_) | | | |  
   @@@@@@@@@@@@@@@@                 @@@@@@@@@       \___/|_| |_|_|\___/|_| |_|  
      @@@@@@@@@                 @@@@@@@@@@@@@@@@    _____ _                     
      @@@@@@@@@@                  @@@@@@@@@@@@     /  ___| |                    
       @@@@@@@@@@                   @@@@@@@@       \ `--.| |__   __ _ _ __ ___ 
       @@@@@@@@@@@               @    @@@@          `--. \ '_ \ / _` | '__/ _ \
        @@@@@@@@@@@@@         @@@@@@               /\__/ / | | | (_| | | |  __/
         @@@@@@@@@@@@@@@@@@@@@@@@@@@@@             \____/|_| |_|\__,_|_|  \___|
           @@@@@@@@@@@@@@@@@@@@@@@@@@@@@            
             @@@@@@@@@@@@@@@@@@@@@@@@@              
                @@@@@@@@@@@@@@@@@@@                 
                     @@@@@@@@@                      

You must install tor to use OnionShare from the command line</pre>
  <p class="graf graf--p">
   哦对了，我需要安装tor。这很容易：
  </p>
  <pre class="graf graf--pre">sudo apt install tor</pre>
  <p class="graf graf--p">
   好了，再试一次：
  </p>
  <pre class="graf graf--pre">$ onionshare-cli --chat
OnionShare 2.3.1 | https://onionshare.org/

                     @@@@@@@@@                      
                @@@@@@@@@@@@@@@@@@@                 
             @@@@@@@@@@@@@@@@@@@@@@@@@              
           @@@@@@@@@@@@@@@@@@@@@@@@@@@@@            
             @@@@@@@@@@@@@@@@@@@@@@@@@@@@@           ___        _               
               @@@@@@         @@@@@@@@@@@@@         / _ \      (_)              
         @@@@    @               @@@@@@@@@@@       | | | |_ __  _  ___  _ __    
       @@@@@@@@                   @@@@@@@@@@       | | | | '_ \| |/ _ \| '_ \   
     @@@@@@@@@@@@                  @@@@@@@@@@      \ \_/ / | | | | (_) | | | |  
   @@@@@@@@@@@@@@@@                 @@@@@@@@@       \___/|_| |_|_|\___/|_| |_|  
      @@@@@@@@@                 @@@@@@@@@@@@@@@@    _____ _                     
      @@@@@@@@@@                  @@@@@@@@@@@@     /  ___| |                    
       @@@@@@@@@@                   @@@@@@@@       \ `--.| |__   __ _ _ __ ___ 
       @@@@@@@@@@@               @    @@@@          `--. \ '_ \ / _` | '__/ _ \
        @@@@@@@@@@@@@         @@@@@@               /\__/ / | | | (_| | | |  __/
         @@@@@@@@@@@@@@@@@@@@@@@@@@@@@             \____/|_| |_|\__,_|_|  \___|
           @@@@@@@@@@@@@@@@@@@@@@@@@@@@@            
             @@@@@@@@@@@@@@@@@@@@@@@@@              
                @@@@@@@@@@@@@@@@@@@                 
                     @@@@@@@@@                      

Connecting to the Tor network: 100% - Done

Give this address to the recipient:
http://onionshare:<a class="__cf_email__" data-cfemail="ddbcadadb8a9b4a7b8aff0bcbeb4b99db5b5a7a5a5a7bbaea5eee9beb6a5b7a9b1eea7ebbeb7babbb6eaeea9a4afeebba5bfaea8eeafa8b0b4acaebab9a7ebb3ab" href="/cdn-cgi/l/email-protection">[email protected]</a>morhnyd.onion

Press Ctrl+C to stop the server</pre>
  <p class="graf graf--p">
   加载您在Tor浏览器中看到的OnionShare地址，以确保其有效。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="830" data-image-id="0*0NqByPE_9sgqPIwp.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*0NqByPE_9sgqPIwp.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1020" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*0NqByPE_9sgqPIwp.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="830" data-image-id="0*0NqByPE_9sgqPIwp.png" data-recalc-dims="1" data-width="1020" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*0NqByPE_9sgqPIwp.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   很好。按Ctrl-C退出 OnionShare。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     启动一个永久的匿名敏感文件投递箱
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   要让别人匿名上传文件到您的电脑上（在本例中是您的树莓派），您可以使用
   <a class="markup--anchor markup--p-anchor" data-href="https://docs.onionshare.org/2.3.1/en/features.html#receive-files" href="https://docs.onionshare.org/2.3.1/en/features.html#receive-files" rel="noopener" target="_blank">
    接收模式
   </a>
   。在命令行中就是 -receive。
  </p>
  <p class="graf graf--p">
   您还需要确保使用 -persistent。这将会把Tor的洋葱密钥保存到一个文件中，这样如果您重启树莓派 ，可以用完全相同的 OnionShare 地址来启动您的服务。
  </p>
  <p class="graf graf--p">
   您可能还想使用 -public 来禁用默认的密码保护，基本上这可以让您在Twitter等公开的地方上发布一个链接到您的匿名投递箱，比如下面这样，于是任何人都可以去那里匿名泄露文件给您。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 794px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="532" data-image-id="1*Rv0ypJq25UM_0cQdMrOpWg.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Rv0ypJq25UM_0cQdMrOpWg.png?resize=794%2C532&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="794" height="532" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Rv0ypJq25UM_0cQdMrOpWg.png?resize=794%2C532&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="794"/>
     <noscript>
      <img alt="" class="graf-image" data-height="532" data-image-id="1*Rv0ypJq25UM_0cQdMrOpWg.png" data-recalc-dims="1" data-width="794" height="532" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Rv0ypJq25UM_0cQdMrOpWg.png?resize=794%2C532&amp;ssl=1" width="794"/>
     </noscript>
     <figcaption class="wp-caption-text">
      这位是 The Intercept 的驻美国的记者，以前是 The Young Turks 的高级调查记者，他正在征集吹哨
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   好了，把上述这些整合起来：
  </p>
  <pre class="graf graf--pre">$ onionshare-cli --receive --persistent ~/anon-dropbox.session --public
OnionShare 2.3.1 | https://onionshare.org/

                     @@@@@@@@@                      
                @@@@@@@@@@@@@@@@@@@                 
             @@@@@@@@@@@@@@@@@@@@@@@@@              
           @@@@@@@@@@@@@@@@@@@@@@@@@@@@@            
             @@@@@@@@@@@@@@@@@@@@@@@@@@@@@           ___        _               
               @@@@@@         @@@@@@@@@@@@@         / _ \      (_)              
         @@@@    @               @@@@@@@@@@@       | | | |_ __  _  ___  _ __    
       @@@@@@@@                   @@@@@@@@@@       | | | | '_ \| |/ _ \| '_ \   
     @@@@@@@@@@@@                  @@@@@@@@@@      \ \_/ / | | | | (_) | | | |  
   @@@@@@@@@@@@@@@@                 @@@@@@@@@       \___/|_| |_|_|\___/|_| |_|  
      @@@@@@@@@                 @@@@@@@@@@@@@@@@    _____ _                     
      @@@@@@@@@@                  @@@@@@@@@@@@     /  ___| |                    
       @@@@@@@@@@                   @@@@@@@@       \ `--.| |__   __ _ _ __ ___ 
       @@@@@@@@@@@               @    @@@@          `--. \ '_ \ / _` | '__/ _ \
        @@@@@@@@@@@@@         @@@@@@               /\__/ / | | | (_| | | |  __/
         @@@@@@@@@@@@@@@@@@@@@@@@@@@@@             \____/|_| |_|\__,_|_|  \___|
           @@@@@@@@@@@@@@@@@@@@@@@@@@@@@            
             @@@@@@@@@@@@@@@@@@@@@@@@@              
                @@@@@@@@@@@@@@@@@@@                 
                     @@@@@@@@@                      

Connecting to the Tor network: 100% - Done
 * Running on http://127.0.0.1:17636/ (Press CTRL+C to quit)

Files sent to you appear in this folder: /home/ubuntu/OnionShare

Warning: Receive mode lets people upload files to your computer. Some files can potentially take control of your computer if you open them. Only open things from people you trust, or if you know what you are doing.

Give this address to the sender:
http://vxat6yszh7o5r2fxzvibxsb4lmfi6yzudobn3o3yz2vhvue3z2xmbqid.onion

Press Ctrl+C to stop the server</pre>
  <p class="graf graf--p">
   现在，再次在Tor浏览器中加载 OnionShare 地址以确保其正常工作。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="830" data-image-id="0*H44b9Wn9VRRhrilv.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*H44b9Wn9VRRhrilv.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1020" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*H44b9Wn9VRRhrilv.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="830" data-image-id="0*H44b9Wn9VRRhrilv.png" data-recalc-dims="1" data-width="1020" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*H44b9Wn9VRRhrilv.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   这是有效的样子。
  </p>
  <p class="graf graf--p">
   实时网络日志也将显示在终端中。例如，当我加载 OnionShare 地址时，该地址显示在终端中是这样的：
  </p>
  <pre class="graf graf--pre">127.0.0.1 - - [24/Feb/2021 02:36:06] "GET / HTTP/1.1" 200 -
127.0.0.1 - - [24/Feb/2021 02:36:07] "GET /static_nwr7jepc7gzurz2tyf2ddqnaxe/css/style.css HTTP/1.1" 200 -
127.0.0.1 - - [24/Feb/2021 02:36:08] "GET /static_nwr7jepc7gzurz2tyf2ddqnaxe/js/jquery-3.5.1.min.js HTTP/1.1" 200 -
127.0.0.1 - - [24/Feb/2021 02:36:08] "GET /static_nwr7jepc7gzurz2tyf2ddqnaxe/js/receive.js HTTP/1.1" 200 -
127.0.0.1 - - [24/Feb/2021 02:36:08] "GET /static_nwr7jepc7gzurz2tyf2ddqnaxe/img/logo.png HTTP/1.1" 200 -
127.0.0.1 - - [24/Feb/2021 02:36:08] "GET /static_nwr7jepc7gzurz2tyf2ddqnaxe/img/logo_large.png HTTP/1.1" 200 -
127.0.0.1 - - [24/Feb/2021 02:36:09] "GET /static_nwr7jepc7gzurz2tyf2ddqnaxe/img/favicon.ico HTTP/1.1" 200 -</pre>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    您永远不会知道访问您的洋葱站点的人的IP地址。他们的IP总是看起来像127.0.0.1。这就是Tor洋葱服务的工作方式：您匿名运行服务，所有连接到您的服务的客户端也都是匿名的
   </strong>
   。如果有人加载您的匿名投递箱，而您正好在看终端，您就能知道有人在那里，因为您会看到他们生成的日志，但您不会知道那是谁。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     上传文件，然后查看上传的内容
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在让我们尝试上传一个文件。在我的例子中，我上传的是一个约2.6mb的图像文件，名为 IMG_0417.jpg。
  </p>
  <p class="graf graf--p">
   在终端中，您可以看到文件上传时的进度，然后可以看到它被保存到的位置：
  </p>
  <pre class="graf graf--pre">=&gt; 2.5 MiB IMG_0417.jpg             
Received: /home/ubuntu/OnionShare/2021-02-24/22.29.20/IMG_0417.jpg
127.0.0.1 - - [24/Feb/2021 22:29:29] "POST /upload-ajax HTTP/1.1" 200 -</pre>
  <p class="graf graf--p">
   但现在如何实际访问这个文件呢？有很多方法。以下是一些选项。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff6600;">
    <strong class="markup--strong markup--p-strong">
     在MacOS或Windows中
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   如果您使用macOS或Windows，可以使用SFTP软件，如
   <a class="markup--anchor markup--p-anchor" data-href="https://cyberduck.io/" href="https://cyberduck.io/" rel="noopener" target="_blank">
    Cyberduck
   </a>
   。例如，这里我在 Cyberduck 中设置了一个新的连接，叫做 onionsharepi：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1096" data-image-id="0*Rj_hMXHb36MR35NV.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Rj_hMXHb36MR35NV.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1244" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Rj_hMXHb36MR35NV.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1096" data-image-id="0*Rj_hMXHb36MR35NV.png" data-recalc-dims="1" data-width="1244" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Rj_hMXHb36MR35NV.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   然后当我连接到它时就可以浏览文件并将任何内容下载到我的计算机上：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1028" data-image-id="0*3CN8QXkAuKfpLEFn.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*3CN8QXkAuKfpLEFn.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1424" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*3CN8QXkAuKfpLEFn.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1028" data-image-id="0*3CN8QXkAuKfpLEFn.png" data-recalc-dims="1" data-width="1424" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*3CN8QXkAuKfpLEFn.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   最后，我可以打开 IMG_0417.jpg，看看我上传的这张图片是什么：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1652" data-image-id="0*9phRggUJf43dudu5.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*9phRggUJf43dudu5.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1328" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*9phRggUJf43dudu5.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1652" data-image-id="0*9phRggUJf43dudu5.png" data-recalc-dims="1" data-width="1328" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*9phRggUJf43dudu5.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #ff6600;">
    <strong class="markup--strong markup--p-strong">
     在 Linux 中
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   在Ubuntu（或其他使用 nautilus 作为文件管理器的发行版）中，打开文件管理器，转到 “Other Locations”，然后连接到服务器
   <code>
    sftp://
    <a class="__cf_email__" data-cfemail="cfbaadbaa1bbba8ffef6fde1fef9f7e1fee1fbf9" href="/cdn-cgi/l/email-protection">
     [email protected]
    </a>
    /
   </code>
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="685" data-image-id="0*Vt8zP5BWfClL4Ty2.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Vt8zP5BWfClL4Ty2.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="920" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Vt8zP5BWfClL4Ty2.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="685" data-image-id="0*Vt8zP5BWfClL4Ty2.png" data-recalc-dims="1" data-width="920" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*Vt8zP5BWfClL4Ty2.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   现在就可以访问该文件了：
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="543" data-image-id="0*MCLjWSwAD_Aczg9V.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*MCLjWSwAD_Aczg9V.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="920" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*MCLjWSwAD_Aczg9V.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="543" data-image-id="0*MCLjWSwAD_Aczg9V.png" data-recalc-dims="1" data-width="920" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*MCLjWSwAD_Aczg9V.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     确保匿名保管箱可以持久工作
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   用于在接收模式下启动OnionShare的命令是这样：
  </p>
  <pre class="graf graf--pre">onionshare-cli --receive --persistent ~/anon-dropbox.session --public</pre>
  <p class="graf graf--p">
   这存储了所有与这个会话相关的设置，包括获得相同的Tor洋葱地址所需的密钥，在文件 anon-dropbox.session 中。
  </p>
  <p class="graf graf--p">
   如果您退出 OnionShare 按 Ctrl-C，然后再次运行相同的命令（在终端按向上箭头，然后回车），它应该再次启动 OnionShare，URL应该是完全相同的。这一点很重要，因为如果您不得不退出 OnionShare (比如您需要拔掉树莓派的插头，然后把它插到别的地方，迫使它重新启动)，您需要能够让您的匿名保管箱用同样的地址重新运行。
  </p>
  <p class="graf graf--p">
   您可能希望将此文件的内容复制并粘贴到密码管理器的备注栏中，或以其他方式对其进行安全备份。这样，当您把咖啡洒在树莓派上时，就可以不费吹灰之力地重新启动和运行它。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff6600;">
    <strong class="markup--strong markup--p-strong">
     在屏幕会话中运行 OnionShare，这样您就可以关闭终端了
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   到目前为止，这个方法很好用，但是有一个很大的问题：当您通过SSH进入远程服务器（树莓派）并运行一个命令（onionshare-cli）时，如果您关闭终端，断开wifi连接，或者以其他方式结束SSH会话，它也会关闭 onionshare-cli。理想情况下，您会希望它总是打开的并在后台运行。
  </p>
  <p class="graf graf--p">
   一个简单的方法是使用 screen，一个终端多路复用器（您也可以使用 tmux 或其他您喜欢的东西）。如果 OnionShare 正在树莓派上运行，用 Ctrl-C 退出它。然后从终端上安装 screen，并下载一个简单的 .screenrc 文件，这样它看起来会更漂亮一些：
  </p>
  <pre class="graf graf--pre">sudo apt install -y screen
wget https://raw.githubusercontent.com/micahflee/dotfiles/master/.screenrc</pre>
  <p class="graf graf--p">
   然后运行 screen:
  </p>
  <pre class="graf graf--pre">screen</pre>
  <p class="graf graf--p">
   您应该会看到屏幕底部有一个新的条形图，黄色高亮显示为0 bash。这意味着您现在进入了一个屏幕会话。
  </p>
  <p class="graf graf--p">
   现在再次运行 onionshare-cli。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="776" data-image-id="0*x-nrPEsCB_6CwDbz.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*x-nrPEsCB_6CwDbz.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="846" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*x-nrPEsCB_6CwDbz.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="776" data-image-id="0*x-nrPEsCB_6CwDbz.png" data-recalc-dims="1" data-width="846" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*x-nrPEsCB_6CwDbz.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   现在继续操作，完全关闭终端窗口，并确保您仍然可以加载 OnionShare 地址。它应该可以正常加载，因为 onionshare-cli 应该仍在屏幕会话中运行。
  </p>
  <p class="graf graf--p">
   现在让我们返回。打开一个新的终端，并通过SSH再次回到树莓派：
  </p>
  <pre class="graf graf--pre">ssh <a class="__cf_email__" data-cfemail="225740574c565762131b100c13141a0c130c1614" href="/cdn-cgi/l/email-protection">[email protected]</a></pre>
  <p class="graf graf--p">
   进入后，重新连接
   <code>
    screen
   </code>
   ：
  </p>
  <pre class="graf graf--pre">screen -x</pre>
  <p class="graf graf--p">
   您应该再次看到您的 OnionShare 匿名投递箱。
  </p>
  <h2 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     最后的一些想法
    </strong>
   </span>
  </h2>
  <p class="graf graf--p">
   遵循本指南后，您应该有：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    一台安装了Ubuntu Server 20. 04的树莓派。
   </li>
   <li class="graf graf--li">
    能够通过SSH进入该服务器进行远程配置。
   </li>
   <li class="graf graf--li">
    一个在屏幕会话中运行的OnionShare匿名投递箱。
   </li>
   <li class="graf graf--li">
    能够在您的普通电脑上访问所有上传到您的匿名投递箱的文件。
   </li>
  </ul>
  <p class="graf graf--p">
   恭喜！现在您已经具备了接受来自公众的吹哨文件的平台。只要让人们知道他们可以加载您的 OnionShare 地址在Tor浏览器中匿名将文件发送给您。
  </p>
  <p class="graf graf--p">
   📌 这里有几件事要注意：
  </p>
  <p class="graf graf--p">
   1、您可以通过在终端保持打开状态并连接屏幕会话来查看是否有人访问它，并定期检查上传的文件。
  </p>
  <p class="graf graf--p">
   2、现在您正在运行一个服务器，定期安装更新是个好主意，这样它就不会被黑客攻击，同时也要注意 OnionShare 的更新（您可以通过运行 pip3 install — upgrade onionshare-cli 来更新 onionshare-cli）。您可能还想做其他事来加固您的服务器，比如开始使用SSH密钥而不是密码，或者设置一个防火墙。
  </p>
  <p class="graf graf--p">
   3、您的树莓派的硬盘没有加密，这意味着如果有人可以物理访问您的树莓派，他们可以简单地拔掉 microSD卡，将其插入自己的电脑，然后复制人们上传给您的所有机密文件。最好的解决方案是在这个设置中添加磁盘加密。但另一方面，
   <strong class="markup--strong markup--p-strong">
    每当有人给您发送任何吹哨文件时，您可以将其下载到电脑上，然后从树莓派中删除，然后安全地清除树莓派的 microSD 卡上的空闲空间，这样就无法恢复了
   </strong>
   。
  </p>
  <p class="graf graf--p">
   要安全删除空闲空间，请安装 secure-delete 包：
  </p>
  <pre class="graf graf--pre">sudo apt install secure-delete</pre>
  <p class="graf graf--p">
   然后运行 sfill 来填充所有从零开始的空闲空间：
  </p>
  <pre class="graf graf--pre">sudo sfill -v -l /</pre>
  <p class="graf graf--p">
   📌 警告: 接收模式可以让别人上传文件到您的电脑上。如果其中有恶意软件，它们有可能会控制您的电脑。请确保只打开来自您信任的人的东西，或者如果您知道您在做什么的话。
  </p>
  <p class="graf graf--p">
   这个警告在 OnionShare 中的显著位置，我觉得很有必要再次指出。就像为什么指示您不要随便打开邮件附件一样，您也不应该盲目地打开从 OnionShare 中收到的文档。
  </p>
  <p class="graf graf--p">
   📌
   <strong class="markup--strong markup--p-strong">
    如果您得到一个文件，担心它可能是恶意的，这里有几个策略可以尝试
   </strong>
   :
  </p>
  <p class="graf graf--p">
   1、如果是 office 文件，先用
   <a class="markup--anchor markup--p-anchor" data-href="https://dangerzone.rocks/" href="https://dangerzone.rocks/" rel="noopener" target="_blank">
    Dangerzone
   </a>
   运行它。这个工具可以把 office 文档变成安全的PDF，这样您就可以放心了。
  </p>
  <p class="graf graf--p">
   2、如果您不担心与第三方共享的话：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    可以把它上传到
    <a class="markup--anchor markup--li-anchor" data-href="https://www.virustotal.com/" href="https://www.virustotal.com/" rel="noopener" target="_blank">
     VirusTotal
    </a>
    上，让它被几十个反病毒程序扫描，这可能有助于告知您是否可以打开它。
   </li>
   <li class="graf graf--li">
    也可以将某些类型的文档（包括 office文档、视频和音频文件）上传到 Google Drive，然后在网页浏览器中查看，而不是Word或VLC等程序。
   </li>
   <li class="graf graf--li">
    更好的方法是，设置一个虚拟机，关闭网络，把文档复制到您的虚拟机上，然后在那里打开它。如果它是恶意的，它会试图黑入您的虚拟机而不是您的主机，如果它试图连接骇客服务器，是不会成功的，因为您的虚拟机没有联网。您可以
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%88%e5%a6%88%e8%af%b4%ef%bc%8c%e6%93%8d%e4%bd%9c%e5%ae%89%e5%85%a8%e6%b0%b8%e8%bf%9c%e4%b8%8d%e8%83%bd%e8%a2%ab%e5%bf%bd%e8%a7%86%e2%80%8a-%e2%80%8a%e5%8c%bf%e5%90%8d%e5%b7%a5%e5%85%b7%ef%bc%9a/" href="https://www.iyouport.org/%e5%a6%88%e5%a6%88%e8%af%b4%ef%bc%8c%e6%93%8d%e4%bd%9c%e5%ae%89%e5%85%a8%e6%b0%b8%e8%bf%9c%e4%b8%8d%e8%83%bd%e8%a2%ab%e5%bf%bd%e8%a7%86%e2%80%8a-%e2%80%8a%e5%8c%bf%e5%90%8d%e5%b7%a5%e5%85%b7%ef%bc%9a/" rel="noopener" target="_blank">
     试试 Whonix
    </a>
    。
   </li>
  </ul>
  <p class="graf graf--p">
   好运！希望公民独立调查组织能够拥有安全可靠的吹哨平台以帮助吹哨人公开真相。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://micahflee.com/2021/02/onionshare-anonymous-dropbox-raspberry-pi/" href="https://micahflee.com/2021/02/onionshare-anonymous-dropbox-raspberry-pi/" rel="noopener" target="_blank">
    Running an OnionShare anonymous dropbox on a Raspberry Pi
   </a>
  </p>
  <div id="atatags-1611829871-60b70451e231c">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16184" href="https://www.iyouport.org/%e6%9e%84%e5%bb%ba%e8%87%aa%e5%b7%b1%e7%9a%84%e5%90%b9%e5%93%a8%e5%b9%b3%e5%8f%b0%ef%bc%9a%e5%9c%a8%e6%a0%91%e8%8e%93%e6%b4%be%e4%b8%8a%e8%bf%90%e8%a1%8conionshare%e5%8c%bf%e5%90%8d%e6%8a%95%e9%80%92/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16184" href="https://www.iyouport.org/%e6%9e%84%e5%bb%ba%e8%87%aa%e5%b7%b1%e7%9a%84%e5%90%b9%e5%93%a8%e5%b9%b3%e5%8f%b0%ef%bc%9a%e5%9c%a8%e6%a0%91%e8%8e%93%e6%b4%be%e4%b8%8a%e8%bf%90%e8%a1%8conionshare%e5%8c%bf%e5%90%8d%e6%8a%95%e9%80%92/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16184-60b70451e29f6" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16184&amp;origin=www.iyouport.org&amp;obj_id=161182987-16184-60b70451e29f6" id="like-post-wrapper-161182987-16184-60b70451e29f6">
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
    <a href="https://www.iyouport.org/tag/activism/" rel="tag">
     Activism
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/onionshare/" rel="tag">
     OnionShare
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
   <li>
    <a href="https://www.iyouport.org/tag/tools/" rel="tag">
     tools
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/truth/" rel="tag">
     truth
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/whistleblowers/" rel="tag">
     Whistleblowers
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-06-02T00:03:47+08:00">
    2021年6月2日
   </time>
   <time class="updated" datetime="2021-03-05T13:46:22+08:00">
    2021年3月5日
   </time>
  </div>
 </div>
</article>

