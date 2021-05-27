---
layout: post
title: "如何在Linux上使用GnuPG进行加密 - iYouPort"
date: 2021-05-25T16:04:11+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8linux%e4%b8%8a%e4%bd%bf%e7%94%a8gnupg%e8%bf%9b%e8%a1%8c%e5%8a%a0%e5%af%86/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16112 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-54 tag-encryption tag-linux tag-security tag-technology" id="post-16112">
 <header class="entry-header">
  <h1 class="entry-title">
   如何在Linux上使用GnuPG进行加密
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
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-05-26T00:04:11+08:00">
    2021年5月26日
   </time>
   <time class="updated" datetime="2021-02-26T12:23:27+08:00">
    2021年2月26日
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
       想要在Linux上发送和接收安全的电子邮件吗？以下是使用GnuPG创建和管理加密电子邮件的简单方法
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1500" data-image-id="0*MAngz-PFBaZe0rRb" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*MAngz-PFBaZe0rRb?is-pending-load=1" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*MAngz-PFBaZe0rRb" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1500" data-image-id="0*MAngz-PFBaZe0rRb" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*MAngz-PFBaZe0rRb"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   您是否曾经有一些敏感信息，如密码或服务器登录信息需要通过电子邮件发送给别人，但不知道如何安全地发送以避免信息落入坏人手中？
  </p>
  <p class="graf graf--p">
   在这里，您将学习如何通过流行的gnupg 工具安全地传输用PGP加密的邮件和文件。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     安装gnupg
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   如果您从来没有听说过PGP，请查看
   <a class="markup--anchor markup--p-anchor" data-href="https://www.makeuseof.com/tag/pgp-me-pretty-good-privacy-explained/" href="https://www.makeuseof.com/tag/pgp-me-pretty-good-privacy-explained/" rel="noopener" target="_blank">
    一个优秀的PGP入门和解释
   </a>
   ，其中包含了各种细节，为了简洁起见，我们在这里就不多说了。首先检查是否已经安装了gnupg. 在终端中, 运行命令:
  </p>
  <pre class="graf graf--p">gnupg — version</pre>
  <p class="graf graf--p">
   如果它显示了您当前正在运行的 gnupg 的版本（应为v2 +），那么说明您已经准备就绪，可以继续进行下一部分。否则，您可以通过运行以下命令安装gnupg：
  </p>
  <pre class="graf graf--p">sudo apt-get install gnupg2</pre>
  <p class="graf graf--p">
   完成后，检查一下确保已安装：
  </p>
  <pre class="graf graf--p">gnupg — version</pre>
  <p class="graf graf--p">
   如果正确安装了gnupg，它将显示版本号。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     生成PGP密钥
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   使用非对称加密技术，您首先要生成一个PGP密钥对，它由公钥和私钥组成。公钥可以自由地分配给任何您想接收加密信息的人，而私钥则被保存在一个安全的地方，只有您自己知道。
  </p>
  <p class="graf graf--p">
   然后，人们可以将信息加密到公钥，并发送加密的信息，然后可以使用私钥解密。要生成密钥对运行以下命令：
  </p>
  <pre class="graf graf--p">gpg — generate-key</pre>
  <p class="graf graf--p">
   这将从询问您的姓名和电子邮件地址开始，这不一定是您的真实姓名和电子邮件。然而，当选择加密信息的对象时，其他人会看到它，所以您应该确保它是别人很容易识别您的东西。
  </p>
  <p class="graf graf--p">
   接下来输入字母O来确认姓名和电子邮件地址，然后会提示您输入一个所需的密码，可以是任何您想要的。每次您想解密发给您的信息时，都需要输入这个密码。
  </p>
  <p class="graf graf--p">
   一旦确认了密码，它就会开始生成新的PGP密钥对，这可能需要几分钟的时间从您的电脑中收集足够的熵/随机数据。您可以离开终端几分钟做一些别的事，直到您看到一条消息说您的密钥已经成功生成。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     导出您的公钥
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在您的密钥对已经生成了，您需要导出公钥来分发给其他人。在终端机上运行该命令：
  </p>
  <pre class="graf graf--p">gpg -a — export -e ‘<a class="__cf_email__" data-cfemail="5e3327303f333b1e3a31333f3730703d3133" href="/cdn-cgi/l/email-protection">[email protected]</a>` &gt; mykey.asc</pre>
  <p class="graf graf--p">
   确保将 “
   <a class="__cf_email__" data-cfemail="5934203738343c193d3634383037773a3634" href="/cdn-cgi/l/email-protection">
    [email protected]
   </a>
   ” 改为您在生成PGP密钥时提供的电子邮件地址。现在您会在当前目录下看到一个名为 mykey.asc 的新文件。把这个文件发送给任何您希望能给您发送加密信息的人.
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     导入公钥
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   就像您现在可以和别人分享您的公钥一样，别人也会和您分享他们的公钥。当您收到别人的PGP公钥时，将文件保存到一个目录下，从同一个目录下访问终端，运行：
  </p>
  <pre class="graf graf--p">gpg — import key.asc</pre>
  <p class="graf graf--p">
   这将会把这个人的公共PGP密钥导入到gnupg中，允许您开始向他们发送加密信息。您可以在任何时候查看当前在gnupg中可用的所有PGP密钥列表：
  </p>
  <pre class="graf graf--p">gpg — list-keys</pre>
  <p class="graf graf--p">
   您将看到一堆看起来类似于下面的条目：
  </p>
  <pre class="graf graf--pre"><code>pub rsa3072 2020-01-30 [SC] [expires: 2022-01-29]</code></pre>
  <pre class="graf graf--pre"><code>8978168C4E79A08553E5789CD42A4A4EC1468CFE</code></pre>
  <pre class="graf graf--pre"><code>uid [ unknown] Matt Dizak &lt;<a class="__cf_email__" data-cfemail="3f525e4b4b115b56455e547f58525e5653115c5052" href="/cdn-cgi/l/email-protection">[email protected]</a>&gt;</code></pre>
  <p class="graf graf--p">
   您需要注意的唯一信息是条目的名称和电子邮件地址，其中说明了该密钥的所有者。当加密信息时，您只需要收件人的电子邮件地址即可。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     通过PGP加密邮件
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   例如，您可能需要发送一些敏感信息给您的网页设计师，而您的PGP密钥已经被导入到您的邮箱地址
   <a class="__cf_email__" data-cfemail="fc98998f959b92998ebc9893919d9592d29f9391" href="/cdn-cgi/l/email-protection">
    [email protected]
   </a>
   。键入所需的信息，并将其保存到一个文本文件中，例如：message.txt。在终端机中，在 mail.txt 所在的目录下，运行命令：
  </p>
  <pre class="graf graf--p">gpg -e -a -r ‘<a class="__cf_email__" data-cfemail="0165647268666f647341656e6c60686f2f626e6c" href="/cdn-cgi/l/email-protection">[email protected]</a>’ message.txt</pre>
  <p class="graf graf--p">
   快速解释上面的命令：
  </p>
  <p class="graf graf--p">
   -e 表示您要加密数据。
   <br/>
   -a 表示您希望以ASCII或纯文本格式输出。
   <br/>
   -r 代表收件人，因此它的后面是您的设计师的电子邮件地址。
   <br/>
   最后是您要加密的信息文件。
  </p>
  <p class="graf graf--p">
   最有可能的是，这将要求您确认您确实希望加密到这个公钥，只需按Y键表示同意。一个新的 message.txt.asc 文件将被创建，如果您在文本编辑器中打开这个文件，会看到类似这样的内容：
  </p>
  <pre class="graf graf--pre"><code>-----BEGIN PGP MESSAGE-----</code></pre>
  <pre class="graf graf--pre"><code>hQGMAzCBDnMltq9zAQv/ZHQ3tJq+feazdLa3thzQE2bhPx+7WaPZcX7SdkoyuKvw</code></pre>
  <pre class="graf graf--pre"><code>9faS7h9OwBjQ4vUyDKespSq3ZNf1pRgNoXijjs3MGEi5IsYxDgNWo1ZJv2qQqp36</code></pre>
  <pre class="graf graf--pre"><code>.....</code></pre>
  <pre class="graf graf--pre"><code>-----END PGP MESSAGE-----</code></pre>
  <p class="graf graf--p">
   这是新生成的加密形式的信息。您可以在电子邮件中附加这个文件，或者简单地将这个文件的内容复制并粘贴到电子邮件的正文内容中。
  </p>
  <p class="graf graf--p">
   然后，收件人将能够使用他们的私钥在他们的终端上解密消息，确保任何人在传输过程中看到这条消息时无法查看纯文本版本。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     加密二进制文件
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   以上介绍了如何加密文本信息，但二进制文件呢？工作原理大同小异，例如要加密一个名为 images.zip 的文件，在终端运行以下命令：
  </p>
  <pre class="graf graf--p">gpg -e -r ‘<a class="__cf_email__" data-cfemail="b7d3d2c4ded0d9d2c5f7d3d8dad6ded999d4d8da" href="/cdn-cgi/l/email-protection">[email protected]</a>’ images.zip</pre>
  <p class="graf graf--p">
   唯一不同的是去掉了-a选项，以及输出文件的名称。然后和之前一样，如果提示确认使用该公钥，只需按Y键表示同意。
  </p>
  <p class="graf graf--p">
   一个名为 images.zip.gpg 的新文件将被创建，这是该压缩文件的加密版本，可以将其作为附件通过电子邮件发送给收件人。然后，他们可以使用他们的私钥解密ZIP文件。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     解密信息
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   您还需要一种方法来解密发给您的信息. 请记住, 为了让别人能够给您发送加密的消息, 您必须先和他们分享您的公共PGP密钥. 您将得到一个加密的文本块，它看起来和加密消息差不多，比如这样：
  </p>
  <pre class="graf graf--pre"><code>-----BEGIN PGP MESSAGE-----</code></pre>
  <pre class="graf graf--pre"><code>hQGMAzCBDnMltq9zAQv/ZHQ3tJq+feazdLa3thzQE2bhPx+7WaPZcX7SdkoyuKvw</code></pre>
  <pre class="graf graf--pre"><code>9faS7h9OwBjQ4vUyDKespSq3ZNf1pRgNoXijjs3MGEi5IsYxDgNWo1ZJv2qQqp36</code></pre>
  <pre class="graf graf--pre"><code>.....</code></pre>
  <pre class="graf graf--pre"><code>-----END PGP MESSAGE-----</code></pre>
  <p class="graf graf--p">
   将此文本块保存到诸如 message.asc 之类的文件中，并在终端中运行以下命令：
  </p>
  <pre class="graf graf--p">gpg -d message.asc &gt; message.txt</pre>
  <p class="graf graf--p">
   系统会提示您输入密码，这个密码与您最初生成PGP密钥对时提供的密码相同。成功输入密码后，将创建一个mail.txt文件，其中包含纯文本的解密信息。这就是全部了!
  </p>
  <p class="graf graf--p">
   恭喜，您的通信现在安全了
  </p>
  <p class="graf graf--p">
   通过本指南，您已经了解了通过PGP加密来保护通信安全的所有必要知识。您已经学会了如何生成PGP密钥对，导出您的公钥以分享给他人，导入他人的公钥，以及如何加密和解密信息。
  </p>
  <p class="graf graf--p">
   现在就可以实践它了。加密愉快。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://www.makeuseof.com/gnupg-encryption-on-linux/" href="https://www.makeuseof.com/gnupg-encryption-on-linux/" rel="noopener" target="_blank">
    How to Use GnuPG for Encryption on Linux
   </a>
  </p>
  <div id="atatags-1611829871-60afb5c0de3ce">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16112" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8linux%e4%b8%8a%e4%bd%bf%e7%94%a8gnupg%e8%bf%9b%e8%a1%8c%e5%8a%a0%e5%af%86/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16112" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e5%9c%a8linux%e4%b8%8a%e4%bd%bf%e7%94%a8gnupg%e8%bf%9b%e8%a1%8c%e5%8a%a0%e5%af%86/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16112-60afb5c0deb2b" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16112&amp;origin=www.iyouport.org&amp;obj_id=161182987-16112-60afb5c0deb2b" id="like-post-wrapper-161182987-16112-60afb5c0deb2b">
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
    <a href="https://www.iyouport.org/tag/linux/" rel="tag">
     Linux
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/security/" rel="tag">
     Security
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/technology/" rel="tag">
     Technology
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-05-26T00:04:11+08:00">
    2021年5月26日
   </time>
   <time class="updated" datetime="2021-02-26T12:23:27+08:00">
    2021年2月26日
   </time>
  </div>
 </div>
</article>

