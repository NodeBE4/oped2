---
layout: post
title: "翻墙七种武器之霸王枪：Shadowsocks"
date: 2014-07-11T08:28:52+02:00
author: Vergil
from: https://pao-pao.net/article/130
tags: [ 泡泡 ]
categories: [ 泡泡 ]
---

<section class="clearfix" id="content" role="main">
 <div class="region region-content">
  <div class="block block-system" id="block-system-main">
   <div class="content">
    <div about="/article/130" class="node node-pao-pao-article node-promoted node-full view-mode-full clearfix" id="node-130" typeof="sioc:Item foaf:Document">
     <span class="rdf-meta element-hidden" content="翻墙七种武器之霸王枪：Shadowsocks" property="dc:title">
     </span>
     <span class="rdf-meta element-hidden" content="3" datatype="xsd:integer" property="sioc:num_replies">
     </span>
     <div class="submitted">
      <span content="2014-07-11T08:28:52+02:00" datatype="xsd:dateTime" property="dc:date dc:created" rel="sioc:has_creator">
       <a about="/author/30" class="username" datatype="" href="/author/30" property="foaf:name" title="查看用户资料" typeof="sioc:UserAccount" xml:lang="">
        Vergil
       </a>
       在 星期五, 07/11/2014 - 08:28 提交
      </span>
     </div>
     <div class="content">
      <div class="field field-name-field-image field-type-image field-label-hidden">
       <div class="field-items">
        <div class="field-item even">
         <div class="file file-image file-image-jpeg" id="file-313--2">
          <h2 class="element-invisible">
           <a href="/file/313">
            shadowsocks.jpg
           </a>
          </h2>
          <div class="content">
           <img alt="" height="164" src="https://pao-pao.net/sites/pao-pao.net/files/styles/article_detail/public/shadowsocks.jpg?itok=OOEMBiW1" title="" typeof="foaf:Image" width="290"/>
          </div>
         </div>
        </div>
       </div>
      </div>
      <div class="field field-name-title field-type-ds field-label-hidden">
       <div class="field-items">
        <div class="field-item even" property="dc:title">
         <h1 class="page-title">
          翻墙七种武器之霸王枪：Shadowsocks
         </h1>
        </div>
       </div>
      </div>
      <div class="field-name-author">
       <div class="label-inline">
        文/
       </div>
       <a about="/author/30" class="username" datatype="" href="/author/30" property="foaf:name" title="查看用户资料" typeof="sioc:UserAccount" xml:lang="">
        Vergil
       </a>
      </div>
      <div class="field field-name-body field-type-text-with-summary field-label-hidden">
       <div class="field-items">
        <div class="field-item even" property="content:encoded">
         <p>
          古龙先生在《七种武器之霸王枪》一文中是这样描述这把神兵利刃的，“霸王。力拔山兮气盖世。枪，百兵之祖是为枪，霸王枪长一丈三尺七寸三分，重七十三斤七两三钱。江湖中其实很少有人亲眼见到这霸王枪。可是江湖中每个人都知道，世上最霸道的七种兵器，就有一种是霸王枪。普天之下，独一无二的霸王枪。”
          <br/>
          <br/>
          随着今年六月以来大陆网络环境进一步恶化，Google 全系列产品再次被干扰至今无法正常使用，导致依托于
          <a href="https://appengine.google.com/" rel="nofollow">
           Google App Agine
          </a>
          的
          <a href="https://pao-pao.net/node/111" rel="nofollow">
           Goagent
          </a>
          也变得不听使唤，而
          <a href="https://www.getlantern.org/" rel="nofollow" target="_blank">
           Lantern
          </a>
          被墙之后一直未能恢复元气，免费翻墙工具们第一次遇到全方位的威胁。
          <br/>
          <br/>
          如果实在不想掏钱去买那些专业的商用翻墙服务，同时自己或身边的朋友手头上空闲一台
          <strong>
           VPS
          </strong>
          ，如果对 Linux 系统命令行有一个基本的认识，那么你可以尝试在VPS服务器上自行搭建
          <a href="https://github.com/clowwindy/shadowsocks" rel="nofollow" target="_blank">
           Shadowsocks
          </a>
          （Goagent是搭建在Google服务器上的）。或者说你不愿意耗费精力搭建，可以直接跳过本文中“服务器设置端”的内容，直接看“本地客户端”设置，然后填入公共服务器的地址，同样可以享受到免费快速的翻墙服务。
          <br/>
          <br/>
          Shadowssocks采用socks代理，设置虽然复杂，但翻墙效果稳定流畅，比Http代理更难以识别，多平台支持，目前难以为GFW所屏蔽。正如霸王枪一样，虽然沉重无比难以施展，但如果被具备天生神力的西楚霸王项羽所用，则立时化成一柄横扫千军、所向披靡无往不胜的百兵之王。
          <br/>
          <br/>
          <strong>
           一、配置环境准备
          </strong>
         </p>
         <ul>
          <li>
           一台闲置的VPS,可以使用免费试用一年的
           <a href="https://aws.amazon.com/ec2/" rel="nofollow" target="_blank">
            Amazon EC2
           </a>
           主机，也可以使用便宜的
           <a href="https://www.digitalocean.com/" rel="nofollow" target="_blank">
            DigitalOcean
           </a>
           最低配的新加坡主机
          </li>
          <li>
           VPS上预装好 linux 系统，可以是 Debain 或 Ubuntu，我们这里以流行的
           <a href="https://pao-pao.net/node/119" rel="nofollow">
            <strong>
             Ubuntu
            </strong>
           </a>
           为例；
          </li>
          <li>
           具备基本的命令行基础和纯文本编辑能力。
          </li>
         </ul>
         <p>
          <strong>
           二、服务器端设置
          </strong>
         </p>
         <p>
          首先确保系统安装了 Python 2.6 或2.7：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
           </td>
           <td>
            <p>
             python –version
            </p>
           </td>
          </tr>
         </table>
         <p>
          下面开始安装软件包：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
            <p>
             2
            </p>
           </td>
           <td>
            <p>
             apt-get install build-essential python-pip python-m2crypto python-dev
            </p>
            <p>
             pip install gevent shadowsocks
            </p>
           </td>
          </tr>
         </table>
         <p>
          创建一个配置文件 /etc/shadowsocks.json
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
            <p>
             2
            </p>
            <p>
             3
            </p>
            <p>
             4
            </p>
            <p>
             5
            </p>
            <p>
             6
            </p>
            <p>
             7
            </p>
            <p>
             8
            </p>
            <p>
             9
            </p>
           </td>
           <td>
            <p>
             "server":"服务器 IP 地址",     #VPS的IP地址
            </p>
            <p>
             "server_port":8388,     #监听的端口
            </p>
            <p>
             "local_address": "127.0.0.1",     #本地监听的IP地址，默认为主机
            </p>
            <p>
             "local_port":1080,                #本地监听的端口
            </p>
            <p>
             "password":"mypassword",          #服务密码
            </p>
            <p>
             "timeout":300,                    #用于加密的密码
            </p>
            <p>
             "method":"aes-256-cfb",           #加密方法，推荐 "aes-256-cfb"
            </p>
            <p>
             "fast_open": false,               #是否使用 TCP_FASTOPEN, true / false
            </p>
            <p>
             "workers": 1     #worker 数量，Unix/Linux 可用，如果不理解含义请不要改
            </p>
           </td>
          </tr>
         </table>
         <p>
          设置完毕保存配置文件，然后在命令行下输入：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
           </td>
           <td>
            <p>
             ssserver -c /etc/shadowsocks.json
            </p>
           </td>
          </tr>
         </table>
         <p>
          为了保证此项服务一直在后台运行，可以使用
          <a href="http://supervisord.org/" rel="nofollow" target="_blank">
           Supervisor
          </a>
          工具：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
           </td>
           <td>
            <p>
             nano /etc/supervisor/conf.d/shadowsocks.conf
            </p>
           </td>
          </tr>
         </table>
         <p>
          新建 Supervisor 的配置文件
          <strong>
           shadowsocks.conf
          </strong>
          ：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
            <p>
             2
            </p>
            <p>
             3
            </p>
            <p>
             4
            </p>
           </td>
           <td>
            <p>
             [program:shadowsocks]
            </p>
            <p>
             command=ssserver -c /etc/shadowsocks.json
            </p>
            <p>
             autorestart=true
            </p>
            <p>
             user=nobody
            </p>
           </td>
          </tr>
         </table>
         <p>
          继续编辑这个文件/etc/default/supervisor，并在文件末尾添加如下代码：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
           </td>
           <td>
            <p>
             ulimit -n 51200
            </p>
           </td>
          </tr>
         </table>
         <p>
          更新服务，开始运行：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
            <p>
             2
            </p>
           </td>
           <td>
            <p>
             service supervisor start
            </p>
            <p>
             supervisorctl reload
            </p>
           </td>
          </tr>
         </table>
         <p>
          下面的命令告诉你如何结束以及重新启动 Shadowsocks 服务：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
            <p>
             2
            </p>
           </td>
           <td>
            <p>
             supervisorctl stop shadowsocks
            </p>
            <p>
             supervisorctl start shadowsocks
            </p>
           </td>
          </tr>
         </table>
         <p>
          你也可以通过下面命令来查看此进程的日志文件：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
           </td>
           <td>
            <p>
             supervisorctl tail -f shadowsocks stderr
            </p>
           </td>
          </tr>
         </table>
         <p>
          你也可以通过访问 VPS 的9001端口查看系统运行状态，关于 Supervisor 更多的命令使用可以访问它的
          <a href="http://supervisord.org/" rel="nofollow">
           官方网站
          </a>
          。
         </p>
         <p>
          好了，服务器端的设置完毕了，下面进入客户端（本地）设置环节：
         </p>
         <p>
          <strong>
           三、本地设置
          </strong>
         </p>
         <p>
          服务器正常运行后，我们还需要在本地电脑上安装客户端进行转发，和使用 SSH 翻墙的原理如出一辙，首先根据本地电脑系统的情况进入
          <a href="https://github.com/clowwindy/shadowsocks/wiki/Ports-and-Clients" rel="nofollow" target="_blank">
           此页面
          </a>
          下载对应的客户端：
         </p>
         <p>
          下载完成后运行，然后依次填入上面 shadowsocks.json 配置文件中的选项，然后保存，可以看到客户端提示已连接：
         </p>
         <p>
         </p>
         <div class="media media-element-container media-full">
          <div class="ds-1col file file-image file-image-png view-mode-full clearfix">
           <img alt="" class="media-element file-full" height="458" src="https://pao-pao.net/sites/pao-pao.net/files/styles/large/public/vpn_0.png?itok=ewJLZme1" title="" typeof="foaf:Image" width="480"/>
          </div>
         </div>
         <p>
          接下来我们需要再 Firefox 和 Chrome 客户端上安装好
          <a href="https://addons.mozilla.org/zh-cn/firefox/addon/autoproxy/" rel="nofollow" target="_blank">
           AutoProxy
          </a>
          或
          <a href="https://chrome.google.com/webstore/detail/proxy-switchysharp/dpplabbmogkhghncfbfdeeokoefdjegm?hl=zh-CN" rel="nofollow" target="_blank">
           Proxy SwitchySharp
          </a>
          插件，然后进行如下设置：
         </p>
         <table>
          <tr>
           <td>
            <p>
             1
            </p>
            <p>
             2
            </p>
            <p>
             3
            </p>
           </td>
           <td>
            <p>
             协议: socks5
            </p>
            <p>
             地址: 127.0.0.1
            </p>
            <p>
             端口: 你填的 local_port 默认是1080
            </p>
           </td>
          </tr>
         </table>
         <p>
          <strong>
           四、手机平台设置
          </strong>
         </p>
         <p>
          Shadowsocks不仅仅局限于PC桌面应用，它还可以在例如 IOS 和 Android 平台上广泛应用，IOS平台上直接在 Appstore 里搜索“shadowsocks”，app打开之后是一个浏览器，内置了免费的公共服务器，如果公共服务器出现运行不稳定的情况，这时就可以按照上述的方法在VPS中安装好 shadowssocks 就可以翻墙访问了。当然要想全面使用 Socks 代理最好是先越狱。
          <br/>
          <br/>
          Andorid 平台也是如法炮制，只不过在
          <a href="play.google.com/">
           GooglePlay
          </a>
          里要改为
          <strong>
           搜索“影梭”
          </strong>
          ，具体使用方法和IOS平台基本一致，只不过不是在浏览器而是在专有客户端中进行设置。
          <br/>
          <br/>
          虽然整个设置过程比较繁琐，特别是还需要租用VPS并和枯燥的命令行打交道（我估计现在没有几个非专业的计算机课程还在讲DOS了），但只要热爱互联网，乐于接受新鲜事物，特别是对于自由互联网空间的渴望，那么一切都不会成为障碍，还是用《霸王枪》里的一句话送给各位共勉：
         </p>
         <p>
          “
          <strong>
           霸王枪是勇气，一个人只要有勇气去冒险，天下就绝没有不能解决的事
          </strong>
          。”
         </p>
        </div>
       </div>
      </div>
      <div class="field field-name-service-links-displays-group field-type-ds field-label-hidden">
       <div class="field-items">
        <div class="field-item even">
         <div class="service-links">
          <a class="service-links-twitter" href="https://twitter.com/share?url=https%3A//pao-pao.net/article/130&amp;text=%E7%BF%BB%E5%A2%99%E4%B8%83%E7%A7%8D%E6%AD%A6%E5%99%A8%E4%B9%8B%E9%9C%B8%E7%8E%8B%E6%9E%AA%EF%BC%9AShadowsocks" rel="nofollow" title="Share this on Twitter">
           <img alt="Twitter logo" src="https://pao-pao.net/sites/pao-pao.net/themes/rnw_paopao/servicelinks/png/twitter.png" typeof="foaf:Image"/>
          </a>
          <a class="service-links-facebook" href="https://www.facebook.com/sharer.php?u=https%3A//pao-pao.net/article/130&amp;t=%E7%BF%BB%E5%A2%99%E4%B8%83%E7%A7%8D%E6%AD%A6%E5%99%A8%E4%B9%8B%E9%9C%B8%E7%8E%8B%E6%9E%AA%EF%BC%9AShadowsocks" rel="nofollow" title="Share on Facebook">
           <img alt="Facebook logo" src="https://pao-pao.net/sites/pao-pao.net/themes/rnw_paopao/servicelinks/png/facebook.png" typeof="foaf:Image"/>
          </a>
          <a class="service-links-google" href="https://www.google.com/bookmarks/mark?op=add&amp;bkmk=https%3A//pao-pao.net/article/130&amp;title=%E7%BF%BB%E5%A2%99%E4%B8%83%E7%A7%8D%E6%AD%A6%E5%99%A8%E4%B9%8B%E9%9C%B8%E7%8E%8B%E6%9E%AA%EF%BC%9AShadowsocks" rel="nofollow" title="Bookmark this post on Google">
           <img alt="谷歌 logo" src="https://pao-pao.net/sites/pao-pao.net/themes/rnw_paopao/servicelinks/png/google.png" typeof="foaf:Image"/>
          </a>
         </div>
        </div>
       </div>
      </div>
     </div>
     <div class="block block-views related" id="block-views-articles-related-block-1">
      <h2>
       您可能感兴趣的文章
      </h2>
      <div class="content">
       <div class="view view-articles-related view-id-articles_related view-display-id-block_1 related promoted view-dom-id-2545fb67214a50782ca520fe1f608306">
        <div class="view-content">
         <div class="views-row views-row-1 views-row-odd views-row-first">
          <div class="ds-2col node node-pao-pao-article node-promoted node-sticky view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/1001">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/tou__6.jpeg?itok=Idz0AQWf" typeof="foaf:Image" width="160"/>
               </a>
              </div>
             </div>
            </div>
           </div>
           <div class="group-right">
            <div class="field field-name-field-promotitle field-type-text field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <h2>
                <a href="/article/1001">
                 不知不觉中，你已经变成了别人——社交媒体如何改写了你的记忆
                </a>
                <h2>
                </h2>
               </h2>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
         <div class="views-row views-row-2 views-row-even">
          <div class="ds-2col node node-pao-pao-article node-promoted node-sticky view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/833">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/2_tou_.jpeg?itok=sG1HDdN9" typeof="foaf:Image" width="160"/>
               </a>
              </div>
             </div>
            </div>
           </div>
           <div class="group-right">
            <div class="field field-name-field-promotitle field-type-text field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <h2>
                <a href="/article/833">
                 从媒体卖乖到政治品牌化（二）消费者经济时代脆弱的民主
                </a>
                <h2>
                </h2>
               </h2>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
         <div class="views-row views-row-3 views-row-odd">
          <div class="ds-2col node node-pao-pao-article node-promoted node-sticky view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/781">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/tou__26.jpg?itok=-Zg38xYV" typeof="foaf:Image" width="160"/>
               </a>
              </div>
             </div>
            </div>
           </div>
           <div class="group-right">
            <div class="field field-name-field-promotitle field-type-text field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <h2>
                <a href="/article/781">
                 纠错有很高的技术含量 稍有不慎便适得其反，该怎么做？
                </a>
                <h2>
                </h2>
               </h2>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
         <div class="views-row views-row-4 views-row-even views-row-last">
          <div class="ds-2col node node-pao-pao-article node-promoted node-sticky view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/734">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/tou__1.jpg?itok=Y1H6jhyM" typeof="foaf:Image" width="160"/>
               </a>
              </div>
             </div>
            </div>
           </div>
           <div class="group-right">
            <div class="field field-name-field-promotitle field-type-text field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <h2>
                <a href="/article/734">
                 隐私问题四：便捷科技，还是圆形监狱？
                </a>
                <h2>
                </h2>
               </h2>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
     <!-- /.block -->
     <ul class="links inline">
      <li class="comment-add first last active">
       <a class="active" href="/article/130#comment-form" title="分享您有关本文的看法与观点。">
        冒个泡吧！
       </a>
      </li>
     </ul>
     <div class="comment-wrapper" id="comments">
      <h2 class="title">
       评论
      </h2>
      <a id="comment-4068">
      </a>
      <div about="/comment/4068#comment-4068" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Jeaacalay (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-04-23T12:00:28+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期二, 04/23/2019 - 12:00
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/4068#comment-4068" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/4068#comment-4068" rel="bookmark">
          Viagra Vente Libre Andorre JeaPriods
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/130">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             2095 Albuterol Inhaler  &lt;a href=
             <a href="http://cheapviapill.com&gt;viagra">
              http://cheapviapill.com&gt;viagra
             </a>
             online prescription&lt;/a&gt; Cialis Dosage 40 Mg
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/130/4068">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-16007">
      </a>
      <div about="/comment/16007#comment-16007" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            StevElug (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-01T10:38:19+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期六, 06/01/2019 - 10:38
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/16007#comment-16007" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/16007#comment-16007" rel="bookmark">
          On Sale Generic Fedex Macrobid Tablets Medication Stevprople
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/130">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Where To Buy Tab Finasteride Visa Viagra Generika Gesundheit  &lt;a href=
             <a href="http://cialcost.com&gt;generic">
              http://cialcost.com&gt;generic
             </a>
             cialis from india&lt;/a&gt; Cali'S Without Prescription What Does Mexican Amoxicillin Look Like
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/130/16007">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-22273">
      </a>
      <div about="/comment/22273#comment-22273" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Stepthype (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-03T20:50:50+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期一, 06/03/2019 - 20:50
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/22273#comment-22273" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/22273#comment-22273" rel="bookmark">
          Inhouse Pharmacy Amoxicillin EllCauh
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/130">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Tadacip 60mg  &lt;a href=
             <a href="http://drugsed.com&gt;&lt;/a&gt;">
              http://drugsed.com&gt;&lt;/a&gt;
             </a>
             Levitra Orodispersible Healthy Men Viagra Offer Buy Disulfiram Online
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/130/22273">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <h2 class="title comment-form">
       冒个泡吧！
      </h2>
     </div>
    </div>
   </div>
  </div>
  <!-- /.block -->
 </div>
 <!-- /.region -->
</section>

