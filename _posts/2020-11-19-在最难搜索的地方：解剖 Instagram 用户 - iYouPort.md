---
layout: post
title: "在最难搜索的地方：解剖 Instagram 用户 - iYouPort"
date: 2020-11-19T16:03:11+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%9c%a8%e6%9c%80%e9%9a%be%e6%90%9c%e7%b4%a2%e7%9a%84%e5%9c%b0%e6%96%b9%ef%bc%9a%e8%a7%a3%e5%89%96-instagram-%e7%94%a8%e6%88%b7/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-15171 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-osint tag-instagram tag-investigations tag-osint tag-technique tag-tools" id="post-15171">
 <header class="entry-header">
  <h1 class="entry-title">
   在最难搜索的地方：解剖 Instagram 用户
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
   <a href="https://www.iyouport.org/category/osint/" rel="category tag">
    OSINT
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2020-11-20T00:03:11+08:00">
    2020年11月20日
   </time>
   <time class="updated" datetime="2020-11-20T00:03:04+08:00">
    2020年11月20日
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
       提供一些工具以协助您的调查工作
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <p>
  </p>
  <p>
   <img alt="" class="aligncenter size-full wp-image-15173 jetpack-lazy-image" data-lazy-sizes="(max-width: 1055px) 100vw, 1055px" data-lazy-src="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=1055%2C699&amp;is-pending-load=1#038;ssl=1" data-lazy-srcset="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?w=1055&amp;ssl=1 1055w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=300%2C199&amp;ssl=1 300w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=1024%2C678&amp;ssl=1 1024w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=768%2C509&amp;ssl=1 768w" data-recalc-dims="1" height="699" src="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=1055%2C699&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1055"/>
   <noscript>
    <img alt="" class="aligncenter size-full wp-image-15173" data-recalc-dims="1" height="699" sizes="(max-width: 1055px) 100vw, 1055px" src="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=1055%2C699&amp;ssl=1" srcset="https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?w=1055&amp;ssl=1 1055w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=300%2C199&amp;ssl=1 300w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=1024%2C678&amp;ssl=1 1024w, https://i0.wp.com/www.iyouport.org/wp-content/uploads/2020/10/photo-1569783899817-a49d2d25287c.jpeg?resize=768%2C509&amp;ssl=1 768w" width="1055"/>
   </noscript>
  </p>
  <p class="graf graf--p">
   Instagram 难以搜索的特点给开源情报调查设置了很多障碍。
   <a class="markup--anchor markup--p-anchor" data-href="https://osintcurio.us/2019/10/01/searching-instagram-part-2/" href="https://osintcurio.us/2019/10/01/searching-instagram-part-2/" rel="noopener noreferrer" target="_blank">
    osintcurio
   </a>
   介绍了一些方法和工具，以帮助调查人员获得更多信息。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    在开始之前
   </strong>
  </h3>
  <p class="graf graf--p">
   虽然没有必要为了在 Instagram 上做调查而注册有一个 Instagram 账户，方法在下面；但无论何时您想关注某些标签或个人资料时，有账户会更容易。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e6%97%a0%e9%9c%80%e5%b8%90%e6%88%b7%e5%8d%b3%e5%8f%af%e5%8c%bf%e5%90%8d%e6%9f%a5%e7%9c%8binstagram%e5%b8%96%e5%ad%90/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e6%97%a0%e9%9c%80%e5%b8%90%e6%88%b7%e5%8d%b3%e5%8f%af%e5%8c%bf%e5%90%8d%e6%9f%a5%e7%9c%8binstagram%e5%b8%96%e5%ad%90/" rel="noopener noreferrer" target="_blank">
     如何无需帐户即可匿名查看Instagram帖子
    </a>
    》
   </li>
   <li class="graf graf--li">
    做一个匿名账户专用于调查，
    <a class="markup--anchor markup--li-anchor" data-href="http://某些行动者，你需要一个袜子木偶" href="http://某些行动者%EF%BC%8C你需要一个袜子木偶" rel="noopener noreferrer" target="_blank">
     见这里
    </a>
   </li>
  </ul>
  <p class="graf graf--p">
   可以通过手机应用创建账户，也可以使用网站创建。对于下面即将展示的大部分内容，您都不需要登录账户。如果哪个方面您需要登录，本文会在截图的左上方显示蓝色的 “登录” 小按钮。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜索栏
   </strong>
  </h3>
  <p class="graf graf--p">
   只要随便访问任何一个 Instagram 个人资料，就能在上面找到搜索栏。您不需要为此而登录。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="139" data-image-id="0*DLljAgJRhTob9i4o" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*DLljAgJRhTob9i4o?is-pending-load=1" data-width="720" height="139" src="https://cdn-images-1.medium.com/max/1067/0*DLljAgJRhTob9i4o" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="139" data-image-id="0*DLljAgJRhTob9i4o" data-width="720" height="139" src="https://cdn-images-1.medium.com/max/1067/0*DLljAgJRhTob9i4o" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      instagram.com/search
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜人
   </strong>
  </h3>
  <p class="graf graf--p">
   在 Instagram 上搜人可能并不像看起来那么有效率。而谷歌、或任何其他搜索引擎都比它效率更高。以扎克伯格为例，使用 Google Dorks，这样 ‘site:Instagram.com “mark zuckerberg”。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="150" data-image-id="0*XN5HOvD0JI0EzSKl" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*XN5HOvD0JI0EzSKl?is-pending-load=1" data-width="720" height="150" src="https://cdn-images-1.medium.com/max/1067/0*XN5HOvD0JI0EzSKl" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="150" data-image-id="0*XN5HOvD0JI0EzSKl" data-width="720" height="150" src="https://cdn-images-1.medium.com/max/1067/0*XN5HOvD0JI0EzSKl" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      左：Instagram中的搜索结果；右：谷歌中的搜索结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   还有很多网站为您提供了在 Instagram 上搜索内容的可能性。
   <a class="markup--anchor markup--p-anchor" data-href="http://picdeer.com/" href="http://picdeer.com/" rel="noopener noreferrer" target="_blank">
    Picdeer.com
   </a>
   就是众多为您提供搜索用户选项的网站之一。
  </p>
  <p class="graf graf--p">
   这可以使您的操作更容易一些，因为标签和用户不会像 Instagram.com 那样在搜索结果中被混在一起。现在您会看到左手边的标签列表和右手边的用户。
  </p>
  <p class="graf graf--p">
   同样，还有更多这样的网站；
   <a class="markup--anchor markup--p-anchor" data-href="https://pictame.com/" href="https://pictame.com/" rel="noopener noreferrer" target="_blank">
    pictame.com
   </a>
   、
   <a class="markup--anchor markup--p-anchor" data-href="https://sometag.com/" href="https://sometag.com/" rel="noopener noreferrer" target="_blank">
    sometag.com
   </a>
   都是。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="235" data-image-id="0*1Rgwu1iX3rIdJaKm" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*1Rgwu1iX3rIdJaKm?is-pending-load=1" data-width="720" height="235" src="https://cdn-images-1.medium.com/max/1067/0*1Rgwu1iX3rIdJaKm" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="235" data-image-id="0*1Rgwu1iX3rIdJaKm" data-width="720" height="235" src="https://cdn-images-1.medium.com/max/1067/0*1Rgwu1iX3rIdJaKm" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      在Picdeer.com上的搜索结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   如果您正在寻找某种类型的用户，比方说属于某个团体或信奉某种宗教的人，那么搜索目标人的简历中的关键词可能会很有趣。
   <a class="markup--anchor markup--p-anchor" data-href="https://searchmy.bio/" href="https://searchmy.bio/" rel="noopener noreferrer" target="_blank">
    Searchmy.bio
   </a>
   就能帮您做到这一点。
  </p>
  <p class="graf graf--p">
   您可以根据 ‘最多关注者’ 或 ‘最相关的人’ 进行排序，选择结果中关注者的最低或最高数量，也选择包含主题标签。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="251" data-image-id="0*B5lbyHAOufmVcfiW" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*B5lbyHAOufmVcfiW?is-pending-load=1" data-width="720" height="251" src="https://cdn-images-1.medium.com/max/1067/0*B5lbyHAOufmVcfiW" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="251" data-image-id="0*B5lbyHAOufmVcfiW" data-width="720" height="251" src="https://cdn-images-1.medium.com/max/1067/0*B5lbyHAOufmVcfiW" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Searchmy.bio
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   当您找到了您感兴趣的个人资料时，就可以开始使用一些有用的附加组件了。
  </p>
  <p class="graf graf--p">
   从 “
   <a class="markup--anchor markup--p-anchor" data-href="https://chrome.google.com/webstore/detail/helper-tools-for-instagra/hcdbfckhdcpepllecbkaaojfgipnpbpb" href="https://chrome.google.com/webstore/detail/helper-tools-for-instagra/hcdbfckhdcpepllecbkaaojfgipnpbpb" rel="noopener noreferrer" target="_blank">
    Helpertools for Instagram
   </a>
   ”开始，这是一个谷歌浏览器插件。
  </p>
  <p class="graf graf--p">
   在下面的例子中使用的是马克·扎克伯格的个人资料，
   <a class="markup--anchor markup--p-anchor" data-href="http://twitter.com/zuck" href="https://twitter.com/zuck" rel="noopener noreferrer" target="_blank" title="Twitter profile for @zuck">
    @zuck
   </a>
   。‘Helptools for Instagram’ 是一个部分免费的插件。有几个选项真的很不错，您可以将两个个人资料相比较。
  </p>
  <p class="graf graf--p">
   根据关注/追随者的数量不同，有时可能需要一段时间。这是因为 Helpertools 设置了“暂停”，以防止 Instagram 检测到该工具。
  </p>
  <p class="graf graf--p">
   这里有一个小选项值得关注，可能一开始不会引起您的注意；“商业账户”。
  </p>
  <p class="graf graf--p">
   在扎克伯格的案例中，它被标记为 “false”，这意味着他不是商业账户。
  </p>
  <p class="graf graf--p">
   拥有一个 ‘商业账户’ 和 ‘已验证’ 账户是不同的。把您的个人资料改成 ‘商业’ 是您自己就可以更改的设置。Instagram 不会验证任何信息。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="422" data-image-id="0*LPX8jj8xXWMHT_QY" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*LPX8jj8xXWMHT_QY?is-pending-load=1" data-width="720" height="422" src="https://cdn-images-1.medium.com/max/1067/0*LPX8jj8xXWMHT_QY" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="422" data-image-id="0*LPX8jj8xXWMHT_QY" data-width="720" height="422" src="https://cdn-images-1.medium.com/max/1067/0*LPX8jj8xXWMHT_QY" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      ‘Helpertools for Instagram’ 的结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   扎克伯格的账户不是商业账户。所以来看另一个是商业账户的例子：荷兰当地一家奶酪店的账户；看它的简介；您能看到任何联系方式吗？没有!
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="316" data-image-id="0*-sXqjVtajKJfRTF1" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*-sXqjVtajKJfRTF1?is-pending-load=1" data-width="720" height="316" src="https://cdn-images-1.medium.com/max/1067/0*-sXqjVtajKJfRTF1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="316" data-image-id="0*-sXqjVtajKJfRTF1" data-width="720" height="316" src="https://cdn-images-1.medium.com/max/1067/0*-sXqjVtajKJfRTF1" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      没有显示联系方式
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   检查一下 Helpertools，看看它是否是商业帐户…
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="112" data-image-id="0*djL-fGM3HeTGAQr7" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*djL-fGM3HeTGAQr7?is-pending-load=1" data-width="362" src="https://cdn-images-1.medium.com/max/1067/0*djL-fGM3HeTGAQr7" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="112" data-image-id="0*djL-fGM3HeTGAQr7" data-width="362" src="https://cdn-images-1.medium.com/max/1067/0*djL-fGM3HeTGAQr7"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   是的，它是商业账户。
  </p>
  <p class="graf graf--p">
   甚至可以看到他们把自己的资料放在哪个类别中。而且还有更多!
  </p>
  <p class="graf graf--p">
   要查看更多信息，您现在需要创建一个档案或登录到您的档案。在手机上（或良好的模拟器上）登陆互联网。
  </p>
  <p class="graf graf--p">
   这里使用的是安卓应用。
  </p>
  <p class="graf graf--p">
   访问该奶酪店的简介，您现在会看到个人资料下面的一些按钮。其中一个是 “联系”。如果点击 “联系”，会出现一个弹出式窗口，并向您展示与简介相关的任何联系信息（由店主填写）。所以，现在我们看到了一个以前看不到的电子邮件地址。
  </p>
  <p class="graf graf--p">
   并且还有另一个 “呼叫” 按钮（Bellen），它将为您显示电话号码。
  </p>
  <p class="graf graf--p">
   请记得，仅通过网站查看个人资料时，您会错过此信息。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="382" data-image-id="0*BE2JJbpNBa0Pqsft" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*BE2JJbpNBa0Pqsft?is-pending-load=1" data-width="720" height="382" src="https://cdn-images-1.medium.com/max/1067/0*BE2JJbpNBa0Pqsft" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="382" data-image-id="0*BE2JJbpNBa0Pqsft" data-width="720" height="382" src="https://cdn-images-1.medium.com/max/1067/0*BE2JJbpNBa0Pqsft" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      1、移动应用程序登入；2、选‘Contact’ ；3、查看电话号码，或电子邮件地址
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   如果您想对一个个人资料进行分析，statflux.com 也许能帮到您。它将向您展示一些细节，您能够找到的个人资料，但它也会给您在一些其他细节上的洞见，如最多点赞和最多评论等。
  </p>
  <p class="graf graf--p">
   在查看包含大量帖子的个人资料时，您会不知道哪个帖子可能对您来说很有趣，Statflux.com 可以为您提供帮助。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="301" data-image-id="0*bEjJ4JG6Q5dHhEAv" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*bEjJ4JG6Q5dHhEAv?is-pending-load=1" data-width="720" height="301" src="https://cdn-images-1.medium.com/max/1067/0*bEjJ4JG6Q5dHhEAv" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="301" data-image-id="0*bEjJ4JG6Q5dHhEAv" data-width="720" height="301" src="https://cdn-images-1.medium.com/max/1067/0*bEjJ4JG6Q5dHhEAv" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      在Statflux.com 上以扎克伯格为例
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    放大个人资料图片并下载帐户照片
   </strong>
  </h3>
  <p class="graf graf--p">
   Instagram 有一个被裁剪的个人资料照片（圆形）。但有时您想拥有完整的照片，因为这将提供关于照片后面发生的事或可能还有谁在照片中的更多细节。
  </p>
  <p class="graf graf--p">
   插件 “
   <a class="markup--anchor markup--p-anchor" data-href="https://chrome.google.com/webstore/detail/downalbum/cgjnhhjpfcdhbhlcmmjppicjmgfkppok?hl=en" href="https://chrome.google.com/webstore/detail/downalbum/cgjnhhjpfcdhbhlcmmjppicjmgfkppok?hl=en" rel="noopener noreferrer" target="_blank">
    DownAlbum
   </a>
   ” 可以帮您做到这一点。它不仅可以帮助您在 Instagram 上使用，
   <strong class="markup--strong markup--p-strong">
    还可以在 Facebook、Pinterest、Twitter、Ask.fm 和中国的微博上使用。
   </strong>
   DownAlbum 可以帮助您轻松地放大个人资料图片。
  </p>
  <p class="graf graf--p">
   安装后，在资料图片下方会出现一个按钮 “下载照片”。点击链接后会打开一个新的页面，显示出更大的个人资料图片，您可以用它来进一步调查。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="345" data-image-id="0*rJeZfUo4zXNPqFQd" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*rJeZfUo4zXNPqFQd?is-pending-load=1" data-width="720" height="345" src="https://cdn-images-1.medium.com/max/1067/0*rJeZfUo4zXNPqFQd" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="345" data-image-id="0*rJeZfUo4zXNPqFQd" data-width="720" height="345" src="https://cdn-images-1.medium.com/max/1067/0*rJeZfUo4zXNPqFQd" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      ‘DownAlbum’的例子
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   DownAlbum 也为您提供了下载照片的选项。单击照片即可，这将打开一个新页面，向您展示稍大的照片。只需右键单击并保存照片。
  </p>
  <p class="graf graf--p">
   另一个可选的网站是 ‘
   <a class="markup--anchor markup--p-anchor" data-href="http://instasave.io/" href="http://instasave.io/" rel="noopener noreferrer" target="_blank">
    instasave.io
   </a>
   ’，输入您感兴趣的个人资料的用户名，点击每张照片下面的 ‘下载’ 按钮，就可以保存照片。
  </p>
  <p class="graf graf--p">
   您想下载一个账户上所有可能的照片吗？有一款名为 ‘
   <a class="markup--anchor markup--p-anchor" data-href="https://chrome.google.com/webstore/detail/downloader-for-instagram/olkpikmlhoaojbbmmpejnimiglejmboe?hl=en" href="https://chrome.google.com/webstore/detail/downloader-for-instagram/olkpikmlhoaojbbmmpejnimiglejmboe?hl=en" rel="noopener noreferrer" target="_blank">
    Downloader for Instagram + Direct Message
   </a>
   ’ 的谷歌浏览器插件可以批量下载照片。
  </p>
  <p class="graf graf--p">
   安装插件后，您会在右上角看到一个按钮。
  </p>
  <p class="graf graf--p">
   选择最右边的按钮，以下载完整的个人资料。确保已经完全加载页面，以便下载所有内容。正如您在这个例子中看到的，扎克伯格有141个帖子，但该工具显示只有24个。如果您完全加载页面就能下载所有的照片。您可以自定义范围。
  </p>
  <p class="graf graf--p">
   另外：别忘了 Instagram 上的 “Tagged” 部分，这确实需要您登录，但有时其他图片可以带来很大的启示。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="288" data-image-id="0*IQGhTSmBNFa08orh" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*IQGhTSmBNFa08orh?is-pending-load=1" data-width="720" height="288" src="https://cdn-images-1.medium.com/max/1067/0*IQGhTSmBNFa08orh" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="288" data-image-id="0*IQGhTSmBNFa08orh" data-width="720" height="288" src="https://cdn-images-1.medium.com/max/1067/0*IQGhTSmBNFa08orh" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Downloader for Instagram + Direct Message
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    Instagram Stories
   </strong>
  </h3>
  <p class="graf graf--p">
   Instagram Stories 是类似 Snapchat 的短视频或照片。您可以通过查看个人资料图片来识别个人资料是否包含故事。如果周围有一个彩色圆圈，则表明该个人资料包含故事。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="373" data-image-id="0*_XGcVdfi6ZaBz3nv" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*_XGcVdfi6ZaBz3nv?is-pending-load=1" data-width="720" height="373" src="https://cdn-images-1.medium.com/max/1067/0*_XGcVdfi6ZaBz3nv" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="373" data-image-id="0*_XGcVdfi6ZaBz3nv" data-width="720" height="373" src="https://cdn-images-1.medium.com/max/1067/0*_XGcVdfi6ZaBz3nv" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      扎克伯格没有“story”，BBC有
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   有时，个人资料会对那些突出显示的故事进行分类。您会在简介下方看到这些故事。 单击类别以查看。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="329" data-image-id="0*xBYuiNx6Vc3UiEeP" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*xBYuiNx6Vc3UiEeP?is-pending-load=1" data-width="720" src="https://cdn-images-1.medium.com/max/1067/0*xBYuiNx6Vc3UiEeP" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="329" data-image-id="0*xBYuiNx6Vc3UiEeP" data-width="720" src="https://cdn-images-1.medium.com/max/1067/0*xBYuiNx6Vc3UiEeP"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    对 Stories 进行查找
   </strong>
  </h3>
  <p class="graf graf--p">
   仅当故事标记有位置或主题标签时，才可以搜索。
  </p>
  <p class="graf graf--p">
   该网站为您提供了一个搜索故事的机会，如果您在网站顶部搜索栏中搜索一个标签或地点，会看到一张圆形照片，周围有彩色的圆圈。点击照片，就可以看到与该特定标签或地点相匹配的故事。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="304" data-image-id="0*7_4epusKkm9nK7ZG" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*7_4epusKkm9nK7ZG?is-pending-load=1" data-width="720" height="304" src="https://cdn-images-1.medium.com/max/1067/0*7_4epusKkm9nK7ZG" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="304" data-image-id="0*7_4epusKkm9nK7ZG" data-width="720" height="304" src="https://cdn-images-1.medium.com/max/1067/0*7_4epusKkm9nK7ZG" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      在Instagram上搜索结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   使用 Google Chrome 插件
   <a class="markup--anchor markup--p-anchor" data-href="https://chrome.google.com/webstore/detail/downloader-for-instagram/olkpikmlhoaojbbmmpejnimiglejmboe?hl=en" href="https://chrome.google.com/webstore/detail/downloader-for-instagram/olkpikmlhoaojbbmmpejnimiglejmboe?hl=en" rel="noreferrer noopener" target="_blank">
    Downloader for Instagram
   </a>
   搜索故事要容易一些。
  </p>
  <p class="graf graf--p">
   安装后，您会在右上角看到一个小图标。点击该标志以打开一个新的页面，在那里您会看到菜单，如截图所示；搜索了 “阿姆斯特丹” 这个标签，并选择了有小旗子的那个。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="395" data-image-id="0*xQrBIKmYPnv3hp-O" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*xQrBIKmYPnv3hp-O?is-pending-load=1" data-width="720" height="395" src="https://cdn-images-1.medium.com/max/1067/0*xQrBIKmYPnv3hp-O" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="395" data-image-id="0*xQrBIKmYPnv3hp-O" data-width="720" height="395" src="https://cdn-images-1.medium.com/max/1067/0*xQrBIKmYPnv3hp-O" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      使用“ Downloader for Instagram”的搜索结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   点击黑色小眼睛图标可立即看到故事。
  </p>
  <p class="graf graf--p">
   通过使用箭头（左右键），您可以在故事之间切换。上传故事的用户显示在左侧（在截图中以蓝色遮盖的部分）而且非常有帮助； 该插件也为您提供了仅下载与主题标签相关的一个或所有故事的机会（左上角）。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="426" data-image-id="0*Ji9DF3xDNgMdJY3O" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*Ji9DF3xDNgMdJY3O?is-pending-load=1" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*Ji9DF3xDNgMdJY3O" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="426" data-image-id="0*Ji9DF3xDNgMdJY3O" data-width="650" src="https://cdn-images-1.medium.com/max/1067/0*Ji9DF3xDNgMdJY3O"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜索关键词
   </strong>
  </h3>
  <p class="graf graf--p">
   如果您不是在寻找标签，只是寻找一般使用的词语，Instagram 可能不是最好的搜索地点，正如您在下面左边的截图中看到的那样。
  </p>
  <p class="graf graf--p">
   谷歌、或任何其他搜索引擎都会更好，对于谷歌来说，使用运算符。
  </p>
  <p class="graf graf--p">
   比如这样
   <em class="markup--em markup--p-em">
    Inurl:instagram.com/p/ “keyword”
   </em>
   （用您喜欢的任何关键字替换“
   <em class="markup--em markup--p-em">
    keyword
   </em>
   ”）。在示例中选择的是 “diner time”。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="265" data-image-id="0*mxv90bNdohRoKrbs" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*mxv90bNdohRoKrbs?is-pending-load=1" data-width="720" height="265" src="https://cdn-images-1.medium.com/max/1067/0*mxv90bNdohRoKrbs" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="265" data-image-id="0*mxv90bNdohRoKrbs" data-width="720" height="265" src="https://cdn-images-1.medium.com/max/1067/0*mxv90bNdohRoKrbs" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      左：在Instagram中搜索关键字；右：在Google中搜索关键字
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   现在您看到，其中一个结果中包含了这个关键词。Diner time 并不是作为一个标签使用的，所以如果您在 Instagram 搜索栏中搜索这些关键词，就不会找到这个结果。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="156" data-image-id="0*1tCGxWVwXSPft1A3" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*1tCGxWVwXSPft1A3?is-pending-load=1" data-width="720" height="156" src="https://cdn-images-1.medium.com/max/1067/0*1tCGxWVwXSPft1A3" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="156" data-image-id="0*1tCGxWVwXSPft1A3" data-width="720" height="156" src="https://cdn-images-1.medium.com/max/1067/0*1tCGxWVwXSPft1A3" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Google搜索结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜主题标签
   </strong>
  </h3>
  <p class="graf graf--p">
   当您选择了一个结果，在这种情况下，一个标签，确保不只是检查到前几个照片。这些将是 “Tops”（最受欢迎的）照片，并不总是给您您要找的东西。相反您应该向下滚动查看 “Most Recent”。
  </p>
  <p class="graf graf--p">
   专门搜索主题标签时别忘了加上 #。
  </p>
  <p class="graf graf--p">
   当然，有很多网站可以帮助您搜索 Instagram 使用的主题标签。像
   <a class="markup--anchor markup--p-anchor" data-href="http://pictame.com/" href="http://pictame.com/" rel="noopener noreferrer" target="_blank">
    pictame.com
   </a>
   和
   <a class="markup--anchor markup--p-anchor" data-href="http://hashatit.com/" href="http://hashatit.com/" rel="noopener noreferrer" target="_blank">
    hashatit.com
   </a>
   这样的网站只是其中的一些。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="350" data-image-id="0*ajn-BJw599PDO8GC" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*ajn-BJw599PDO8GC?is-pending-load=1" data-width="720" height="350" src="https://cdn-images-1.medium.com/max/1067/0*ajn-BJw599PDO8GC" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="350" data-image-id="0*ajn-BJw599PDO8GC" data-width="720" height="350" src="https://cdn-images-1.medium.com/max/1067/0*ajn-BJw599PDO8GC" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      在Instagram上搜索主题标签，向下滚动到 ‘Most recent’
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    跟踪主题标签
   </strong>
  </h3>
  <p class="graf graf--p">
   当您找到了一个特定的标签、并想了解最新情况时，一定要登录并按 “关注”，以便关注与该特定标签相关的帖子。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 642px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="370" data-image-id="0*PmjXVw3asX3qjxFQ" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*PmjXVw3asX3qjxFQ?is-pending-load=1" data-width="642" height="370" src="https://cdn-images-1.medium.com/max/1067/0*PmjXVw3asX3qjxFQ" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="642"/>
     <noscript>
      <img alt="" class="graf-image" data-height="370" data-image-id="0*PmjXVw3asX3qjxFQ" data-width="642" height="370" src="https://cdn-images-1.medium.com/max/1067/0*PmjXVw3asX3qjxFQ" width="642"/>
     </noscript>
     <figcaption class="wp-caption-text">
      如何在Instagram上跟随目标主题标签
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    下载主题标签
   </strong>
  </h3>
  <p class="graf graf--p">
   使用 Google Chrome 插件 “ Downloader for Instagram” 时，下载主题标签非常容易。
  </p>
  <p class="graf graf--p">
   将页面加载到所需的程度，然后使用插件下载链接到主题标签的帖子。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="242" data-image-id="0*GhsVc3I_xRwY5Sna" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*GhsVc3I_xRwY5Sna?is-pending-load=1" data-width="720" height="242" src="https://cdn-images-1.medium.com/max/1067/0*GhsVc3I_xRwY5Sna" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="242" data-image-id="0*GhsVc3I_xRwY5Sna" data-width="720" height="242" src="https://cdn-images-1.medium.com/max/1067/0*GhsVc3I_xRwY5Sna" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      使用‘Downloader for Instagram’ 下载带有主题标签的帖子
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜索位置
   </strong>
  </h3>
  <p class="graf graf--p">
   可以通过网站顶部的搜索栏来搜索位置。您可以通过 “drop” 图标识别位置。
  </p>
  <p class="graf graf--p">
   选择一个位置，以查看从该位置发布的故事以及从该位置发布的其他帖子。
  </p>
  <p class="graf graf--p">
   请注意：您不一定要亲自到那个地点。您可以选择任何您喜欢的地点。所以一张站在阿姆斯特丹中央车站前的照片，可以有纽约时代广场的位置，只是因为您告诉 Instagram 照片是在那里拍摄的。如果您想在照片上添加位置，需要让 Instagram 允许您的位置数据。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="292" data-image-id="0*OjtEPFkg1_e1YiLB" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*OjtEPFkg1_e1YiLB?is-pending-load=1" data-width="720" height="292" src="https://cdn-images-1.medium.com/max/1067/0*OjtEPFkg1_e1YiLB" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="292" data-image-id="0*OjtEPFkg1_e1YiLB" data-width="720" height="292" src="https://cdn-images-1.medium.com/max/1067/0*OjtEPFkg1_e1YiLB" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Instagram上的位置搜索结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   国家列表如下所示。选择您感兴趣的国家和城市。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 636px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="450" data-image-id="0*sqIG7SqYPDTBiY5G" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*sqIG7SqYPDTBiY5G?is-pending-load=1" data-width="636" height="450" src="https://cdn-images-1.medium.com/max/1067/0*sqIG7SqYPDTBiY5G" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="636"/>
     <noscript>
      <img alt="" class="graf-image" data-height="450" data-image-id="0*sqIG7SqYPDTBiY5G" data-width="636" height="450" src="https://cdn-images-1.medium.com/max/1067/0*sqIG7SqYPDTBiY5G" width="636"/>
     </noscript>
     <figcaption class="wp-caption-text">
      筛选国家和城市，以查看特定城市的位置
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong>
    搜索标记到某个位置的旧帖子
   </strong>
  </h3>
  <p class="graf graf--p">
   有一个视频讲述了如何找到某个地点的 Instagram 帖子：
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="449" src="//www.youtube.com/embed/FYnfKghpJBw" width="800">
   </iframe>
  </p>
  <p class="graf graf--p">
   Python脚本：
   <a class="markup--anchor markup--p-anchor" data-href="https://repl.it/repls/FormalYellowgreenLinux" href="https://repl.it/repls/FormalYellowgreenLinux" rel="nofollow noopener noreferrer" target="_blank">
    https://repl.it/repls/FormalYellowgreenLinux
   </a>
  </p>
  <p class="graf graf--p">
   向下滚动到 ‘Most recent’ 以查看较旧的帖子。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="190" data-image-id="0*IhDXymBqx7XMJqwJ" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*IhDXymBqx7XMJqwJ?is-pending-load=1" data-width="720" height="190" src="https://cdn-images-1.medium.com/max/1067/0*IhDXymBqx7XMJqwJ" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="190" data-image-id="0*IhDXymBqx7XMJqwJ" data-width="720" height="190" src="https://cdn-images-1.medium.com/max/1067/0*IhDXymBqx7XMJqwJ" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      左图是2011年8月27日的照片，但在 ‘Most recent’ 部分中显示为第一个结果
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    无需工具即可搜索商业帐户的联系方式
   </strong>
  </h3>
  <p class="graf graf--p">
   方法：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    确保在网络浏览器中登录到您的 Instagram 帐户，该账户应该为调查所用，与您的真实身份不应存在任何联系；
   </li>
   <li class="graf graf--li">
    访问您感兴趣的帐户，并检查该帐户是否为商业帐户。您可以使用
    <a class="markup--anchor markup--li-anchor" data-href="https://chrome.google.com/webstore/detail/helper-tools-for-instagra/hcdbfckhdcpepllecbkaaojfgipnpbpb" href="https://chrome.google.com/webstore/detail/helper-tools-for-instagra/hcdbfckhdcpepllecbkaaojfgipnpbpb" rel="noreferrer noopener" target="_blank">
     Helper Tools
    </a>
    工具进行检查，但也可以通过继续以下步骤试试运气；
   </li>
   <li class="graf graf--li">
    现在需要检索 Instagram 用户ID。您可以通过右键单击空白位置选择 “查看页面源码”（或使用 Ctrl + U，在大多数浏览器中都可以使用）；
   </li>
   <li class="graf graf--li">
    使用 Ctrl + F 搜索 profilePage _（“ profilePage_” 后面的数字是您需要复制的数字；
   </li>
  </ul>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="82" data-image-id="0*nrCBj9jp-C0xIYnJ" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*nrCBj9jp-C0xIYnJ?is-pending-load=1" data-width="720" height="82" src="https://cdn-images-1.medium.com/max/1067/0*nrCBj9jp-C0xIYnJ" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="82" data-image-id="0*nrCBj9jp-C0xIYnJ" data-width="720" height="82" src="https://cdn-images-1.medium.com/max/1067/0*nrCBj9jp-C0xIYnJ" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      星巴克Instagram页面的用户ID示例
     </figcaption>
    </figure>
   </p>
  </figure>
  <ul class="postList">
   <li class="graf graf--li">
    现在打开一个新标签并粘贴以下 URL。将 “ID” 替换为您在感兴趣的页面上找到的ID号。
   </li>
   <li class="graf graf--li">
    <a class="markup--anchor markup--li-anchor" data-href="https://i.instagram.com/api/v1/users/" href="https://i.instagram.com/api/v1/users/" rel="nofollow noopener noreferrer" target="_blank">
     https://i.instagram.com/api/v1/users/
    </a>
    <strong class="markup--strong markup--li-strong">
     ID
    </strong>
    /info/
    <br/>
    (e.g.
    <a class="markup--anchor markup--li-anchor" data-href="https://i.instagram.com/api/v1/users/1034466/info" href="https://i.instagram.com/api/v1/users/1034466/info" rel="nofollow noopener noreferrer" target="_blank">
     <em class="markup--em markup--li-em">
      https://i.instagram.com/api/v1/users/1034466/info
     </em>
    </a>
    )
   </li>
  </ul>
  <p class="graf graf--p">
   现在您就可以查看该商业帐户已填写的信息了。
  </p>
  <p class="graf graf--p">
   以星巴克为例，结果将如下所示：
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="583" data-image-id="0*4T3wMRLpjkAByQbk" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*4T3wMRLpjkAByQbk?is-pending-load=1" data-width="720" height="583" src="https://cdn-images-1.medium.com/max/1067/0*4T3wMRLpjkAByQbk" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="583" data-image-id="0*4T3wMRLpjkAByQbk" data-width="720" height="583" src="https://cdn-images-1.medium.com/max/1067/0*4T3wMRLpjkAByQbk" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      您会看到“ is_business”设置为TRUE，并且可以看到电子邮件地址和电话号码
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   在联系方式旁边还可以收集到很多其他有趣的东西，比如 ‘instagram_location_id’。如果您
   <strong class="markup--strong markup--p-strong">
    复制这个数字，并把它放在 ‘facebook.com’ 后面 (facebook.com/22092443056)，它就会显示星巴克的 facebook 账号
   </strong>
   。
  </p>
  <p class="graf graf--p">
   其他可能有趣的东西包括关注的人/粉丝的确切数量等等。您可以自己试试。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜索已被删除的 Instagram 内容
   </strong>
  </h3>
  <p class="graf graf--p">
   您一定知道，在线内容的删除速度可以与上传一样快。因此，搜索任何已删除的内容的技巧都非常重要。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    您可以在这里看到相关的综合性手册 《如
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%bf%ab%e9%80%9f%e6%89%be%e5%88%b0%e4%bd%a0%e6%83%b3%e8%a6%81%e7%9a%84%e4%b8%9c%e8%a5%bf%ef%bc%9a%e8%bf%bd%e8%b8%aa%e6%95%b0%e5%ad%97%e8%af%81%e6%8d%ae%e7%9a%84%e5%b0%8f%e6%8a%80/" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%bf%ab%e9%80%9f%e6%89%be%e5%88%b0%e4%bd%a0%e6%83%b3%e8%a6%81%e7%9a%84%e4%b8%9c%e8%a5%bf%ef%bc%9a%e8%bf%bd%e8%b8%aa%e6%95%b0%e5%ad%97%e8%af%81%e6%8d%ae%e7%9a%84%e5%b0%8f%e6%8a%80/" rel="noopener noreferrer" target="_blank">
     何快速找到你想要的东西：追踪数字证据的小技巧
    </a>
    》
   </li>
  </ul>
  <p class="graf graf--p">
   如上面文章所述，
   <a class="markup--anchor markup--p-anchor" data-href="http://archive.org/" href="https://archive.org/" rel="noopener noreferrer" target="_blank">
    Archive.org
   </a>
   是一个很好的资源，以 DJ Hardwell 的 Instagram 资料为例（点击
   <a class="markup--anchor markup--p-anchor" data-href="https://web.archive.org/web/20170326031437/https://www.instagram.com/hardwell/" href="https://web.archive.org/web/20170326031437/https://www.instagram.com/hardwell/" rel="noopener noreferrer" target="_blank">
    这里
   </a>
   查看已存档的资料，点击
   <a class="markup--anchor markup--p-anchor" data-href="https://www.instagram.com/hardwell/" href="https://www.instagram.com/hardwell/" rel="noopener noreferrer" target="_blank">
    这里
   </a>
   查看当前的资料），来查找 Instagram 的旧帖子。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="231" data-image-id="0*W5Is8Q9Ct10PXvF_" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*W5Is8Q9Ct10PXvF_?is-pending-load=1" data-width="720" height="231" src="https://cdn-images-1.medium.com/max/1067/0*W5Is8Q9Ct10PXvF_" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="231" data-image-id="0*W5Is8Q9Ct10PXvF_" data-width="720" height="231" src="https://cdn-images-1.medium.com/max/1067/0*W5Is8Q9Ct10PXvF_" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      左：Archive.org 右：Instagram.com/hardwell
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   再有，当研究任何名人的时候，有很大的可能性会遇到其他的模仿名人的账号。例如；有多个真人秀明星卡戴珊的账号，他们在 Instagram 上转发她的一切，或者将她在 Snapchat 上发布的所有内容都发布在 Instagram 账号上。
  </p>
  <p class="graf graf--p">
   通过查看这些 “粉丝帐户”，您也许可以找到可能原账户中已经被删除的所有数据。
  </p>
  <p class="graf graf--p">
   搜索已删除内容的另一种方法是使用 Google。
  </p>
  <p class="graf graf--p">
   您可能知道有很多不同的网站也会将 Instagram 的帖子来显示在他们的网站上。通过使用谷歌Dorks，您可以找到使用 Instagram 帖子的网站，也许能找到一些被删除的内容。
  </p>
  <p class="graf graf--p">
   比如这样：
   <em class="markup--em markup--p-em">
    -site:instagram.com instagram keyword -twitter
   </em>
  </p>
  <p class="graf graf--p">
   -site:instagram.com = 排除此网站的任何结果
  </p>
  <p class="graf graf--p">
   instagram = 专注于 instagram 帖子
  </p>
  <p class="graf graf--p">
   keyword = 用您想要的关键字和用户名来替换这个位置
  </p>
  <p class="graf graf--p">
   -twitter = 排除推特，因为推特在此有很多误报
  </p>
  <p class="graf graf--p">
   例如：
   <em class="markup--em markup--p-em">
    -site:instagram.com instagram hardwell -twitter
   </em>
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="253" data-image-id="0*q5Kh1rX4MZCu6Qy6" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*q5Kh1rX4MZCu6Qy6?is-pending-load=1" data-width="720" height="253" src="https://cdn-images-1.medium.com/max/1067/0*q5Kh1rX4MZCu6Qy6" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="253" data-image-id="0*q5Kh1rX4MZCu6Qy6" data-width="720" height="253" src="https://cdn-images-1.medium.com/max/1067/0*q5Kh1rX4MZCu6Qy6" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Example: -site:instagram.com instagram hardwell -twitter
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   或者您可以尝试设置一个网络监控工具来检测网站的变化。这种工具可以捕捉到页面上的任何变化，这样您就不会错过任何更新的帖子。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    在 Twitter 上搜索 Instagram 的内容
   </strong>
  </h3>
  <p class="graf graf--p">
   查找您可能感兴趣的人的 Instagram 帐户或与特定主题相关的任何帖子的另一种方法是通过 Twitter。
  </p>
  <p class="graf graf--p">
   首先，您不需要 Twitter 的账户就可以搜索 Twitter。只需导航到 Twitter.com/explore，使用其顶部的搜索栏。
  </p>
  <p class="graf graf--p">
   要搜索 Instagram 内容，请使用以下搜索查询：
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://twitter.com/search?q=instagram.com%2Fp&amp;src=typed_query&amp;f=live" href="https://twitter.com/search?q=instagram.com%2Fp&amp;src=typed_query&amp;f=live" rel="noreferrer noopener" target="_blank">
    instagram.com/p
   </a>
   将显示包含 “instagram.com/p” 的推文；
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://twitter.com/search?q=source%3Ainstagram%20party&amp;src=typed_query&amp;f=live" href="https://twitter.com/search?q=source%3Ainstagram%20party&amp;src=typed_query&amp;f=live" rel="noreferrer noopener" target="_blank">
    source:Instagram party
   </a>
   将在 Instagram 帖子中显示包含 “party” 一词的推文。将 “party” 一词更改为您要查找的任何内容；
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://twitter.com/search?q=filter%3Alinks%20instagram&amp;src=typed_query&amp;f=live" href="https://twitter.com/search?q=filter%3Alinks%20instagram&amp;src=typed_query&amp;f=live" rel="noreferrer noopener" target="_blank">
    instagram filter:links
   </a>
   包含网址和单词 “Instagram” 的推文。
  </p>
  <p class="graf graf--p">
   执行这些查询时，请确保切换到 “最新” 推文以查看最新帖子。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    不要错过，一些很好玩的技巧《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e4%bb%8e%e6%8e%a8%e7%89%b9%e4%b8%ad%e6%8c%96%e6%8e%98%e7%9c%9f%e7%9b%b8%e4%b8%8d%e9%9c%80%e8%a6%81%e5%a4%aa%e5%a4%8d%e6%9d%82%e7%9a%84%e5%b7%a5%e5%85%b7%ef%bc%9a%e4%b8%80%e4%b8%aa%e5%b8%b8%e7%94%a8/" href="https://www.iyouport.org/%e4%bb%8e%e6%8e%a8%e7%89%b9%e4%b8%ad%e6%8c%96%e6%8e%98%e7%9c%9f%e7%9b%b8%e4%b8%8d%e9%9c%80%e8%a6%81%e5%a4%aa%e5%a4%8d%e6%9d%82%e7%9a%84%e5%b7%a5%e5%85%b7%ef%bc%9a%e4%b8%80%e4%b8%aa%e5%b8%b8%e7%94%a8/" rel="noopener noreferrer" target="_blank">
     从推特中挖掘真相不需要太复杂的工具：一个常用工具的全面指南
    </a>
    》
   </li>
   <li class="graf graf--li">
    工具介绍《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e6%b7%b1%e6%8c%96%e6%8e%a8%e7%89%b9%ef%bc%9a%e6%8f%90%e4%be%9b%e6%8a%80%e5%b7%a7%e3%80%81%e5%b7%a5%e5%85%b7%e5%92%8c%e5%b9%b3%e5%8f%b0/" href="https://www.iyouport.org/%e6%b7%b1%e6%8c%96%e6%8e%a8%e7%89%b9%ef%bc%9a%e6%8f%90%e4%be%9b%e6%8a%80%e5%b7%a7%e3%80%81%e5%b7%a5%e5%85%b7%e5%92%8c%e5%b9%b3%e5%8f%b0/" rel="noopener noreferrer" target="_blank">
     深挖推特：提供技巧、工具和平台
    </a>
    》
   </li>
   <li class="graf graf--li">
    以及《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%e7%a4%be%e4%ba%a4%e7%bd%91%e7%ab%99%e4%b8%8a%e8%bf%9b%e8%a1%8c%e6%96%b0%e9%97%bb%e6%94%b6%e9%9b%86%e5%92%8c%e7%9b%91%e8%a7%86%e7%9a%84%e5%9f%ba%e6%9c%ac%e6%8c%87%e5%8d%97/" href="https://www.iyouport.org/%e7%a4%be%e4%ba%a4%e7%bd%91%e7%ab%99%e4%b8%8a%e8%bf%9b%e8%a1%8c%e6%96%b0%e9%97%bb%e6%94%b6%e9%9b%86%e5%92%8c%e7%9b%91%e8%a7%86%e7%9a%84%e5%9f%ba%e6%9c%ac%e6%8c%87%e5%8d%97/" rel="noopener noreferrer" target="_blank">
     社交网站上进行新闻收集和监视的基本指南
    </a>
    》
   </li>
  </ul>
  <p class="graf graf--p">
   比如您可以更精确地搜索：
   <a class="markup--anchor markup--p-anchor" data-href="https://twitter.com/search?q=instagram.com%2Fp%20near%3AAmsterdam%20within%3A15mi&amp;src=typed_query&amp;f=live" href="https://twitter.com/search?q=instagram.com%2Fp%20near%3AAmsterdam%20within%3A15mi&amp;src=typed_query&amp;f=live" rel="noreferrer noopener" target="_blank">
    instagram.com/p near:Amsterdam within:15mi
   </a>
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="182" data-image-id="0*SHVIHY1Zg2id0-BW" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*SHVIHY1Zg2id0-BW?is-pending-load=1" data-width="720" height="182" src="https://cdn-images-1.medium.com/max/1067/0*SHVIHY1Zg2id0-BW" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="182" data-image-id="0*SHVIHY1Zg2id0-BW" data-width="720" height="182" src="https://cdn-images-1.medium.com/max/1067/0*SHVIHY1Zg2id0-BW" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      不要忘记选择“最新”以查看最新帖子
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜索标记到某个位置的较旧照片
   </strong>
  </h3>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="http://twitter.com/osintcombine" href="https://twitter.com/osintcombine" rel="noreferrer noopener" target="_blank">
    OSINT Combine
   </a>
   现在可帮助您查找标记到 Instagram 位置的旧照片（
   <a class="markup--anchor markup--p-anchor" data-href="https://www.osintcombine.com/instagram-explorer" href="https://www.osintcombine.com/instagram-explorer" rel="noopener noreferrer" target="_blank">
    单击此处
   </a>
   ）。
  </p>
  <p class="graf graf--p">
   OSINT Combine 的工作原理非常简单，只需粘贴任何给定 Instagram 位置的 URL，并调整日期。点击绿色的搜索图标进行搜索，向下滚动到 “最近的” 部分，就可以了。
  </p>
  <p class="graf graf--p">
   请注意，Instagram 于2011年8月24日上线，您不会找到该日期之前的任何帖子。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="432" data-image-id="0*bkG_ybq7v8qwtt_Q" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*bkG_ybq7v8qwtt_Q?is-pending-load=1" data-width="720" height="432" src="https://cdn-images-1.medium.com/max/1067/0*bkG_ybq7v8qwtt_Q" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="432" data-image-id="0*bkG_ybq7v8qwtt_Q" data-width="720" height="432" src="https://cdn-images-1.medium.com/max/1067/0*bkG_ybq7v8qwtt_Q" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      1、在Instagram上搜索您要的位置，选择位置并复制URL；2、在“查找照片”框中粘贴所选的网址，选择一个日期，然后点击绿色按钮；3、在 Instagram 中向下滚动至“Most recent”以查看所选日期的照片
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    仅搜索 Instagram 视频的内容
   </strong>
  </h3>
  <p class="graf graf--p">
   如果您只搜索用特定标签分享的视频，可以使用
   <a class="markup--anchor markup--p-anchor" data-href="http://skimagram.com/" href="http://skimagram.com/" rel="noopener noreferrer" target="_blank">
    skimagram.com
   </a>
   。
  </p>
  <p class="graf graf--p">
   只需输入您要找的标签，然后选择（右边下图红框所示）是要找视频还是帖子。选择视频图标，才能只搜索视频。
  </p>
  <p class="graf graf--p">
   请注意：这将只搜索视频，不搜索 Instagram Stories。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="164" data-image-id="0*9BJH4584_OsvJg8s" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*9BJH4584_OsvJg8s?is-pending-load=1" data-width="720" src="https://cdn-images-1.medium.com/max/1067/0*9BJH4584_OsvJg8s" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="164" data-image-id="0*9BJH4584_OsvJg8s" data-width="720" src="https://cdn-images-1.medium.com/max/1067/0*9BJH4584_OsvJg8s"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    搜索多个主题标签
   </strong>
  </h3>
  <p class="graf graf--p">
   Instagram.com 并不能让您轻松搜索多个标签。而这可能是您需要做的事以便缩小调查的相关结果。虽然还没有碰到专门为此而设计的搜索引擎，但谷歌可以在这段时间内帮您做到。
  </p>
  <p class="graf graf--p">
   使用下面的谷歌Dorks，以便搜索多个标签。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="123" data-image-id="0*Plnn0ZPXIRrMmTdx" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*Plnn0ZPXIRrMmTdx?is-pending-load=1" data-width="720" src="https://cdn-images-1.medium.com/max/1067/0*Plnn0ZPXIRrMmTdx" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="123" data-image-id="0*Plnn0ZPXIRrMmTdx" data-width="720" src="https://cdn-images-1.medium.com/max/1067/0*Plnn0ZPXIRrMmTdx"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   由于某些原因，
   <strong class="markup--strong markup--p-strong">
    是否将标签放在引号内会得到不同的结果。所以请确保您同时尝试这两种方法
   </strong>
   ，以100% 确保您搜索到了所有可能的选项。而且您可以根据自己的需要来扩展这个功能。
  </p>
  <p class="graf graf--p">
   如果您不确定一个标签是如何拼写的，或者想知道是否有包含更多单词的标签，请查看
   <a class="markup--anchor markup--p-anchor" data-href="https://keywordtool.io/instagram" href="https://keywordtool.io/instagram" rel="noopener noreferrer" target="_blank">
    Keywordtool.io/instagram
   </a>
   。Keywordtool 让您可以只搜索标签的前几个字母，它会完成尽可能多的可能选项。它还会指出有多少帖子可以找到该特定标签。
  </p>
  <p class="graf graf--p">
   一个额外的好处是，您还可以搜索谷歌、YouTube、Bing、亚马逊、eBay、Play Store 和 Twitter。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="297" data-image-id="0*T3XByITIhs6kNioW" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*T3XByITIhs6kNioW?is-pending-load=1" data-width="720" height="297" src="https://cdn-images-1.medium.com/max/1067/0*T3XByITIhs6kNioW" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="297" data-image-id="0*T3XByITIhs6kNioW" data-width="720" height="297" src="https://cdn-images-1.medium.com/max/1067/0*T3XByITIhs6kNioW" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      keywordtool.io/instagram 的示例
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    在 Instagram 帖子中搜索关键字
   </strong>
  </h3>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="http://mulpix.com/instagram/" href="http://mulpix.com/instagram/" rel="noopener noreferrer" target="_blank">
    mulpix.com/instagram
   </a>
   这个工具为您提供了在帖子和视频之间过滤的选项。它还提供了一些关于使用的关键词的统计。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="259" data-image-id="0*Hmdg55yCqzxNjzpw" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*Hmdg55yCqzxNjzpw?is-pending-load=1" data-width="720" height="259" src="https://cdn-images-1.medium.com/max/1067/0*Hmdg55yCqzxNjzpw" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="259" data-image-id="0*Hmdg55yCqzxNjzpw" data-width="720" height="259" src="https://cdn-images-1.medium.com/max/1067/0*Hmdg55yCqzxNjzpw" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      mulpix.com/instagram 的示例
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    匿名查看 stories
   </strong>
  </h3>
  <p class="graf graf--p">
   想匿名查看公开的故事吗？使用
   <a class="markup--anchor markup--p-anchor" data-href="http://stalker-stories.com/" href="http://stalker-stories.com/" rel="noopener noreferrer" target="_blank">
    stalker-stories.com
   </a>
   可以做到，而无需登录 Instagram 帐户。
  </p>
  <p class="graf graf--p">
   额外的好处是该网站还允许您下载故事。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="332" data-image-id="0*9hzbS1iANf4We82V" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*9hzbS1iANf4We82V?is-pending-load=1" data-width="720" height="332" src="https://cdn-images-1.medium.com/max/1067/0*9hzbS1iANf4We82V" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="332" data-image-id="0*9hzbS1iANf4We82V" data-width="720" height="332" src="https://cdn-images-1.medium.com/max/1067/0*9hzbS1iANf4We82V" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Stalkerstories.com
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    跟踪您 “关注” 的人
   </strong>
  </h3>
  <p class="graf graf--p">
   The Wired 写了一篇文章，介绍了这款非常有趣的应用，名为 “Who’s In Town”。
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    在这里看到《
    <a class="markup--anchor markup--li-anchor" data-href="https://www.iyouport.org/%E6%AD%A4%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F%E8%AE%A9%E6%82%A8%E7%9A%84-instagram-%E7%B2%89%E4%B8%9D%E8%B7%9F%E8%B8%AA%E6%82%A8%E7%9A%84%E4%BD%8D%E7%BD%AE/" href="https://www.iyouport.org/%E6%AD%A4%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F%E8%AE%A9%E6%82%A8%E7%9A%84-instagram-%E7%B2%89%E4%B8%9D%E8%B7%9F%E8%B8%AA%E6%82%A8%E7%9A%84%E4%BD%8D%E7%BD%AE/" rel="noopener noreferrer" target="_blank">
     此应用程序让您的 Instagram 粉丝跟踪您的位置
    </a>
    》
   </li>
  </ul>
  <p class="graf graf--p">
   这款应用可以让您连接到 Instagram 账户，这样就可以看到您关注的人在哪里登入了。
  </p>
  <p class="graf graf--p">
   在地图上，您可以看到他们去了哪里 (这可能包括他们住的地方、工作地点、吃饭的地方、锻炼的地方等)。
  </p>
  <p class="graf graf--p">
   如果您有一个专门用来调查的匿名账户、关注一个特定类型的人，这可以给您一个非常好的洞察力，关于他们可能会去哪里，他们可能喜欢什么。
  </p>
  <p class="graf graf--p graf--startsWithSingleQuote">
   ‘Who’s in Town?’ 适合iOS和安卓，
   <a class="markup--anchor markup--p-anchor" data-href="https://whosintown.app/" href="https://whosintown.app/" rel="noopener noreferrer" target="_blank">
    在这里下载
   </a>
   。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="295" data-image-id="0*-xLCaHoTalfOrblv" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*-xLCaHoTalfOrblv?is-pending-load=1" data-width="720" height="295" src="https://cdn-images-1.medium.com/max/1067/0*-xLCaHoTalfOrblv" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="295" data-image-id="0*-xLCaHoTalfOrblv" data-width="720" height="295" src="https://cdn-images-1.medium.com/max/1067/0*-xLCaHoTalfOrblv" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Whosintown.app
     </figcaption>
    </figure>
   </p>
  </figure>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    了解您关注的人/粉丝最活跃的时间
   </strong>
  </h3>
  <p class="graf graf--p">
   比方说，您有一个有很多粉丝的研究资料（必须超过100个），您有兴趣知道他们中谁可能是最活跃的。也许是因为您可以为他们量身定做帖子，或者，您可以更多了解关于您的目标群体，这对活动家来说就很有用。
  </p>
  <p class="graf graf--p">
   在这种情况下，您可以考虑将您的 Instagram 账户切换到 “商业” 账户。这是您可以自己做的一个选项，不需要 Instagram 的许可。
  </p>
  <p class="graf graf--p">
   以下是您如何在您的个人资料中开启它（注意：只有通过手机应用才能实现）。
  </p>
  <ol class="postList">
   <li class="graf graf--li">
    在移动应用程序中打开您的 Instagram 帐户
   </li>
   <li class="graf graf--li">
    单击右下角的应用程序中的小人儿图标
   </li>
   <li class="graf graf--li">
    选择右上角的三条线菜单
   </li>
   <li class="graf graf--li">
    选择 “设置”
   </li>
   <li class="graf graf--li">
    选择 “帐户”
   </li>
   <li class="graf graf--li">
    选择 “切换到商业账户”
   </li>
  </ol>
  <p class="graf graf--p">
   现在您会被要求提供一些联系细节，如您的电子邮件地址、电话号码、或地理位置。这是为了让您的客户可以联系您 —— 要知道，这也意味着查看您个人资料的人，可以认出您是一个商业账户。
  </p>
  <p class="graf graf--p">
   如果您有一百个或更多的关注者，则可以看
   <a class="markup--anchor markup--p-anchor" data-href="https://help.instagram.com/1533933820244654" href="https://help.instagram.com/1533933820244654" rel="noreferrer noopener" target="_blank">
    Insights
   </a>
   。Insights 是对您的关注者的分析。您可以了解到您的追随者何时活跃，他们的性别、他们的年龄、以及更多。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    特定 Instagram 个人资料的统计信息
   </strong>
  </h3>
  <p class="graf graf--p">
   Stalkture.com 可以向你展示更多的数据。下面是扎克伯格个人资料的统计数据：
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 720px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="306" data-image-id="0*5SVeLw0n26NfhJVK" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*5SVeLw0n26NfhJVK?is-pending-load=1" data-width="720" height="306" src="https://cdn-images-1.medium.com/max/1067/0*5SVeLw0n26NfhJVK" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="720"/>
     <noscript>
      <img alt="" class="graf-image" data-height="306" data-image-id="0*5SVeLw0n26NfhJVK" data-width="720" height="306" src="https://cdn-images-1.medium.com/max/1067/0*5SVeLw0n26NfhJVK" width="720"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Stalkture.com/a/zuck/314216 的示例
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   向下滚动时，您不仅会看到排名统计信息，还会看到各种过滤器，如最受欢迎的/被评论的/被点赞的帖子等等。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://osintcurio.us/2019/07/16/searching-instagram/" href="https://osintcurio.us/2019/07/16/searching-instagram/" rel="noopener noreferrer" target="_blank">
    Searching Instagram
   </a>
  </p>
  <div id="atatags-1611829871-5fe0836550396">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-15171" href="https://www.iyouport.org/%e5%9c%a8%e6%9c%80%e9%9a%be%e6%90%9c%e7%b4%a2%e7%9a%84%e5%9c%b0%e6%96%b9%ef%bc%9a%e8%a7%a3%e5%89%96-instagram-%e7%94%a8%e6%88%b7/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Twitter 上共享">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击以在 Twitter 上共享（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-15171" href="https://www.iyouport.org/%e5%9c%a8%e6%9c%80%e9%9a%be%e6%90%9c%e7%b4%a2%e7%9a%84%e5%9c%b0%e6%96%b9%ef%bc%9a%e8%a7%a3%e5%89%96-instagram-%e7%94%a8%e6%88%b7/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击以在 Facebook 上共享">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-15171-5fe0836550f52" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=15171&amp;origin=www.iyouport.org&amp;obj_id=161182987-15171-5fe0836550f52" id="like-post-wrapper-161182987-15171-5fe0836550f52">
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
    <a href="https://www.iyouport.org/tag/instagram/" rel="tag">
     Instagram
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
    <a href="https://www.iyouport.org/tag/technique/" rel="tag">
     technique
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
   <time class="entry-date published" datetime="2020-11-20T00:03:11+08:00">
    2020年11月20日
   </time>
   <time class="updated" datetime="2020-11-20T00:03:04+08:00">
    2020年11月20日
   </time>
  </div>
 </div>
</article>

