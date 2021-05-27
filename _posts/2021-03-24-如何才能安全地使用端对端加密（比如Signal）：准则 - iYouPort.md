---
layout: post
title: "如何才能安全地使用端对端加密（比如Signal）：准则 - iYouPort"
date: 2021-03-24T16:01:18+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%ae%89%e5%85%a8%e5%9c%b0%e4%bd%bf%e7%94%a8-signal%ef%bc%9a%e5%87%86%e5%88%99/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-15644 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-54 category-67 tag-activism tag-e2ee tag-opsec tag-privacy tag-security tag-self-defense tag-signal tag-technique" id="post-15644">
 <header class="entry-header">
  <h1 class="entry-title">
   如何才能安全地使用端对端加密（比如Signal）：准则
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
   <time class="entry-date published" datetime="2021-03-25T00:01:18+08:00">
    2021年3月25日
   </time>
   <time class="updated" datetime="2021-03-24T14:32:46+08:00">
    2021年3月24日
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
       一个软件不能保护您的一切，最严重的问题往往都出在人身上
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="667" data-image-id="0*eGegN19fMSWYYpoh" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*eGegN19fMSWYYpoh?is-pending-load=1" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*eGegN19fMSWYYpoh" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="667" data-image-id="0*eGegN19fMSWYYpoh" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*eGegN19fMSWYYpoh"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   您
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e6%b3%84%e6%bc%8f%e6%96%87%e4%bb%b6%e6%98%be%e7%a4%ba%e9%97%b4%e8%b0%8d%e5%b7%b2%e7%bb%8f%e8%83%bd%e7%bb%95%e8%bf%87-signal-%e7%9a%84%e5%8a%a0%e5%af%86%ef%bc%8c%e9%82%a3%e4%b9%88%e7%ab%af%e5%af%b9/" href="https://www.iyouport.org/%e6%b3%84%e6%bc%8f%e6%96%87%e4%bb%b6%e6%98%be%e7%a4%ba%e9%97%b4%e8%b0%8d%e5%b7%b2%e7%bb%8f%e8%83%bd%e7%bb%95%e8%bf%87-signal-%e7%9a%84%e5%8a%a0%e5%af%86%ef%bc%8c%e9%82%a3%e4%b9%88%e7%ab%af%e5%af%b9/" rel="noopener" target="_blank">
    应该使用端对端加密
   </a>
   ，这不必细说了；幸运的是如今很多人已经理解到使用端对端加密的重要性，尤其是，
   <strong class="markup--strong markup--p-strong">
    人们已经知道，安全不是哪个软件能完全解决的问题，安全必须是一套
   </strong>
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e4%bf%9d%e6%8a%a4%e5%ae%89%e5%85%a8%e9%9c%80%e8%a6%81%e4%b8%80%e7%b3%bb%e5%88%97%e6%80%9d%e8%80%83%e6%96%b9%e5%bc%8f%ef%bc%8c%e8%80%8c%e4%b8%8d%e6%98%af%e5%93%aa%e4%b8%aa%e8%bd%af%e4%bb%b6/" href="https://www.iyouport.org/%e4%bf%9d%e6%8a%a4%e5%ae%89%e5%85%a8%e9%9c%80%e8%a6%81%e4%b8%80%e7%b3%bb%e5%88%97%e6%80%9d%e8%80%83%e6%96%b9%e5%bc%8f%ef%bc%8c%e8%80%8c%e4%b8%8d%e6%98%af%e5%93%aa%e4%b8%aa%e8%bd%af%e4%bb%b6/" rel="noopener" target="_blank">
    <strong class="markup--strong markup--p-strong">
     科学的思维习惯
    </strong>
   </a>
   <strong class="markup--strong markup--p-strong">
    ➕ 科学的
   </strong>
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/opsec-%e6%93%8d%e4%bd%9c%e5%ae%89%e5%85%a8%ef%bc%9a%e5%9c%a8%e5%8f%8d%e4%be%a6%e5%af%9f%e7%9a%84%e8%bf%87%e7%a8%8b%e4%b8%ad%e6%82%a8%e5%ba%94%e8%af%a5%e6%b3%a8%e6%84%8f%e5%93%aa%e4%ba%9b%e9%99%b7/" href="https://www.iyouport.org/opsec-%e6%93%8d%e4%bd%9c%e5%ae%89%e5%85%a8%ef%bc%9a%e5%9c%a8%e5%8f%8d%e4%be%a6%e5%af%9f%e7%9a%84%e8%bf%87%e7%a8%8b%e4%b8%ad%e6%82%a8%e5%ba%94%e8%af%a5%e6%b3%a8%e6%84%8f%e5%93%aa%e4%ba%9b%e9%99%b7/" rel="noopener" target="_blank">
    <strong class="markup--strong markup--p-strong">
     操作方法
    </strong>
   </a>
   <strong class="markup--strong markup--p-strong">
    ➕
   </strong>
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%ae%89%e5%85%a8%e6%98%af%e8%bf%bd%e6%b1%82%ef%bc%8c%e8%80%8c%e4%b8%8d%e6%98%af%e4%bb%bb%e5%8a%a1%ef%bc%9a%e6%95%b4%e4%bd%93%e5%ae%89%e5%85%a8%ef%bc%888%ef%bc%89-%e5%87%86%e5%a4%87%e5%a5%bd/" href="https://www.iyouport.org/%e5%ae%89%e5%85%a8%e6%98%af%e8%bf%bd%e6%b1%82%ef%bc%8c%e8%80%8c%e4%b8%8d%e6%98%af%e4%bb%bb%e5%8a%a1%ef%bc%9a%e6%95%b4%e4%bd%93%e5%ae%89%e5%85%a8%ef%bc%888%ef%bc%89-%e5%87%86%e5%a4%87%e5%a5%bd/" rel="noopener" target="_blank">
    <strong class="markup--strong markup--p-strong">
     有效的协作
    </strong>
   </a>
   <strong class="markup--strong markup--p-strong">
    。
   </strong>
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%f0%9f%94%90-%e5%a6%82%e4%bd%95%e5%9c%a8%e4%b8%8d%e5%bf%85%e6%9a%b4%e9%9c%b2%e7%9c%9f%e5%ae%9e%e7%94%b5%e8%af%9d%e5%8f%b7%e7%a0%81%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e4%bd%bf%e7%94%a8-signal/" href="https://www.iyouport.org/%f0%9f%94%90-%e5%a6%82%e4%bd%95%e5%9c%a8%e4%b8%8d%e5%bf%85%e6%9a%b4%e9%9c%b2%e7%9c%9f%e5%ae%9e%e7%94%b5%e8%af%9d%e5%8f%b7%e7%a0%81%e7%9a%84%e6%83%85%e5%86%b5%e4%b8%8b%e4%bd%bf%e7%94%a8-signal/" rel="noopener" target="_blank">
    Signal
   </a>
   也一样。作为一个安全工具，如今它是许多群体相互联系和沟通的首选渠道。用户团体的意图和目的可以有很大的不同，从制定晚餐计划到组织下一次反抗运动。
  </p>
  <p class="graf graf--p">
   但是，仅仅使用 Signal 还不足以保证您和您的朋友的安全 ——
   <strong class="markup--strong markup--p-strong">
    安全只有在堵住最薄弱环节之后才能有保障，在通讯软件上，“最薄弱环节” 就是：您与之交流的所有人中最不注重安全性的那个/那些人
   </strong>
   。
  </p>
  <p class="graf graf--p">
   因此本文将概述一些准则和协议，以帮助加强您的个人和集体安全实践。
  </p>
  <p>
   <strong>
    请注意：端对端加密工具不只有Signal！本文中强调的大部分准则适用于所有端对端加密通信应用
   </strong>
   。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     当创建一个新群组时
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   加密通信的技术能力本身会给人们一种误解，似乎 “我终于可以随便说话了”，并不是这样的！还记得英国间谍搞出来的入侵 Signal 的方法吗？是的，最危险的部分在于人，在这里看到《
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/%e5%85%b3%e4%ba%8e%e5%b9%bd%e7%81%b5%e7%94%a8%e6%88%b7%e5%92%8c%e5%bc%80%e8%a3%86%e8%a3%a4/" href="https://www.iyouport.org/%e5%85%b3%e4%ba%8e%e5%b9%bd%e7%81%b5%e7%94%a8%e6%88%b7%e5%92%8c%e5%bc%80%e8%a3%86%e8%a3%a4/" rel="noopener" target="_blank">
    关于幽灵用户和开裆裤
   </a>
   》。
  </p>
  <p class="graf graf--p">
   创建群组要有目的性，添加成员同样需要有目的性。在将任何一个人添加到您的联系人列表之前要知道：一旦某人成为群组的一部分，您就不可能简单地将其删除了。您不可能在完全放弃这个群组或者要求此人离开之前删除他。
  </p>
  <p class="graf graf--p">
   📌 您随时应该知道您加进来的人都是谁。
  </p>
  <p class="graf graf--p">
   考虑一下您会怎么处理一个一开始就被单方面添加进来的人，
   <strong class="markup--strong markup--p-strong">
    单方面添加
   </strong>
   指的是比如无法双向认证的，或者是让群组中其他人对此有顾虑的。另外，在没有事先征得群组中其他人同意的情况下，
   <strong class="markup--strong markup--p-strong">
    不要
   </strong>
   把新人加到敏感的群组里。
  </p>
  <p class="graf graf--p">
   群组建立后，您需要说明此群组的目的，并立即点名 —— 可以完全根据您的需求，不论是不是实名，或者所有成员都使用代号，只要彼此知道其他成员都是谁就可以了。这些应该
   <strong class="markup--strong markup--p-strong">
    在对话开始之前完成
   </strong>
   。
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    不要
   </strong>
   在没有问过群组成员的情况下添加新的人进入，并给人们一个指定的时间来表达意见，比如24小时，因为许多人不可能每时每刻都在手机上活动。
   <strong class="markup--strong markup--p-strong">
    鼓励原成员对新成员提出问题或进行阐述
   </strong>
   ，这比简单地说 “您担保” 更有助于创造良好的对话。
  </p>
  <p class="graf graf--p">
   每次增加新成员时，都要重新点名，这样您的群组其他成员就会知道自己正在和谁说话。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     担保
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   这里的的担保就是它本来的意思 —— 即 支持是真实的、确定的、可靠的，或 证明、保证、认证。
   <strong class="markup--strong markup--p-strong">
    在政治背景下，为某人担保指的是，您相信此人致力于团队的目标，值得信赖，可靠和负责任
   </strong>
   。
  </p>
  <p class="graf graf--p">
   📌 请记住，担保是对您个人意见的反映，建议谨慎使用担保，因为如果是不负责任的担保，就会影响群体的安全、信任和凝聚力。
  </p>
  <p class="graf graf--p">
   担保是某人获得一种凭证，
   <strong class="markup--strong markup--p-strong">
    这样的 “凭证” 对于以前可能没有合作经验的群体来说非常重要，他们需要一定的信任和安全感才能舒适有效地合作
   </strong>
   。
  </p>
  <p class="graf graf--p">
   担保制度可以让1个人或多个人（越多越好）使用他们从团体中获得的信任，并将其扩展到他们想要带入的人身上。担保的必要性根据您工作的内容而异，越是敏感的工作，这个过程就越是需要谨慎。
  </p>
  <p class="graf graf--p">
   担保某人是否应该能够进入一个群组的对话、是否合乎该群组的目标和目的，应该
   <strong class="markup--strong markup--p-strong">
    结合群组的整体目标和风险来考虑
   </strong>
   。群里的其他成员在选择是否相信您提供的担保时，都会有自己的判断力。
  </p>
  <p class="graf graf--p">
   📌 使用担保的一些标准包括：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    认识此人有一段时间了，对此人有一定程度上的了解；尤其是，了解此人在该群组的目标方面的契合度；
   </li>
   <li class="graf graf--li">
    您与此人合作过一段时间，对此人的工作方式、品格和原则立场有一定了解；
   </li>
   <li class="graf graf--li">
    您的熟人中有一些人在一定时间内与此人合作过，他们对此人的信任加之您对他们的信任，可以在您的心目中给此人一个信任度的基础分数；
   </li>
   <li class="graf graf--li">
    您了解此人的优势和缺点，以及知道此人在面临镇压的情况下的反应；
   </li>
   <li class="graf graf--li">
    您知道此人如何回应批评或反馈，以及此人对自己的行为负责的程度；
   </li>
   <li class="graf graf--li">
    您了解此人的大家庭、儿时的朋友、以及整个人生故事（开个玩笑…也许是，但比较少见…）
   </li>
  </ul>
  <p class="graf graf--p">
   总之，
   <strong class="markup--strong markup--p-strong">
    您应为以下人员提供担保：您认识和信任的人，您知道他们了解特定群体的目标和安全要求，您知道他们参加过专业的扎实的安全培训，并可以熟练使用安全操作。
   </strong>
  </p>
  <p class="graf graf--p">
   您
   <strong class="markup--strong markup--p-strong">
    不应该
   </strong>
   仅仅因为 “知道这个人的存在和其工作内容” 或 “有过一两次愉快的谈话” 就给予此人担保，虽然这些东西是了解和信任某人的一部分，但它仅仅是一部分！并非全部。
  </p>
  <p class="graf graf--p">
   担保的严格程度会根据你们的对话的敏感度和团体承担的风险等级而有所不同。如果这是你没有考虑过的问题，现在就需要考虑（我们在不久后会更详细介绍
   <strong class="markup--strong markup--p-strong">
    安全文化的构建
   </strong>
   ）。
  </p>
  <p class="graf graf--p">
   📌 无论您用什么标准来担保他人，都要提前跟群组里的每个人沟通，而且每个人都需要站在同一条线上。担保这个词已经被用烂了，几乎没有详细地说明，人们对它的含义往往有不同的想法。这就是您需要沟通的地方，让所有人
   <strong class="markup--strong markup--p-strong">
    统一对这个概念的理解标准
   </strong>
   。
  </p>
  <p class="graf graf--p">
   请注意，
   <strong class="markup--strong markup--p-strong">
    数字安全不能代替关系安全！
   </strong>
   如果您决定信任的任何一个人在敏感的信息对话中，结果此人本来是恶意的、鲁莽的、粗心的、或不负责任的，那么世界上所有安全软件和安全协议都无法帮助您。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <b>
     规则
    </b>
   </span>
  </h3>
  <p class="graf graf--p">
   当重新安装 Signal 或获得新的电话号码时，
   <strong class="markup--strong markup--p-strong">
    请事先通知各群组
   </strong>
   ，让他们知道要接受新的安全密钥 —— 他们会看到您的 “安全码已改变” 的提示，如果他们不知道您在做什么，他们会因此害怕。
  </p>
  <p class="graf graf--p">
   或者，如果您无法事先通知其他人，也要
   <strong class="markup--strong markup--p-strong">
    在事后立即让他们知道
   </strong>
   。📌 根据安全级别不同，您应该选择亲自见面、或发送安全号码的截图，来验证新的安全码。
  </p>
  <p class="graf graf--p">
   使用安卓系统时，一定要在 Signal 应用上设置密码和超时功能。可惜iOS还没有这个安全功能。至少要为整个手机设置一个复杂的字母数字密码。从法律的角度来看，形状、图案和拇指指纹/生物识别技术
   <strong class="markup--strong markup--p-strong">
    都是不安全的
   </strong>
   ，维稳官员可以依法强制您出示指纹来解锁手机。此外也要对您的手机进行加密。
  </p>
  <p class="graf graf--p">
   一定要使用阅后即焚。时间设置长短根据您的具体危险状况来判断，
   <strong class="markup--strong markup--p-strong">
    您需要想象威胁会如何发生，据此来判断多长时间的销毁是合适的
   </strong>
   。如果您的群组中任何一个人的手机被警察抢走，却没来得及锁屏，你们所有人都会被暴露。
  </p>
  <p class="graf graf--p">
   并且，您需要时刻关注阅后即焚时间的稳定性，有时，当群组中有人重新安装应用程序或添加了新的人员进入时，阅后即焚可能会被自动关闭。您需要确保及时地重新激活该功能。
  </p>
  <p class="graf graf--p">
   📌 如果您正在参加反抗行动、或处于可能导致逮捕的任何一种情况下，包括过境，而您又带着手机，
   <strong class="markup--strong markup--p-strong">
    请事先离开所有的群组并卸载 Signal
   </strong>
   。不论如何，非常建议
   <strong class="markup--strong markup--p-strong">
    不要
   </strong>
   把您的个人手机带入上述这些情况中。您可以在下面阅读详细解释，以及您可以如何处理这种情况：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%8c%87%e5%8d%97%ef%bc%9a%e5%bd%93%e6%82%a8%e5%87%86%e5%a4%87%e5%8f%82%e5%8a%a0%e6%8a%97%e8%ae%ae%e6%b4%bb%e5%8a%a8/" href="https://www.iyouport.org/%e6%8c%87%e5%8d%97%ef%bc%9a%e5%bd%93%e6%82%a8%e5%87%86%e5%a4%87%e5%8f%82%e5%8a%a0%e6%8a%97%e8%ae%ae%e6%b4%bb%e5%8a%a8/" rel="noopener" target="_blank">
     指南：当您准备参加抗议活动…
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e4%b9%b0%e4%b8%8d%e8%b5%b7-%e4%b9%b0%e4%b8%8d%e5%88%b0%e4%b8%80%e6%ac%a1%e6%80%a7%e6%89%8b%e6%9c%ba%e6%80%8e%e4%b9%88%e5%8a%9e%ef%bc%9f%e8%bf%99%e9%87%8c%e6%98%af%e6%82%a8%e5%9c%a8%e5%8f%82%e5%8a%a0/" href="https://www.iyouport.org/%e4%b9%b0%e4%b8%8d%e8%b5%b7-%e4%b9%b0%e4%b8%8d%e5%88%b0%e4%b8%80%e6%ac%a1%e6%80%a7%e6%89%8b%e6%9c%ba%e6%80%8e%e4%b9%88%e5%8a%9e%ef%bc%9f%e8%bf%99%e9%87%8c%e6%98%af%e6%82%a8%e5%9c%a8%e5%8f%82%e5%8a%a0/" rel="noopener" target="_blank">
     买不起/买不到一次性手机怎么办？这里是您在参加敏感行动之前需要了解的事
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%af%86%e5%88%ab%e6%8a%97%e8%ae%ae%e6%b4%bb%e5%8a%a8%e4%b8%ad%e5%8f%af%e8%a7%81%e7%9a%84%e5%92%8c%e4%b8%8d%e5%8f%af%e8%a7%81%e7%9a%84%e7%9b%91%e8%a7%86/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e8%af%86%e5%88%ab%e6%8a%97%e8%ae%ae%e6%b4%bb%e5%8a%a8%e4%b8%ad%e5%8f%af%e8%a7%81%e7%9a%84%e5%92%8c%e4%b8%8d%e5%8f%af%e8%a7%81%e7%9a%84%e7%9b%91%e8%a7%86/" rel="noopener" target="_blank">
     如何识别抗议活动中可见的和不可见的监视
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%89%8b%e6%9c%ba%e5%ba%94%e8%af%a5%e6%9c%89%e4%b8%94%e5%8f%aa%e6%9c%89%e4%b8%80%e4%b8%aa%e7%94%a8%e9%80%94%ef%bc%9a%e5%9c%a8%e6%95%8c%e5%af%b9%e7%8e%af%e5%a2%83%e4%b8%ad%e4%bf%9d%e6%8a%a4%e8%87%aa/" href="https://www.iyouport.org/%e6%89%8b%e6%9c%ba%e5%ba%94%e8%af%a5%e6%9c%89%e4%b8%94%e5%8f%aa%e6%9c%89%e4%b8%80%e4%b8%aa%e7%94%a8%e9%80%94%ef%bc%9a%e5%9c%a8%e6%95%8c%e5%af%b9%e7%8e%af%e5%a2%83%e4%b8%ad%e4%bf%9d%e6%8a%a4%e8%87%aa/" rel="noopener" target="_blank">
     手机应该有且只有一个用途：在敌对环境中保护自己（3）
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e8%ad%a6%e5%af%9f%e5%a6%82%e4%bd%95%e5%88%a9%e7%94%a8%e6%8a%97%e8%ae%ae%e8%80%85%e7%9a%84%e6%89%8b%e6%9c%ba%e8%bf%bd%e8%b8%aa%e6%af%8f%e4%b8%aa%e4%ba%ba/" href="https://www.iyouport.org/%e8%ad%a6%e5%af%9f%e5%a6%82%e4%bd%95%e5%88%a9%e7%94%a8%e6%8a%97%e8%ae%ae%e8%80%85%e7%9a%84%e6%89%8b%e6%9c%ba%e8%bf%bd%e8%b8%aa%e6%af%8f%e4%b8%aa%e4%ba%ba/" rel="noopener" target="_blank">
     警察如何利用抗议者的手机追踪每个人
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e8%ad%a6%e5%af%9f%e6%9f%a5%e6%89%8b%e6%9c%ba%e7%9a%84%e4%b8%9c%e8%a5%bf%e9%95%bf%e4%bb%80%e4%b9%88%e6%a0%b7%ef%bc%9f-%e4%bb%8e%e6%8a%80%e6%9c%af%e8%a7%92%e5%ba%a6%e7%9c%8b%e7%a7%bb/" href="https://www.iyouport.org/%e8%ad%a6%e5%af%9f%e6%9f%a5%e6%89%8b%e6%9c%ba%e7%9a%84%e4%b8%9c%e8%a5%bf%e9%95%bf%e4%bb%80%e4%b9%88%e6%a0%b7%ef%bc%9f-%e4%bb%8e%e6%8a%80%e6%9c%af%e8%a7%92%e5%ba%a6%e7%9c%8b%e7%a7%bb/" rel="noopener" target="_blank">
     警察查手机的东西长什么样？ — — 从技术角度看移动设备取证
    </a>
    》
   </li>
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%89%8b%e6%9c%ba%e4%b8%ad%e9%9a%90%e8%97%8f%e7%9a%84%e8%b7%9f%e8%b8%aa%e5%99%a8%ef%bc%9a%e4%bb%96%e4%bb%ac%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8%e6%82%a8%e6%89%8b%e6%9c%ba%e7%9a%84%e5%ba%94%e7%94%a8/" href="https://www.iyouport.org/%e6%89%8b%e6%9c%ba%e4%b8%ad%e9%9a%90%e8%97%8f%e7%9a%84%e8%b7%9f%e8%b8%aa%e5%99%a8%ef%bc%9a%e4%bb%96%e4%bb%ac%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8%e6%82%a8%e6%89%8b%e6%9c%ba%e7%9a%84%e5%ba%94%e7%94%a8/" rel="noopener" target="_blank">
     手机中隐藏的跟踪器：他们如何使用您手机的应用程序监视您
    </a>
    》
   </li>
  </ul>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    如果您在跨越国界，必须首先离开所有群组，并卸载 Signal
   </strong>
   。因为通常保护您免受搜查和扣押的法律基本都不适用于国际边境。如果您在国外旅行，强烈建议
   <strong class="markup--strong markup--p-strong">
    不要携带您自己的
   </strong>
   手机/平板电脑/笔记本电脑/等。
  </p>
  <p class="graf graf--p">
   如果出现安全漏洞，比如您带着手机被警察抓到，或者
   <a class="markup--anchor markup--p-anchor" data-href="https://www.iyouport.org/covid-19%e5%90%b9%e5%93%a8%e4%ba%ba%e7%9a%84%e5%ae%b6%e9%81%ad%e9%81%87%e6%ad%a6%e8%a3%85%e7%aa%81%e8%a2%ad%e7%9a%84%e6%83%8a%e4%ba%ba%e6%a1%88%e4%be%8b%e8%af%b4%e6%98%8e%e4%ba%86%e4%bb%80%e4%b9%88/" href="https://www.iyouport.org/covid-19%e5%90%b9%e5%93%a8%e4%ba%ba%e7%9a%84%e5%ae%b6%e9%81%ad%e9%81%87%e6%ad%a6%e8%a3%85%e7%aa%81%e8%a2%ad%e7%9a%84%e6%83%8a%e4%ba%ba%e6%a1%88%e4%be%8b%e8%af%b4%e6%98%8e%e4%ba%86%e4%bb%80%e4%b9%88/" rel="noopener" target="_blank">
    您的家被警察突袭
   </a>
   ，您需要指定一个人开始一个新的群组，并立即离开旧的群组（也就是烧掉这个群组）。确保威胁不会转移到新的循环中。指定一个人留在旧群组上，确保所有人都完全离开了。最后删除这个群组。
  </p>
  <p class="graf graf--p">
   在手机丢失/被盗或被警察没收的情况下，立即向与您在同一个群组中的其他人报告，让他们提醒所有成员需要抛弃旧群组并重新开始。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     签入政策
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   有些群组是短暂的，是为了特定的短期目的而存在的，在目的完成后应予以删除。
   <strong class="markup--strong markup--p-strong">
    生命期不确定的群组应定期检查成员情况
   </strong>
   ，以帮助消除松散的问题。
  </p>
  <p class="graf graf--p">
   考虑建立签到/参与小组讨论的制度。要求群组成员定期重新判断自己在邮件列表或名单上的兴趣，并确保没有出现安全问题。📌 有些群组也可以选择对成员实行
   <strong class="markup--strong markup--p-strong">
    定期签到
   </strong>
   的要求 ——
   <strong class="markup--strong markup--p-strong">
    如果在某段指定时间内没有收到某人的签到，可能表明存在安全漏洞。这在那些经常出现强迫失踪的国家来说，是很有必要的，如果您的群组成员被失踪，您需要做最坏的考虑，尤其是需要及时知道这件事。
   </strong>
  </p>
  <p class="graf graf--p">
   📌 请记住。有时即使一个成员离开了群组，他们也会继续收到该群组的消息（由于软件故障）。
   <strong class="markup--strong markup--p-strong">
    如果该群组的信息是敏感的，某人离开此群组应被视为安全漏洞，该群组应立刻被烧毁。重建
   </strong>
   。
  </p>
  <p class="graf graf--p">
   讨论敏感资料 —— 不论是过去的、现在的或将来的 —— 应该只在所有成员 *需要知道* 的基础上进行，而不是 “我相信你” 或 “我觉得这个很酷”。吹嘘、八卦和传言都是危险的行为，在您的行动中应该没有地位。
  </p>
  <p class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    尤其是！具体的行动规划讨论应该面对面地进行 —— 决不要以数字方式进行！
   </strong>
   所有的数字安全都有弱点和漏洞。您越了解数字安全的弱点和局限性，您就越能保护自己。⚪️
  </p>
  <div id="atatags-1611829871-60afa12839290">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-15644" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%ae%89%e5%85%a8%e5%9c%b0%e4%bd%bf%e7%94%a8-signal%ef%bc%9a%e5%87%86%e5%88%99/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-15644" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%ae%89%e5%85%a8%e5%9c%b0%e4%bd%bf%e7%94%a8-signal%ef%bc%9a%e5%87%86%e5%88%99/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-15644-60afa12839a3c" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=15644&amp;origin=www.iyouport.org&amp;obj_id=161182987-15644-60afa12839a3c" id="like-post-wrapper-161182987-15644-60afa12839a3c">
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
    <a href="https://www.iyouport.org/tag/e2ee/" rel="tag">
     E2EE
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/opsec/" rel="tag">
     OPSEC
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/privacy/" rel="tag">
     privacy
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
    <a href="https://www.iyouport.org/tag/signal/" rel="tag">
     signal
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/technique/" rel="tag">
     technique
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-03-25T00:01:18+08:00">
    2021年3月25日
   </time>
   <time class="updated" datetime="2021-03-24T14:32:46+08:00">
    2021年3月24日
   </time>
  </div>
 </div>
</article>

