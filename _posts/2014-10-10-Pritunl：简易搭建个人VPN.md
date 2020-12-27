---
layout: post
title: "Pritunl：简易搭建个人VPN"
date: 2014-10-10T08:04:46+02:00
author: Vergil
from: https://pao-pao.net/article/213
tags: [ 泡泡 ]
categories: [ 泡泡 ]
---

<section class="clearfix" id="content" role="main">
 <div class="region region-content">
  <div class="block block-system" id="block-system-main">
   <div class="content">
    <div about="/article/213" class="node node-pao-pao-article node-promoted node-full view-mode-full clearfix" id="node-213" typeof="sioc:Item foaf:Document">
     <span class="rdf-meta element-hidden" content="Pritunl：简易搭建个人VPN" property="dc:title">
     </span>
     <span class="rdf-meta element-hidden" content="14" datatype="xsd:integer" property="sioc:num_replies">
     </span>
     <div class="submitted">
      <span content="2014-10-10T08:04:46+02:00" datatype="xsd:dateTime" property="dc:date dc:created" rel="sioc:has_creator">
       <a about="/author/30" class="username" datatype="" href="/author/30" property="foaf:name" title="查看用户资料" typeof="sioc:UserAccount" xml:lang="">
        Vergil
       </a>
       在 星期五, 10/10/2014 - 08:04 提交
      </span>
     </div>
     <div class="content">
      <div class="field field-name-field-image field-type-image field-label-hidden">
       <div class="field-items">
        <div class="field-item even">
         <div class="file file-image file-image-png" id="file-489--2">
          <h2 class="element-invisible">
           <a href="/file/489">
            btakoy8cyaaa2go.png_large.png
           </a>
          </h2>
          <div class="content">
           <img alt="" height="164" src="https://pao-pao.net/sites/pao-pao.net/files/styles/article_detail/public/btakoy8cyaaa2go.png_large.png?itok=4RNemeTK" title="" typeof="foaf:Image" width="290"/>
           <div class="field field-name-field-image-source field-type-link-field field-label-hidden">
            <div class="field-items">
             <div class="field-item even">
              <a href="https://pbs.twimg.com/media/BtaKOy8CYAAA2GO.png:large">
               Pritunl 图：推特
              </a>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
      <div class="field field-name-title field-type-ds field-label-hidden">
       <div class="field-items">
        <div class="field-item even" property="dc:title">
         <h1 class="page-title">
          Pritunl：简易搭建个人VPN
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
          一直以来安装 VPN 服务、提供全局加密代理，是租用VPS（虚拟主机）的一个重要用途，无奈各种命令行操作和复杂繁琐的设置过程，让小白们望而却步。特别是当这种技术被广泛运用到翻墙手段中后，国家防火墙 GFW（Great Fire Wall）就通过智能识别判定，加大了对境外 VPN 服务器的限制和干扰：例如搭建最简单但安全性能较之最薄弱 PPTP 方式的 VPN 链接，很早就遭到联通和电信等 ISP 服务商的封杀；前年十八大之后，没有采用混淆技术的 Openvpn 也被干扰很难使用，因此让更多的初级用户转向其他翻墙手段，或者购买商业付费服务。
          <br/>
          <br/>
          那么有没有一种简单有效的VPN方式，一方面能有一个相对简单的途径，易于初级用户迅速搭建 VPN 服务；另一方面有能抵御 GFW 的干扰，提供稳定有效的代理服务呢？最近我们找到一款免费开源的 VPN 平台软件—
          <a href="https://pritunl.com/#promo" rel="nofollow">
           Pritunl
          </a>
          ，非常符合上述两个要求。
          <br/>
          <br/>
          访问它的
          <a href="https://pritunl.com/#promo" rel="nofollow">
           官网
          </a>
          ，界面非常美观简洁，它采用 OpenVPN 代理方式，一方面提供了 API 供高级开发者使用，同时还针对不同平台和不同 VPS 供应商（包括
          <a href="https://www.digitalocean.com/" rel="nofollow">
           DigitalOcean
          </a>
          和AWS）提供了详尽的安装使用说明，同时我们根据
          <a href="https://pritunl.com/demo/" rel="nofollow">
           官网上提供的测试
          </a>
          发现，此款产品竟然具备图形化界面，方便了初级用户的使用，官方称其能在数分钟内完成搭建过程，这大大的降低了使用门槛。同时，它还提供每月2.5美元的高级会员服务，提供更加强大的功能，我们将在后面予以描述。
          <br/>
          <br/>
          <strong>
           搬瓦工作虚拟主机
          </strong>
          <br/>
          上面已经提到，官网教程中已经为 DigitalOcean 等虚拟主机服务商提供了详细的安装方法，但我们认为如果仅仅是搭建一个 VPN 服务器提供代理服务，那么上述主机中价格最低的 DigitalOcean 最低配的主机每月 5美元的租赁费用还是过高，512M的内存也有浪费之嫌。因此这里，我们使用最近非常火热的搬瓦工（
          <a href="https://bandwagonhost.com/index.php" rel="nofollow">
           BandwagonHost
          </a>
          ）主机作为本次测试的 VPS。
          <br/>
          <br/>
          搬瓦工之所以这么火热，就是因为它低配主机的廉价，非常符合国人搭建代理服务的需求。我们这里选用的是
          <a href="https://bandwagonhost.com/cart.php" rel="nofollow">
           一款内存64M的单核主机
          </a>
          ，年费才3.99美元，平均每个月的开销才2元人民币，1.5G的硬盘和每月100G的流量也完全满足我们需求。它支持信用卡和 Paypal付款，目前有两个美国机房，一个地处东海岸的 Florida 州，一个地处西海岸的 Arizona 州（推荐）。
          <br/>
          <br/>
          价格的便宜不意味着服务的缩水，它带有一个强大的后台管理面板 KiwiVM，可以设置 Two-factor authentication 加强安全性，甚至还可以通过面板直接安装 OpenVPN服务。
          <br/>
          <br/>
          系统默认安装的 CentOS系统，又有编译安装过程太蛋疼，首先通过 KiwiVM 面板重新安装我们更加熟悉的 Ubuntu 12.04 32位系统，然后甚至都不需要使用 Putty ，直接使用面板中的 RootShell-Interactive 就可以进入命令行：
          <br/>
          <br/>
          配置环境
         </p>
         <p>
          1. VPS供应商：
          <a href="https://bandwagonhost.com/index.php" rel="nofollow">
           Bandwagon Host
          </a>
          ；
         </p>
         <p>
          2. VPS配置：1.5G硬盘，单核处理器 64M内存，每月100G流量；
         </p>
         <p>
          3. 服务器系统：Ubuntu 12.04 32位系统；
         </p>
         <p>
          4. 客户端系统：Windows7 64位系统
          <br/>
         </p>
         <div>
          <p>
           <strong>
            一、安装 Pritunl
           </strong>
          </p>
         </div>
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
            <p>
             10
            </p>
            <p>
             11
            </p>
           </td>
           <td>
            <p>
             apt-get update #首先更新软件源
            </p>
            <p>
            </p>
            <p>
             apt-get install -y python-software-properties #安装add-apt-repository工具包
            </p>
            <p>
            </p>
            <p>
             add-apt-repository ppa:pritunl/ppa #添加软件源
            </p>
            <p>
            </p>
            <p>
             apt-get update #更新
            </p>
            <p>
            </p>
            <p>
             apt-get install -y pritunl #安装 pritunl
            </p>
            <p>
            </p>
            <p>
             apt-get upgrade -y #当新版本发布时用此命令进行更新
            </p>
           </td>
          </tr>
         </table>
         <div>
         </div>
         <p>
          <strong>
           二、设置 Pritunl
          </strong>
         </p>
         <p>
          在浏览器中输入：https://&lt;Server_Address&gt;:9700/,注意用自己 VPS 的IP地址进行替换：
          <br/>
          <br/>
          正常情况就应该出现 Pritunl 的登陆界面，默认的用户名和密码都是“Admin”；
          <br/>
          <br/>
          进入“Users”选项卡，点击“Add Organization”输入名称后添加组；
          <br/>
          <br/>
          点击“Add User”命令输入名称后在组下添加用户；
          <br/>
          <br/>
          继续点击“Servers”选项卡，点击“Add Server”输入名称后添加服务器；
          <br/>
          <br/>
          然后点击“Attach Oranization”，将刚新建的组添加到服务器中；
          <br/>
          <br/>
          最后点击“Start Server”运行服务，结束设置环节。
          <br/>
          <br/>
          <br/>
          <strong>
           三、客户端的设置
          </strong>
         </p>
         <p>
          到 OpenVPN 官网上下载 Windows 平台的
          <a href="https://openvpn.net/index.php/open-source/downloads.html" rel="nofollow" target="_blank">
           桌面客户端
          </a>
          并安装；
          <br/>
          <br/>
          进入 Pritunl 设置界面，点击“Users”选项卡，点击用户名右侧的图标下载 OpenVPN 的 Profile设置文件压缩包，里面包含密钥；
          <br/>
          <br/>
          用加压缩软件将其解压，并将 Profile 文件拷贝到 Open configuration file directory目录中；
          <br/>
          <br/>
          以管理员身份运行 OpenVPN（如果用一般用户运行可能会出现无法翻墙的情况），使用配置好的情景链接服务器，成功！
          <br/>
          <br/>
          <strong>
           四、其它
          </strong>
         </p>
         <p>
          1. Pritunl 还提供每个月2.5美元的高级服务，主要功能是提供每个用户产生的流量并以图形化界面反应，如果不是商业运用，这个功能应该和个人用户联系不大，效果如下图：
         </p>
         <p>
         </p>
         <div class="media media-element-container media-original_image">
          <div class="file file-image file-image-jpeg" id="file-488">
           <h2 class="element-invisible">
            <a href="/file/488">
             ev.owa_.jpg
            </a>
           </h2>
           <div class="content">
            <img alt="" class="adaptive-image" height="350" src="https://secure.pao-pao.net/sites/pao-pao.net/files/styles/adaptive_image/adaptive-image/public/ev.owa__1.jpg?itok=UgaDFTOn" title="" typeof="foaf:Image" width="599"/>
           </div>
          </div>
         </div>
         <p>
          2.上述教程是以Ubuntu 12.04作为服务器端系统，以Windows平台作为客户端系统的，其它系统的安装和设置过程请参见
          <a href="https://pritunl.com/tutorial.html" rel="nofollow">
           官方教程
          </a>
          ；
          <br/>
          <br/>
          3.Pritunl为保证安全性还提供了两步认证（ Two-step authenticatioon）；
          <br/>
          <br/>
          4. Pritunl作为VPN服务搭建工具最大的优势就是图形化和简约化，甚至针对目前较为流行的低价主机服务商 DigitalOcean 开发了API接口，能够迅速完成服务器端的搭建和维护。
          <br/>
          <br/>
          5. 上面提到过 Pritunl 采用的 OpenVPN 模式在十八大之后遭遇到一段时间的干扰和屏蔽，但以目前的情况来看链接非常稳定速度也很好，但此款应用刚刚推出，不知道在大规模使用后情况会不会出现逆转，但这一点也妨碍原来高高在上的VPN 搭建过程正逐步向简单化，图形化和普及化方向发展的趋势，在这方面，Pritunl给了我们一个很好的启示和榜样，希望日后类似的应用越来越广泛。
         </p>
         <p>
         </p>
         <p>
         </p>
        </div>
       </div>
      </div>
      <div class="field field-name-service-links-displays-group field-type-ds field-label-hidden">
       <div class="field-items">
        <div class="field-item even">
         <div class="service-links">
          <a class="service-links-twitter" href="https://twitter.com/share?url=https%3A//pao-pao.net/article/213&amp;text=Pritunl%EF%BC%9A%E7%AE%80%E6%98%93%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BAVPN" rel="nofollow" title="Share this on Twitter">
           <img alt="Twitter logo" src="https://pao-pao.net/sites/pao-pao.net/themes/rnw_paopao/servicelinks/png/twitter.png" typeof="foaf:Image"/>
          </a>
          <a class="service-links-facebook" href="https://www.facebook.com/sharer.php?u=https%3A//pao-pao.net/article/213&amp;t=Pritunl%EF%BC%9A%E7%AE%80%E6%98%93%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BAVPN" rel="nofollow" title="Share on Facebook">
           <img alt="Facebook logo" src="https://pao-pao.net/sites/pao-pao.net/themes/rnw_paopao/servicelinks/png/facebook.png" typeof="foaf:Image"/>
          </a>
          <a class="service-links-google" href="https://www.google.com/bookmarks/mark?op=add&amp;bkmk=https%3A//pao-pao.net/article/213&amp;title=Pritunl%EF%BC%9A%E7%AE%80%E6%98%93%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BAVPN" rel="nofollow" title="Bookmark this post on Google">
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
       <div class="view view-articles-related view-id-articles_related view-display-id-block_1 related promoted view-dom-id-06aeb7fcfdeca471ad9c0f345f2ecb49">
        <div class="view-content">
         <div class="views-row views-row-1 views-row-odd views-row-first">
          <div class="ds-2col node node-pao-pao-article node-promoted view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/367">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/xiao_bai_xue_shang_wang_.jpg?itok=4i1B9QRj" typeof="foaf:Image" width="160"/>
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
                <a href="/article/367">
                 技术小白如何选择软件（内附常见软件选择建议）
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
          <div class="ds-2col node node-pao-pao-article node-promoted view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/366">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/da_v_0.jpg?itok=TajJR5I3" typeof="foaf:Image" width="160"/>
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
                <a href="/article/366">
                 大V这次为何没被打倒
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
          <div class="ds-2col node node-pao-pao-article node-promoted view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/114">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/anp-8001154.jpg?itok=6tFFGn9F" typeof="foaf:Image" width="160"/>
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
                <a href="/article/114">
                 长平：“两禁”难禁记者腐败
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
          <div class="ds-2col node node-pao-pao-article node-promoted view-mode-home_promoted_block_ clearfix">
           <div class="group-left">
            <div class="field field-name-field-image field-type-image field-label-hidden">
             <div class="field-items">
              <div class="field-item even">
               <a href="/article/77">
                <img height="90" src="https://pao-pao.net/sites/pao-pao.net/files/styles/home_promoted/public/4816984979_e4fc0fef4b_z_0.jpg?itok=vKsUuFNh" typeof="foaf:Image" width="160"/>
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
                <a href="/article/77">
                 “净网行动”的不列颠经验
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
       <a class="active" href="/article/213#comment-form" title="分享您有关本文的看法与观点。">
        冒个泡吧！
       </a>
      </li>
     </ul>
     <div class="comment-wrapper" id="comments">
      <h2 class="title">
       评论
      </h2>
      <a id="comment-9933">
      </a>
      <div about="/comment/9933#comment-9933" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
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
          <span content="2019-04-24T19:42:58+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期三, 04/24/2019 - 19:42
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/9933#comment-9933" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/9933#comment-9933" rel="bookmark">
          Dogana Kamagra JeaPriods
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Luvox  &lt;a href=
             <a href="http://cheapcial20mg.com&gt;cialis">
              http://cheapcial20mg.com&gt;cialis
             </a>
             20mg for sale&lt;/a&gt; Alcohol Stopping Keflex Levitra Price In Canada Cialis Drogen
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/9933">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-13474">
      </a>
      <div about="/comment/13474#comment-13474" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Randveifs (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-05-31T08:00:27+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期五, 05/31/2019 - 08:00
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/13474#comment-13474" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/13474#comment-13474" rel="bookmark">
          Acquistare Cialis Svizzera LesTreS
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Over Counter Prednisone Cialis Tablets 20mg Cialis Pastiglie  &lt;a href=
             <a href="http://buyviaa.com&gt;viagra">
              http://buyviaa.com&gt;viagra
             </a>
             online prescription&lt;/a&gt; Comprar Cialis En Vina Del Mar Cialis Generico Madrid Levitra Sublinguale Prezzo
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/13474">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-14587">
      </a>
      <div about="/comment/14587#comment-14587" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Matnetela (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-05-31T19:54:54+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期五, 05/31/2019 - 19:54
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/14587#comment-14587" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/14587#comment-14587" rel="bookmark">
          Chewable Kamagra Matnetela
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Levitra Wofur Cialis Ou Viagra Forum  &lt;a href=
             <a href="http://catabs.com&gt;priligy">
              http://catabs.com&gt;priligy
             </a>
             farmacias chile&lt;/a&gt; Buying Levitra Online Reviews
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/14587">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-16595">
      </a>
      <div about="/comment/16595#comment-16595" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            zdorov.bxox.info (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-01T16:30:38+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期六, 06/01/2019 - 16:30
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/16595#comment-16595" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/16595#comment-16595" rel="bookmark">
          zdorov.bxox.info
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Cream wax Health ist eine dickflussige Masse von goldener Farbe, die an eine Art frischen Honigs erinnert.
            </p>
            <p>
             Offiziellen Website:
             <a href="http://zdorov.bxox.info">
              http://zdorov.bxox.info
             </a>
            </p>
            <p>
             кредитная карта --&gt;
             <a href="http://credit.bxox.info">
              http://credit.bxox.info
             </a>
             <br/>
             потребительский кредит--&gt;
             <a href="http://kredit.bxox.info">
              http://kredit.bxox.info
             </a>
             <br/>
             кредитный калькулятор --&gt;
             <a href="http://karta.bxox.info">
              http://karta.bxox.info
             </a>
             <br/>
             взять кредит --&gt;
             <a href="http://kreditov.bxox.info">
              http://kreditov.bxox.info
             </a>
             <br/>
             кредит онлайн --&gt;
             <a href="http://creditov.bxox.info">
              http://creditov.bxox.info
             </a>
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/16595">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-17297">
      </a>
      <div about="/comment/17297#comment-17297" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
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
          <span content="2019-06-01T19:17:31+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期六, 06/01/2019 - 19:17
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/17297#comment-17297" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/17297#comment-17297" rel="bookmark">
          Order Neurontine Overnight Stevprople
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Side Effects Keflex Second Day  &lt;a href=
             <a href="http://tadalaf20mg.com&gt;buy">
              http://tadalaf20mg.com&gt;buy
             </a>
             generic cialis online&lt;/a&gt; Buy Finasteride 1mg Propecia Side Effects
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/17297">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-19611">
      </a>
      <div about="/comment/19611#comment-19611" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Ellincuse (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-02T17:21:00+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期日, 06/02/2019 - 17:21
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/19611#comment-19611" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/19611#comment-19611" rel="bookmark">
          Priligy A New York Ellnoug
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Ordering Viagra From Cananda Cheap Drugs From India Where Can I Buy Onofin Pills  &lt;a href=
             <a href="http://tadalaffbuy.com&gt;cialis">
              http://tadalaffbuy.com&gt;cialis
             </a>
             overnight shipping from usa&lt;/a&gt; Priligy Tijuana
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/19611">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-23037">
      </a>
      <div about="/comment/23037#comment-23037" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            AustAbids (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-04T04:55:05+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期二, 06/04/2019 - 04:55
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/23037#comment-23037" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/23037#comment-23037" rel="bookmark">
          Cialis Generico En Espana JeaEmbaks
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Viagra Info Amoxicillin Uses Diarrhea Wie Teuer Ist Viagra  &lt;a href=
             <a href="http://viaapill.com&gt;viagra&lt;/a&gt;">
              http://viaapill.com&gt;viagra&lt;/a&gt;
             </a>
             Real Hydrochlorothiazide Internet Overseas Amex Accepted Propecia Schweiz Preis How To Last Longer
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/23037">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-23072">
      </a>
      <div about="/comment/23072#comment-23072" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
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
          <span content="2019-06-04T05:12:47+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期二, 06/04/2019 - 05:12
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/23072#comment-23072" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/23072#comment-23072" rel="bookmark">
          Precio De Cialis En La Farmacia EllCauh
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             How To Buy Shipped Ups Generic Progesterone 200mg Website Augmentin 875 Mg Tablet Online  &lt;a href=
             <a href="http://buygenericvia.com&gt;viagra">
              http://buygenericvia.com&gt;viagra
             </a>
             online pharmacy&lt;/a&gt; Generic Prednisone Without A Script
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/23072">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-23911">
      </a>
      <div about="/comment/23911#comment-23911" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Steptwemy (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-04T13:05:33+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期二, 06/04/2019 - 13:05
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/23911#comment-23911" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/23911#comment-23911" rel="bookmark">
          Erection Remedies EllLEANCY
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Legally Doxycycline Amex Accepted Priligy Modo D'Uso Usa Direct Pharmacy  &lt;a href=
             <a href="http://curerxshop.com&gt;cialis">
              http://curerxshop.com&gt;cialis
             </a>
             5mg best price&lt;/a&gt; Levitra Viagra Cialis Test Clarithromycin Omeprazole Amoxil Cialis 5mg Tadalafil Lilly
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/23911">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-25472">
      </a>
      <div about="/comment/25472#comment-25472" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
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
          <span content="2019-06-05T02:50:51+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期三, 06/05/2019 - 02:50
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/25472#comment-25472" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/25472#comment-25472" rel="bookmark">
          Levitra Von Bayer EllCauh
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Avoir Clomid Enceinte Homoopathie Levitra Diflucan 100 Mg  &lt;a href=
             <a href="http://cialtadalaff.com&gt;cheapest">
              http://cialtadalaff.com&gt;cheapest
             </a>
             cialis 20mg&lt;/a&gt; Amoxicillin Suspension
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/25472">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-25640">
      </a>
      <div about="/comment/25640#comment-25640" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Franexpok (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-05T04:00:35+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期三, 06/05/2019 - 04:00
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/25640#comment-25640" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/25640#comment-25640" rel="bookmark">
          Viagra Y Presion Alta Matsculky
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Kamagra Jelly 100mg Toulouse Viagra Dal Canada Cheap Wellbutrin  &lt;a href=
             <a href="http://cialisab.com&gt;cialis">
              http://cialisab.com&gt;cialis
             </a>
             5 mg best price usa&lt;/a&gt; Prevacid Buy One Get One Free Rebate
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/25640">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-29088">
      </a>
      <div about="/comment/29088#comment-29088" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Matnetela (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-05T19:59:52+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期三, 06/05/2019 - 19:59
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/29088#comment-29088" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/29088#comment-29088" rel="bookmark">
          Amoxicillin Good For Prosthesis Matnetela
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Canadian Health Shop Propecia Carne  &lt;a href=
             <a href="http://cheapviapill.com&gt;viagra&lt;/a&gt;">
              http://cheapviapill.com&gt;viagra&lt;/a&gt;
             </a>
             Cialis Simili
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/29088">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-30316">
      </a>
      <div about="/comment/30316#comment-30316" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            Franexpok (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-06T02:10:42+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期四, 06/06/2019 - 02:10
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/30316#comment-30316" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/30316#comment-30316" rel="bookmark">
          Levitra 8 Compresse Matsculky
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Supreme Suppiers Keflex Equivalents  &lt;a href=
             <a href="http://ausgsm.com&gt;&lt;/a&gt;">
              http://ausgsm.com&gt;&lt;/a&gt;
             </a>
             Bupropion Recreational Use Buy Zoloft On Line
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/30316">
           回复
          </a>
         </li>
        </ul>
       </div>
       <!-- /.comment-text -->
      </div>
      <a id="comment-31098">
      </a>
      <div about="/comment/31098#comment-31098" class="comment comment-by-anonymous clearfix" typeof="sioc:Post sioct:Comment">
       <div class="attribution">
        <div class="comment-submitted">
         <p class="commenter-name">
          <span rel="sioc:has_creator">
           <span class="username" datatype="" property="foaf:name" typeof="sioc:UserAccount" xml:lang="">
            KelDees (未验证)
           </span>
          </span>
         </p>
         <p class="comment-time">
          <span content="2019-06-06T05:47:25+02:00" datatype="xsd:dateTime" property="dc:date dc:created">
           星期四, 06/06/2019 - 05:47
          </span>
         </p>
         <p class="comment-permalink">
          <a class="permalink" href="/comment/31098#comment-31098" rel="bookmark">
           永久连接
          </a>
         </p>
        </div>
       </div>
       <div class="comment-text">
        <div class="comment-arrow">
        </div>
        <h3 datatype="" property="dc:title">
         <a class="permalink" href="/comment/31098#comment-31098" rel="bookmark">
          Propecia Generique Canada KelDees
         </a>
        </h3>
        <div class="content">
         <span class="rdf-meta element-hidden" rel="sioc:reply_of" resource="/article/213">
         </span>
         <div class="field field-name-comment-body field-type-text-long field-label-hidden">
          <div class="field-items">
           <div class="field-item even" property="content:encoded">
            <p>
             Comprar Levitra Professional  &lt;a href=
             <a href="http://drugslr.com&gt;canadian">
              http://drugslr.com&gt;canadian
             </a>
             cialis&lt;/a&gt; Retin A
            </p>
           </div>
          </div>
         </div>
        </div>
        <!-- /.content -->
        <ul class="links inline">
         <li class="comment-reply first last">
          <a href="/comment/reply/213/31098">
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

