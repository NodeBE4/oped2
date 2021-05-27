---
layout: post
title: "如何使用 SpiderFoot CLI 从网站提取比特币钱包地址和余额 - iYouPort"
date: 2021-04-27T16:04:01+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8-spiderfoot-cli-%e4%bb%8e%e7%bd%91%e7%ab%99%e6%8f%90%e5%8f%96%e6%af%94%e7%89%b9%e5%b8%81%e9%92%b1%e5%8c%85%e5%9c%b0%e5%9d%80%e5%92%8c%e4%bd%99%e9%a2%9d/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-15903 post type-post status-publish format-standard has-post-thumbnail hentry category-book-documentary category-knowledge-node category-osint tag-bitcoin tag-investigations tag-osint tag-spiderfoot tag-technology tag-tools" id="post-15903">
 <header class="entry-header">
  <h1 class="entry-title">
   如何使用 SpiderFoot CLI 从网站提取比特币钱包地址和余额
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
   <a href="https://www.iyouport.org/category/osint/" rel="category tag">
    OSINT
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-04-28T00:04:01+08:00">
    2021年4月28日
   </time>
   <time class="updated" datetime="2021-01-31T15:04:14+08:00">
    2021年1月31日
   </time>
  </span>
  <span class="word-count">
   6 Minutes
  </span>
 </div>
 <div class="entry-content">
  <ul>
   <li class="graf graf--p">
    <span style="color: #00ccff;">
     <em>
      <strong>
       使用一个强大的开源情报工具
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="600" data-image-id="0*d1DUrrihsIehNaDi.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*d1DUrrihsIehNaDi.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1280" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*d1DUrrihsIehNaDi.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="600" data-image-id="0*d1DUrrihsIehNaDi.jpg" data-recalc-dims="1" data-width="1280" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*d1DUrrihsIehNaDi.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   【按】我们有一个专门板块
   <a class="markup--anchor markup--p-anchor" data-href="https://start.me/p/RMQrDD/iyp-2" href="https://start.me/p/RMQrDD/iyp-2" rel="noopener" target="_blank">
    “监视区块链和返现金之战” 在 列表-2
   </a>
   中。加密货币追踪是近年来的热门议题，尤其是全球最厉害的间谍机构，往往投入最大的资源以追踪各种加密货币，由此催生了一大群监视技术公司进入开发相关工具的轨道。
  </p>
  <p class="graf graf--p">
   众所周知，
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e8%b7%9f%e8%b8%aa%e9%87%91%e9%92%b1%e7%9a%84%e8%b5%b0%e5%90%91%ef%bc%8c%e8%bf%bd%e8%b8%aa%e8%85%90%e8%b4%a5%e5%92%8c%e7%8a%af%e7%bd%aa-%e2%80%8a-%e2%80%8a-%e8%a7%a3%e7%a0%81%e7%a7%98%e5%af%86/" href="https://www.iyouport.org/%e8%b7%9f%e8%b8%aa%e9%87%91%e9%92%b1%e7%9a%84%e8%b5%b0%e5%90%91%ef%bc%8c%e8%bf%bd%e8%b8%aa%e8%85%90%e8%b4%a5%e5%92%8c%e7%8a%af%e7%bd%aa-%e2%80%8a-%e2%80%8a-%e8%a7%a3%e7%a0%81%e7%a7%98%e5%af%86/" rel="noopener" target="_blank">
    追踪金钱
   </a>
   是挖掘腐败和有组织犯罪的最有效战术，
   <strong class="markup--strong markup--p-strong">
    于是对加密货币的追踪也是直接行动活动家所关注的热门技能
   </strong>
   。可惜
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e5%8c%ba%e5%9d%97%e9%93%be%e4%b8%8a%e8%bf%bd%e8%b8%aa%e6%af%94%e7%89%b9%e5%b8%81%e4%ba%a4%e6%98%93%ef%bc%9f/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8%e5%8c%ba%e5%9d%97%e9%93%be%e4%b8%8a%e8%bf%bd%e8%b8%aa%e6%af%94%e7%89%b9%e5%b8%81%e4%ba%a4%e6%98%93%ef%bc%9f/" rel="noopener" target="_blank">
    这不是一个公平的游戏
   </a>
   ，政府间谍的 “优势” 在最后一步：他们可以威胁加密货币服务提供商交出用户的身份。而活动家往往无法做到。
  </p>
  <p class="graf graf--p">
   但活动家依旧可以在此进行足够深入的调查，并结合其他渠道获得的情报，以得出有效的见解。本文就是一个很好的用例。
  </p>
  <p class="graf graf--p">
   我们去年推荐过一本书，见下图，您可以在这里下载《
   <a class="markup--anchor markup--p-anchor" data-href="https://www.patreon.com/posts/zhui-zong-jia-mi-38190629" href="https://www.patreon.com/posts/zhui-zong-jia-mi-38190629" rel="noopener" target="_blank">
    追踪加密货币交易
   </a>
   》：
  </p>
  <figure class="graf graf--figure">
  </figure>
  <p>
   <img alt="" class="aligncenter size-full wp-image-15904 jetpack-lazy-image" data-lazy-sizes="(max-width: 947px) 100vw, 947px" data-lazy-src="https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=947%2C2048&amp;is-pending-load=1#038;ssl=1" data-lazy-srcset="https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?w=947&amp;ssl=1 947w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=139%2C300&amp;ssl=1 139w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=473%2C1024&amp;ssl=1 473w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=768%2C1661&amp;ssl=1 768w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=710%2C1536&amp;ssl=1 710w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=1100%2C2379&amp;ssl=1 1100w" data-recalc-dims="1" height="2048" src="https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=947%2C2048&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="947"/>
   <noscript>
    <img alt="" class="aligncenter size-full wp-image-15904" data-recalc-dims="1" height="2048" sizes="(max-width: 947px) 100vw, 947px" src="https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=947%2C2048&amp;ssl=1" srcset="https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?w=947&amp;ssl=1 947w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=139%2C300&amp;ssl=1 139w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=473%2C1024&amp;ssl=1 473w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=768%2C1661&amp;ssl=1 768w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=710%2C1536&amp;ssl=1 710w, https://i1.wp.com/www.iyouport.org/wp-content/uploads/2021/01/20210131-054616.png?resize=1100%2C2379&amp;ssl=1 1100w" width="947"/>
   </noscript>
  </p>
  <p class="graf graf--p">
   在本文中，null-byte尝试使用我们曾经介绍过的工具 “蜘蛛脚” 进行加密货币追踪调查，关于蜘蛛脚，见《
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%87%aa%e5%8a%a8%e6%89%a7%e8%a1%8c%e6%83%85%e6%8a%a5%e6%90%9c%e9%9b%86%ef%bc%9f%e8%9c%98%e8%9b%9b%e8%84%9a%e5%85%a5%e9%97%a8%e6%8c%87%e5%8d%97/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%87%aa%e5%8a%a8%e6%89%a7%e8%a1%8c%e6%83%85%e6%8a%a5%e6%90%9c%e9%9b%86%ef%bc%9f%e8%9c%98%e8%9b%9b%e8%84%9a%e5%85%a5%e9%97%a8%e6%8c%87%e5%8d%97/" rel="noopener" target="_blank">
    如何自动执行情报搜集？蜘蛛脚入门指南
   </a>
   》、《
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e6%8f%ad%e9%9c%b2%e5%8a%a0%e5%af%86%e8%b4%a7%e5%b8%81%e6%8a%95%e8%b5%84%e9%aa%97%e5%b1%80%ef%bc%9a%e8%9c%98%e8%9b%9b%e8%84%9a%e6%bc%94%e7%a4%ba%e8%87%aa%e5%8a%a8%e5%8c%96%e5%bc%80%e6%ba%90%e6%83%85/" href="https://www.iyouport.org/%e6%8f%ad%e9%9c%b2%e5%8a%a0%e5%af%86%e8%b4%a7%e5%b8%81%e6%8a%95%e8%b5%84%e9%aa%97%e5%b1%80%ef%bc%9a%e8%9c%98%e8%9b%9b%e8%84%9a%e6%bc%94%e7%a4%ba%e8%87%aa%e5%8a%a8%e5%8c%96%e5%bc%80%e6%ba%90%e6%83%85/" rel="noopener" target="_blank">
    揭露加密货币投资骗局：蜘蛛脚演示自动化开源情报调查
   </a>
   》。
  </p>
  <p class="graf graf--p">
   SpiderFoot 总体上是一个很好的自动化
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/category/osint/" href="https://www.iyouport.org/category/osint/" rel="noopener" target="_blank">
    开源情报工具
   </a>
   ，它有两个不同的版本：免费的开源项目和一个付费服务 SpiderFoot HX，一年的费用差不多是800美元。对于本文的使用来说，免费版本足以调查比特币钱包和余额，而且不需要运行一个网络服务器来进行调查，如果您在命令行界面之外使用 SpiderFoot，这一点是必要的。
  </p>
  <p class="graf graf--p">
   比方说，一个组织正在使用比特币筹集资金。不管是合法的还是非法的组织募捐，您都可以先通过刮取网站来定位任何与该组织的域名相关联的比特币钱包地址来监控它的表现。然后，您可以将这些数据传递到一个查询中，找出每个面向公众的钱包中的确切余额。
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="449" src="//www.youtube.com/embed/Z2zmvA-ieQc" width="800">
   </iframe>
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     需要什么
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   要使用 SpiderFoot 的CLI，您需要安装Python 3，新的 Linux、macOS 和 Windows 系统都预装了Python 3。如果没有，或者您有一个旧版本的 Python，Python 3 很容易
   <a class="markup--anchor markup--p-anchor" data-href="https://www.python.org/downloads/" href="https://www.python.org/downloads/" rel="noopener" target="_blank">
    下载和安装
   </a>
   。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff99cc;">
    <strong class="markup--strong markup--p-strong">
     步骤1：安装 SpiderFoot
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   我们不打算去
   <a class="markup--anchor markup--p-anchor" data-href="https://www.spiderfoot.net/" href="https://www.spiderfoot.net/" rel="noopener" target="_blank">
    SpiderFoot 的网站
   </a>
   上获取这个工具。相反，我们将从
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/smicallef/spiderfoot" href="https://github.com/smicallef/spiderfoot" rel="noopener" target="_blank">
    它的 GitHub 库
   </a>
   中获取。除了本文要做的事之外，SpiderFoot 还有很多好用的地方，所以一定要去它的 GitHub 看看它还能做什么。
  </p>
  <p class="graf graf--p">
   它还有一个 SpiderFoot 可以使用的模块列表，这些模块可以组合在一起，以执行非常具体的搜索查询。
  </p>
  <p class="graf graf--p">
   我们稍后将使用两个模块：一个是搜索网站上的比特币地址，另一个是将这些地址传递给余额查询。但首先，要通过
   <strong class="markup--strong markup--p-strong">
    git
   </strong>
   下载 SpiderFoot，在终端发出以下命令：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ git clone https://github.com/smicallef/spiderfoot.git

Cloning into 'spiderfoot'...
remote: Enumerating objects: 43, done.
remote: Counting objects: 100% (43/43), done.
remote: Compressing objects: 100% (36/36), done.
remote: Total 20781 (delta 17), reused 18 (delta 7), pack-reused 20738
Receiving objects: 100% (20781/20781), 13.89 MiB | 9.34 MiB/s, done.
Resolving deltas: 100% (16727/16727), done.</code></pre>
  <p class="graf graf--p">
   然后，转到其目录和执行列表 (
   <strong class="markup--strong markup--p-strong">
    ls
   </strong>
   ).
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ cd spiderfoot
~/spiderfoot$ ls

dicts                 modules                sfcli.py    static
Dockerfile            passwd                 sflib.py    test
dyn                   README.md              sf.py       THANKYOU
generate-certificate  requirements_test.txt  sfscan.py   VERSION
LICENSE               requirements.txt       sfwebui.py
log                   setup.cfg              spiderfoot</code></pre>
  <p class="graf graf--p">
   您可以看到一个 requirements.txt 文件，所以在继续之前确保用
   <strong class="markup--strong markup--p-strong">
    pip3
   </strong>
   安装它。如果不这样做 SpiderFoot 有可能会失败，因为它没有正确运行所需的所有依赖项。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~/spiderfoot$ pip3 install -r requirements.txt

Defaulting to user installation because normal site-packages is not writeable
Requirement already satisfied: adblockparser&gt;=0.7 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 1)) (0.7)
Requirement already satisfied: dnspython&gt;=1.16.0 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 2)) (2.0.0)
Requirement already satisfied: exifread&gt;=2.1.2 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 3)) (2.3.2)
Requirement already satisfied: CherryPy&gt;=18.0 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 4)) (18.6.0)
Requirement already satisfied: cherrypy-cors&gt;=1.6 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 5)) (1.6)
Requirement already satisfied: Mako&gt;=1.0.4 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 6)) (1.1.3)
Requirement already satisfied: beautifulsoup4&gt;=4.4.1 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 7)) (4.9.3)
Requirement already satisfied: lxml&gt;=4.6.1 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 8)) (4.6.1)
Requirement already satisfied: netaddr&gt;=0.7.18 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 9)) (0.7.19)
Requirement already satisfied: pysocks&gt;=1.7.1 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 10)) (1.7.1)
Requirement already satisfied: requests&gt;=2.20.0 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 11)) (2.24.0)
Requirement already satisfied: ipwhois==1.0.0 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 12)) (1.0.0)
Requirement already satisfied: ipaddr&gt;=2.2.0 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 13)) (2.2.0)
Requirement already satisfied: phonenumbers&gt;=8.12.9 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 14)) (8.12.13)
Requirement already satisfied: pygexf&gt;=0.2.2 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 15)) (0.2.2)
Requirement already satisfied: PyPDF2&gt;=1.26.0 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 16)) (1.26.0)
Requirement already satisfied: stem&gt;=1.7.1 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 17)) (1.8.0)
Requirement already satisfied: python-whois&gt;=0.7.1 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 18)) (0.7.3)
Requirement already satisfied: secure&gt;=0.2.1 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 19)) (0.2.1)
Requirement already satisfied: pyOpenSSL&gt;=17.5.0 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 20)) (19.1.0)
Requirement already satisfied: python-docx&gt;=0.8.10 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 21)) (0.8.10)
Requirement already satisfied: python-pptx&gt;=0.6.18 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 22)) (0.6.18)
Requirement already satisfied: networkx&gt;=2.5 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 23)) (2.5)
Requirement already satisfied: cryptography&gt;=3.2.1 in /usr/lib/python3/dist-packages (from -r requirements.txt (line 24)) (3.2.1)
Requirement already satisfied: publicsuffixlist&gt;=0.7.3 in /home/kali/.local/lib/python3.8/site-packages (from -r requirements.txt (line 25)) (0.7.5)
Requirement already satisfied: portend&gt;=2.1.1 in /home/kali/.local/lib/python3.8/site-packages (from CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (2.7.0)
Requirement already satisfied: more-itertools in /usr/lib/python3/dist-packages (from CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (4.2.0)
Requirement already satisfied: zc.lockfile in /home/kali/.local/lib/python3.8/site-packages (from CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (2.0)
Requirement already satisfied: cheroot&gt;=8.2.1 in /home/kali/.local/lib/python3.8/site-packages (from CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (8.4.7)
Requirement already satisfied: jaraco.collections in /home/kali/.local/lib/python3.8/site-packages (from CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (3.0.0)
Requirement already satisfied: httpagentparser&gt;=1.5 in /home/kali/.local/lib/python3.8/site-packages (from cherrypy-cors&gt;=1.6-&gt;-r requirements.txt (line 5)) (1.9.0)
Requirement already satisfied: soupsieve&gt;1.2 in /usr/lib/python3/dist-packages (from beautifulsoup4&gt;=4.4.1-&gt;-r requirements.txt (line 7)) (2.0.1)
Requirement already satisfied: future in /usr/lib/python3/dist-packages (from python-whois&gt;=0.7.1-&gt;-r requirements.txt (line 18)) (0.18.2)
Requirement already satisfied: tempora&gt;=1.8 in /home/kali/.local/lib/python3.8/site-packages (from portend&gt;=2.1.1-&gt;CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (4.0.1)
Requirement already satisfied: setuptools in /usr/lib/python3/dist-packages (from zc.lockfile-&gt;CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (50.3.0)
Requirement already satisfied: jaraco.functools in /home/kali/.local/lib/python3.8/site-packages (from cheroot&gt;=8.2.1-&gt;CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (3.0.1)
Requirement already satisfied: six&gt;=1.11.0 in /usr/lib/python3/dist-packages (from cheroot&gt;=8.2.1-&gt;CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (1.15.0)
Requirement already satisfied: jaraco.text in /home/kali/.local/lib/python3.8/site-packages (from jaraco.collections-&gt;CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (3.2.0)
Requirement already satisfied: jaraco.classes in /home/kali/.local/lib/python3.8/site-packages (from jaraco.collections-&gt;CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (3.1.0)
Requirement already satisfied: pytz in /usr/lib/python3/dist-packages (from tempora&gt;=1.8-&gt;portend&gt;=2.1.1-&gt;CherryPy&gt;=18.0-&gt;-r requirements.txt (line 4)) (2020.4)</code></pre>
  <p class="graf graf--p">
   如果您通过上面的命令安装有问题，可以先用
   <strong class="markup--strong markup--p-strong">
    apt update
   </strong>
   试试，然后再继续。如果仍然有问题，请在前面运行
   <strong class="markup--strong markup--p-strong">
    sudo
   </strong>
   命令。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff99cc;">
    <strong class="markup--strong markup--p-strong">
     步骤2：确保 SpiderFoot 工作正常
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在 SpiderFoot 已经全部准备好了，是时候开始使用它了，用命令行参数传递我们希望返回的信息。从上面执行的列表中，您会看到 sf.py 文件，这就是我们将在这里使用的主要程序。试着运行它一下，看看它是否能正常工作：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~/spiderfoot$ python3 ./sf.py

You must specify a target when running in scan mode. Try --help for guidance.</code></pre>
  <p class="graf graf--p">
   如果您看到了其他东西，或者如果您现在或在后面的步骤中遇到了错误，可以返回去用
   <strong class="markup--strong markup--p-strong">
    pip3
   </strong>
   重新安装 request.txt。如果还不行，就用
   <strong class="markup--strong markup--p-strong">
    sudo
   </strong>
   安装，这样应该可以修复任何丢失的模块。
  </p>
  <p class="graf graf--p">
   现在，让我们快速浏览一下帮助页面，看看使用说明。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~/spiderfoot$ python3 ./sfcli.py --help

usage: sf.py [-h] [-d] [-l IP:port] [-m mod1,mod2,...] [-M] [-s TARGET]
             [-t type1,type2,...] [-T] [-o tab|csv|json] [-n] [-r] [-S LENGTH]
             [-D DELIMITER] [-f] [-F FILTER] [-x] [-q]

SpiderFoot 3.0: Open Source Intelligence Automation.

optional arguments:
  -h, --help          show this help message and exit
  -d, --debug         Enable debug output.
  -l IP:port          IP and port to listen on.
  -m mod1,mod2,...    Modules to enable.
  -M, --modules       List available modules.
  -s TARGET           Target for the scan.
  -t type1,type2,...  Event types to collect.
  -T, --types         List available event types.
  -o tab|csv|json     Output format. Tab is default.
  -n                  Strip newlines from data.
  -r                  Include the source data field in tab/csv output.
  -S LENGTH           Maximum data length to display. By default, all data is
                      shown.
  -D DELIMITER        Delimiter to use for CSV output. Default is ,.
  -f                  Filter out other event types that weren't requested with
                      -t.
  -F FILTER           Filter out a set of event types.
  -x                  STRICT MODE. Will only enable modules that can directly
                      consume your target, and if -t was specified only those
                      events will be consumed by modules. This overrides -t
                      and -m options.
  -q                  Disable logging.</code></pre>
  <h3 class="graf graf--p">
   <span style="color: #ff99cc;">
    <strong class="markup--strong markup--p-strong">
     步骤3：扫描比特币地址和余额
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在来看一个比特币地址和钱包余额，这是我们从一个网站上搜到的。我们要把几个东西链接在一起才行。这就是模块发挥作用的地方。
  </p>
  <pre class="graf graf--pre"><code>~/spiderfoot$ python3 ./sf.py -m sfp_spider,sfp_bitcoin,sfp_blockchain -s websiteurl.com -F -q BITCOIN_ADDRESS,BITCOIN_BALANCE -q</code></pre>
  <p class="graf graf--p">
   在上面您可以看到我们正在使用的命令。命令的第一部分是用 Python 3 启动 SpiderFoot 工具。
   <strong class="markup--strong markup--p-strong">
    -m
   </strong>
   表示您使用的是一个或多个模块，在它后面就是模块，用逗号隔开。
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    sfp_spider
   </strong>
   模块会对我们要扫描的网站网页进行蜘蛛式搜索，找到里面的所有信息。
   <strong class="markup--strong markup--p-strong">
    sfp_bitcoin
   </strong>
   模块会将通过 spidering 找到的所有比特币钱包地址隔离出来。而
   <strong class="markup--strong markup--p-strong">
    sfp_blockchain
   </strong>
   模块将把比特币地址传递给API，由API来确定钱包中存储的具体金额。
  </p>
  <p class="graf graf--p">
   接下来在命令中，使用
   <strong class="markup--strong markup--p-strong">
    -s
   </strong>
   ，后面是网站URL，这将让我们选择目标网站。然后，用
   <strong class="markup--strong markup--p-strong">
    -F
   </strong>
   来过滤出一组事件类型，特别是
   <strong class="markup--strong markup--p-strong">
    BITCOIN_ADDRESS
   </strong>
   和
   <strong class="markup--strong markup--p-strong">
    BITCOIN_BALANCE
   </strong>
   。这就是我们要找的信息。最后，
   <strong class="markup--strong markup--p-strong">
    -q
   </strong>
   用来隐藏输出中的所有信息，除了我们想要的东西。
  </p>
  <p class="graf graf--p">
   现在以 bitcoinforcharity.com 为例，在一个真实的网站上运行它。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~/spiderfoot$ python3 ./sf.py -m sfp_spider,sfp_bitcoin,sfp_blockchain -s bitcoinforcharity.com -F BITCOIN_ADDRESS,BITCOIN_BALANCE -q

Source                          Type                                            Data
sfp_bitcoin                     Bitcoin Address                                 1HesYJSP1QqcyPEjnQ9vzBL1wujruNGe7R
sfp_blockchain                  Bitcoin Balance                                 0.00021 BTC
sfp_bitcoin                     Bitcoin Address                                 16Sy8mvjyNgCRYS14m1Rtca3UfrFPzz9eJ
sfp_blockchain                  Bitcoin Balance                                 0.24481116 BTC
sfp_bitcoin                     Bitcoin Address                                 1M72Sfpbz1BPpXFHz9m3CdqATR44Jvaydd
sfp_blockchain                  Bitcoin Balance                                 1.62908644 BTC
sfp_bitcoin                     Bitcoin Address                                 1946W6LDsEYF9B5sPYDKfwLw6YBZuHns4L
sfp_blockchain                  Bitcoin Balance                                 0.02344126 BTC
sfp_bitcoin                     Bitcoin Address                                 1PC9aZC4hNX2rmmrt7uHTfYAS3hRbph4UN
sfp_blockchain                  Bitcoin Balance                                 1.89378293 BTC
sfp_bitcoin                     Bitcoin Address                                 1PAt5oKQGBRigFDY6fB2WgQTtQJNzFyTDr
sfp_blockchain                  Bitcoin Balance                                 0.0 BTC
sfp_bitcoin                     Bitcoin Address                                 1NgiUwkhYVYMy3eoMC9dHcvdHejGxcuaWm
sfp_blockchain                  Bitcoin Balance                                 0.06070947 BTC
sfp_bitcoin                     Bitcoin Address                                 1M87hiTAa49enJKVeT9gzLjYmJoYh9V98
sfp_blockchain                  Bitcoin Balance                                 0.0 BTC
sfp_bitcoin                     Bitcoin Address                                 1CU5YgjquupDw6UeXEyA9VEBH34R7fZ19b
sfp_blockchain                  Bitcoin Balance                                 0.16549195 BTC
sfp_bitcoin                     Bitcoin Address                                 16DEzKc9fX4XfgGzEvQUJmoYeUrbRNXqxe
sfp_blockchain                  Bitcoin Balance                                 0.18967667 BTC
sfp_bitcoin                     Bitcoin Address                                 1AS3TiTqgJZK6CfNfqcbPXSx4PTFvfghvF
sfp_blockchain                  Bitcoin Balance                                 0.0 BTC
sfp_bitcoin                     Bitcoin Address                                 1Archive1n2C579dMsAu3iC6tWzuQJz8dN
sfp_blockchain                  Bitcoin Balance                                 3.17865301 BTC</code></pre>
  <p class="graf graf--p">
   从上面的输出中可以看到，该慈善机构有多个公开的比特币地址，由此我们看到确切的比特币钱包的金额。该机构并没有真正筹集到任何比特币，3.17865301 BTC 是最多的金额。如果您正在寻找一个通过加密货币转移大量资金的网站，这里的数字会很大。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff99cc;">
    <strong class="markup--strong markup--p-strong">
     步骤4：扫描 Ethereum 地址
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   对于 Ethereum 来说，您可以使用不同的命令结构来获取网站上发现的所有钱包地址，但您将无法像比特币那样获得任何余额。为了快速演示，我们将扫描 etherdonation.com。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~/spiderfoot$ python3 ./sf.py -m sfp_spider,sfp_ethereum -s etherdonation.com -F ETHEREUM_ADDRESS -q

Source                          Type                                            Data
sfp_ethereum                    Ethereum Address                                0xed6ca7d908f897d0b0d5f9b9e7aa470698e10b1b
sfp_ethereum                    Ethereum Address                                0xed6ca7d908f897d0b0d5f9b9e7aa470698e10b1b
sfp_ethereum                    Ethereum Address                                0xed6ca7d908f897d0b0d5f9b9e7aa470698e10b1b
sfp_ethereum                    Ethereum Address                                0xed6ca7d908f897d0b0d5f9b9e7aa470698e10b1b
sfp_ethereum                    Ethereum Address                                0xed6ca7d908f897d0b0d5f9b9e7aa470698e10b1b
sfp_ethereum                    Ethereum Address                                0xed6ca7d908f897d0b0d5f9b9e7aa470698e10b1b</code></pre>
  <p class="graf graf--p">
   这里所做的只是使用 sfp_spider 和 Spider-ether 模块、以及以太坊发现模块 sfp_ethereum。而且去掉了余额的过滤器，因为我们找不到 Ethereum 的余额。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     简单而强大
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   如果您想看到一些比特币交易量最大的组织，您可以在 google 上搜索类似 “top 100 bitcoin addresses” 这样的东西，然后选择一个排名靠前的结果进行监测。然后，您可以在命令中使用该网站的URL来查看哪些比特币地址的BTC移动量最大。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://null-byte.wonderhowto.com/how-to/extract-bitcoin-wallet-addresses-balances-from-websites-with-spiderfoot-cli-0238107/" href="https://null-byte.wonderhowto.com/how-to/extract-bitcoin-wallet-addresses-balances-from-websites-with-spiderfoot-cli-0238107/" rel="noopener" target="_blank">
    Extract Bitcoin Wallet Addresses &amp; Balances from Websites with SpiderFoot CLI
   </a>
  </p>
  <div id="atatags-1611829871-60afa2869b1d5">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-15903" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8-spiderfoot-cli-%e4%bb%8e%e7%bd%91%e7%ab%99%e6%8f%90%e5%8f%96%e6%af%94%e7%89%b9%e5%b8%81%e9%92%b1%e5%8c%85%e5%9c%b0%e5%9d%80%e5%92%8c%e4%bd%99%e9%a2%9d/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-15903" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8-spiderfoot-cli-%e4%bb%8e%e7%bd%91%e7%ab%99%e6%8f%90%e5%8f%96%e6%af%94%e7%89%b9%e5%b8%81%e9%92%b1%e5%8c%85%e5%9c%b0%e5%9d%80%e5%92%8c%e4%bd%99%e9%a2%9d/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-15903-60afa2869b93a" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=15903&amp;origin=www.iyouport.org&amp;obj_id=161182987-15903-60afa2869b93a" id="like-post-wrapper-161182987-15903-60afa2869b93a">
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
    <a href="https://www.iyouport.org/tag/bitcoin/" rel="tag">
     bitcoin
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
    <a href="https://www.iyouport.org/tag/spiderfoot/" rel="tag">
     Spiderfoot
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
   <time class="entry-date published" datetime="2021-04-28T00:04:01+08:00">
    2021年4月28日
   </time>
   <time class="updated" datetime="2021-01-31T15:04:14+08:00">
    2021年1月31日
   </time>
  </div>
 </div>
</article>

