---
layout: post
title: "如何在ProtonMail中设置PGP加密 - iYouPort"
date: 2021-07-06T16:03:50+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8protonmail%e4%b8%ad%e8%ae%be%e7%bd%aepgp%e5%8a%a0%e5%af%86/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16457 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-54 category-67 tag-encryption tag-pgp tag-protonmail tag-security" id="post-16457">
 <header class="entry-header">
  <h1 class="entry-title">
   如何在ProtonMail中设置PGP加密
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
   <a href="https://www.iyouport.org/category/%e6%8a%80%e6%9c%af%e9%98%b2%e8%ba%ab-%e8%87%aa%e6%88%91%e4%bf%9d%e6%8a%a4%e6%96%b9%e6%b3%95/" rel="category tag">
    技术防身/自我保护方法
   </a>
   ,
   <a href="https://www.iyouport.org/category/%e7%bb%99%e8%a1%8c%e5%8a%a8%e8%80%85%e7%9a%84%e6%8a%a4%e8%ba%ab%e7%ac%a6%e5%92%8c%e6%ad%a6%e5%99%a8/" rel="category tag">
    给行动者的护身符和武器
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-07-07T00:03:50+08:00">
    2021年7月7日
   </time>
   <time class="updated" datetime="2021-04-08T12:51:13+08:00">
    2021年4月8日
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
       不需要任何额外的软件
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1500" data-image-id="0*TugIVZvRaNfadDBL" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*TugIVZvRaNfadDBL?is-pending-load=1" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*TugIVZvRaNfadDBL" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1500" data-image-id="0*TugIVZvRaNfadDBL" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*TugIVZvRaNfadDBL"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   任何邮箱加PGP都可以发送加密邮件。但在两个 ProtonMail 用户之间的通信是自动加密的，而您如果与非 ProtonMail 用户通信则需要手动设置。
  </p>
  <p class="graf graf--p">
   Pretty Good Privacy，简称PGP，可以让您锁定您的邮件，只有拥有密钥的目标收件人才能查看邮件。ProtonMail 是为数不多的不需要任何额外软件就能支持此功能的电子邮件服务之一。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    PGP是如何工作的？
   </strong>
  </h3>
  <p class="graf graf--p">
   PGP的工作原理是使用公钥和私钥。要发送加密邮件给某人，您需要知道此人的公钥。用收件人的公钥加密您发出的信息，然后他们就可以用他们的私钥解密。端对端加密使得任何人几乎不可能拦截您的信息 — — 前提是，您永远不要向任何人透露您的私钥。
  </p>
  <p class="graf graf--p">
   在大多数电子邮件客户端中使用PGP都需要使用额外的软件（如
   <a class="markup--anchor markup--p-anchor" data-href="https://flowcrypt.com/" href="https://flowcrypt.com/" rel="noopener" target="_blank">
    FlowCrypt
   </a>
   或
   <a class="markup--anchor markup--p-anchor" data-href="https://www.mailvelope.com/" href="https://www.mailvelope.com/" rel="noopener" target="_blank">
    Mailvelope
   </a>
   ）来处理解密和加密过程。但是 ProtonMail 已经原生支持 OpenPGP，这意味着您可以将其设置为用于特定的电子邮件地址，然后就不用管它了。
  </p>
  <p class="graf graf--p">
   您可以使用免费的 ProtonMail 账户或付费账户来使用PGP。
  </p>
  <p class="graf graf--p">
   提示：如果您已经向另一个 ProtonMail 用户发送了邮件，那么您不需要担心这个问题，因为在 ProtonMail 地址之间发送的邮件已经被端到端加密了。只有当您想和没有使用 ProtonMail 的人交换加密邮件时，才需要这样做。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    第一步：分享您的公钥
   </strong>
  </h3>
  <p class="graf graf--p">
   要通过PGP设置安全的电子邮件通信，您需要先和您要通信的人交换公钥。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="423" data-image-id="0*DMhI9rgriIsqL7BS" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*DMhI9rgriIsqL7BS?is-pending-load=1" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*DMhI9rgriIsqL7BS" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="423" data-image-id="0*DMhI9rgriIsqL7BS" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*DMhI9rgriIsqL7BS"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   如果您还没有这样做，先注册一个 ProtonMail 账户并登录。点击屏幕左上角的 “撰写” 按钮，开始撰写新邮件。输入您要为其建立加密通信的收件人的地址。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="458" data-image-id="0*PwxmAxtHtNT4hdVk" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*PwxmAxtHtNT4hdVk?is-pending-load=1" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*PwxmAxtHtNT4hdVk" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="458" data-image-id="0*PwxmAxtHtNT4hdVk" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*PwxmAxtHtNT4hdVk"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   接下来，点击 “更多” 下拉图标，确保 “附加公钥” 被选中。现在您可以在邮件正文中添加一条信息，通知收件人您的公钥已经附加。您可以在 “设置” &gt; “安全” 下，通过启用PGP设置下的 “自动附加公钥”，将您的公钥自动附加到所有发出的邮件中。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    第2步：信任您的联系人的公钥
   </strong>
  </h3>
  <p class="graf graf--p">
   接下来，您希望与您通信的人分享他们的公钥。他们如何做到这一点最终取决于他们使用PGP的方式，但不管怎样它都将以一个小文件附件的形式出现。当您收到这封邮件的时候，ProtonMail 会通知您附件中有一个公钥，并要求您信任它。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="509" data-image-id="0*QBaV6D75uRkPMTew" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*QBaV6D75uRkPMTew?is-pending-load=1" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*QBaV6D75uRkPMTew" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="509" data-image-id="0*QBaV6D75uRkPMTew" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*QBaV6D75uRkPMTew"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   点击 “信任”，并确保在弹出的窗口中勾选 “用于加密”。这样就会在发送公钥的邮件地址旁边标注这个公钥。
  </p>
  <p class="graf graf--p">
   如果收件人通过其他方式向您发送公钥，比如私密聊天等等，您可以点击页面顶部的 “联系人”，创建一个新的联系人。使用收到公钥的同一邮箱，并上传您收到的那个文件。再次确保选择 “用于加密”，这样您就可以在寄出的邮件上签名了。
  </p>
  <p class="graf graf--p">
   提示：您也可以使用 ProtonMail 的联系人功能手动上传收件人的公钥。请参阅
   <a class="markup--anchor markup--p-anchor" data-href="https://protonmail.com/support/knowledge-base/how-to-use-pgp/" href="https://protonmail.com/support/knowledge-base/how-to-use-pgp/" rel="noopener" target="_blank">
    ProtonMail 的文档
   </a>
   了解更多信息。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    现在可以安全地进行通信了
   </strong>
  </h3>
  <p class="graf graf--p">
   交换了密钥，您的通讯录也更新了正确的密钥，现在您应该可以安全地与您的联系人进行通信了。您还需要为您希望使用PGP的其他联系人重复这个过程。这个过程可能就是为什么PGP仍然是一个相对隐蔽且有效的加密工具。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="181" data-image-id="0*5LBFneMvKTviHVMZ" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*5LBFneMvKTviHVMZ?is-pending-load=1" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*5LBFneMvKTviHVMZ" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="181" data-image-id="0*5LBFneMvKTviHVMZ" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*5LBFneMvKTviHVMZ"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   如果您正确设置了PGP，ProtonMail 会自动对邮件进行加密和解密。如果您看到 “发件人” 栏中的绿色挂锁图标，您就可以知道邮件已经通过PGP加密了（其他ProtonMail用户的邮件会被紫色挂锁表示）。⚪️
  </p>
  <div id="atatags-1611829871-60e5067df2d5f">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16457" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8protonmail%e4%b8%ad%e8%ae%be%e7%bd%aepgp%e5%8a%a0%e5%af%86/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16457" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8protonmail%e4%b8%ad%e8%ae%be%e7%bd%aepgp%e5%8a%a0%e5%af%86/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16457-60e5067df331d" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16457&amp;origin=www.iyouport.org&amp;obj_id=161182987-16457-60e5067df331d" id="like-post-wrapper-161182987-16457-60e5067df331d">
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
    <a href="https://www.iyouport.org/tag/encryption/" rel="tag">
     encryption
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/pgp/" rel="tag">
     PGP
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/protonmail/" rel="tag">
     ProtonMail
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
   <time class="entry-date published" datetime="2021-07-07T00:03:50+08:00">
    2021年7月7日
   </time>
   <time class="updated" datetime="2021-04-08T12:51:13+08:00">
    2021年4月8日
   </time>
  </div>
 </div>
</article>

