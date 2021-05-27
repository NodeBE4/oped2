---
layout: post
title: "如何使用Python免费创建Discord Bot –完整教程 - iYouPort"
date: 2021-04-05T15:03:58+00:00
author: iYouPort
from: https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8python%e5%85%8d%e8%b4%b9%e5%88%9b%e5%bb%badiscord-bot-%e5%ae%8c%e6%95%b4%e6%95%99%e7%a8%8b/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-15679 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-289 tag-discord-bot tag-python tag-technique" id="post-15679">
 <header class="entry-header">
  <h1 class="entry-title">
   如何使用Python免费创建Discord Bot –完整教程
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
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-04-05T23:03:58+08:00">
    2021年4月5日
   </time>
   <time class="updated" datetime="2021-04-05T23:18:01+08:00">
    2021年4月5日
   </time>
  </span>
  <span class="word-count">
   4 Minutes
  </span>
 </div>
 <div class="entry-content">
  <ul>
   <li class="graf graf--p">
    <span style="color: #00ccff;">
     <em>
      <strong>
       本教程将向您展示如何在云中构建自己的 Discord bot
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="710" data-image-id="0*t1x7tPoB-p48o5w8.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*t1x7tPoB-p48o5w8.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1280" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*t1x7tPoB-p48o5w8.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="710" data-image-id="0*t1x7tPoB-p48o5w8.png" data-recalc-dims="1" data-width="1280" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*t1x7tPoB-p48o5w8.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   您不需要在电脑上安装任何东西，也不需要支付任何费用来托管您的机器人。
  </p>
  <p class="graf graf--p">
   我们将使用一些工具，包括 Discord API、Python 库和一个名为
   <a class="markup--anchor markup--p-anchor" data-href="https://www.repl.it/" href="https://www.repl.it/" rel="noopener" target="_blank">
    Repl.it
   </a>
   的云计算平台。
  </p>
  <p class="graf graf--p">
   这个书面教程还有一个视频版本，在下面，书面版本在视频之后。
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="449" src="//www.youtube.com/embed/SPTfmiYiuok" width="800">
   </iframe>
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何创建 Discord Bot 帐户
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   为了使用 Python 库和 Discord API，我们必须首先创建一个 Discord Bot 帐户。
  </p>
  <p class="graf graf--p">
   以下是创建 Discord Bot 账户的步骤。
  </p>
  <p class="graf graf--p">
   1. 确保您已经登录到
   <a class="markup--anchor markup--p-anchor" data-href="https://discord.com/" href="https://discord.com/" rel="noopener" target="_blank">
    Discord 网站
   </a>
   。
  </p>
  <p class="graf graf--p">
   2. 导航到
   <a class="markup--anchor markup--p-anchor" data-href="https://discord.com/developers/applications" href="https://discord.com/developers/applications" rel="noopener" target="_blank">
    应用页面
   </a>
   。
  </p>
  <p class="graf graf--p">
   3. 点击 “New Application” 按钮。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="494" data-image-id="0*97cOWRKws-beCN6W.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*97cOWRKws-beCN6W.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="702" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*97cOWRKws-beCN6W.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="494" data-image-id="0*97cOWRKws-beCN6W.png" data-recalc-dims="1" data-width="702" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*97cOWRKws-beCN6W.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   4. 给应用命名，然后单击 “创建”。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="780" data-image-id="0*mXhu7OUbODlPl6E8.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*mXhu7OUbODlPl6E8.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="912" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*mXhu7OUbODlPl6E8.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="780" data-image-id="0*mXhu7OUbODlPl6E8.png" data-recalc-dims="1" data-width="912" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*mXhu7OUbODlPl6E8.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   5. 转到 “Bot” 选项卡，然后单击 “Add Bot”。然后确认。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="529" data-image-id="0*I0v-sZlfYVSH6ciW.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*I0v-sZlfYVSH6ciW.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2000" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*I0v-sZlfYVSH6ciW.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="529" data-image-id="0*I0v-sZlfYVSH6ciW.png" data-recalc-dims="1" data-width="2000" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*I0v-sZlfYVSH6ciW.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   保持机器人的默认设置 “Public Bot”（已选中）和 “Require OAuth2 Code Grant”（未选中）。
  </p>
  <p class="graf graf--p">
   您的机器人已经被创建。下一步是复制令牌。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="616" data-image-id="0*rEPZG19k0Qm1Ox1R.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*rEPZG19k0Qm1Ox1R.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1472" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*rEPZG19k0Qm1Ox1R.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="616" data-image-id="0*rEPZG19k0Qm1Ox1R.png" data-recalc-dims="1" data-width="1472" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*rEPZG19k0Qm1Ox1R.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   这个令牌是您的机器人的密码，所以不要与任何人分享它。它可能允许某人登录到您的机器人并做各种坏事。
  </p>
  <p class="graf graf--p">
   如果它不小心被泄漏，您可以重新生成令牌。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何将机器人加入服务器
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在，您必须将Bot用户放入服务器。为此，您应该为其创建邀请URL。
  </p>
  <p class="graf graf--p">
   转到 “OAuth2” 选项。然后在 “scopes” 部分下选择 “bot”。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="727" data-image-id="0*NWXt55Q8acsQ0BQF.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*NWXt55Q8acsQ0BQF.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2600" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*NWXt55Q8acsQ0BQF.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="727" data-image-id="0*NWXt55Q8acsQ0BQF.png" data-recalc-dims="1" data-width="2600" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*NWXt55Q8acsQ0BQF.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   现在，选择您想要的机器人权限。我们的机器人将主要使用短信，因此我们不需要很多权限。您可能需要更多，具体取决于您希望机器人执行的操作。请小心 “管理员” 权限！
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1396" data-image-id="0*s8g4QkgcQrKpO_uJ.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*s8g4QkgcQrKpO_uJ.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2044" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*s8g4QkgcQrKpO_uJ.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1396" data-image-id="0*s8g4QkgcQrKpO_uJ.png" data-recalc-dims="1" data-width="2044" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*s8g4QkgcQrKpO_uJ.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   选择合适的权限后，点击权限上方的 “复制” 按钮。这样就会复制一个URL，可以用来将机器人添加到服务器上。
  </p>
  <p class="graf graf--p">
   将这个URL粘贴到浏览器中，选择一个要邀请机器人的服务器，然后点击 “授权”。
  </p>
  <p class="graf graf--p">
   要添加机器人，您的账户需要有 “管理服务器 “的权限。
  </p>
  <p class="graf graf--p">
   现在您已经创建了机器人用户，我们将开始为机器人编写 Python 代码。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何使用 discord.py 库对基本 Discord Bot 进行编码
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   我们将使用 discord.py Python 库编写该机器人的代码。 discord.py 是 Discord 的API包装器，可以更轻松地在Python中创建 Discord 机器人。
  </p>
  <p class="graf graf--p">
   您可以使用任何代码编辑器在本地计算机上开发机器人。本教程将使用的是 Repl.it，因为它更简单。Repl.it 是一个在线IDE，您可以在浏览器中使用。
  </p>
  <p class="graf graf--p">
   首先进入
   <a class="markup--anchor markup--p-anchor" data-href="https://repl.it/" href="https://repl.it/" rel="noopener" target="_blank">
    Repl.it
   </a>
   。创建一个新的 Repl 并选择 “Python” 作为语言。
  </p>
  <p class="graf graf--p">
   要使用 discord.py 库，只需在 main.py 的顶部写上 import discord。按下 “运行” 按钮时，Repl.it 会自动安装这个依赖项。
  </p>
  <p class="graf graf--p">
   如果您喜欢在本地对机器人进行编码，可以在MacOS上使用这个命令来安装 discord.py：
  </p>
  <pre class="graf graf--p">python3 -m pip install -U discord.py</pre>
  <p class="graf graf--p">
   您可能必须使用 pip3 而不是 pip。
  </p>
  <p class="graf graf--p">
   如果您使用的是 Windows，改为以下命令：
  </p>
  <pre class="graf graf--p">py -3 -m pip install -U discord.py</pre>
  <p class="graf graf--p">
   discord.py 围绕事件的概念展开。事件是指您所听到的，然后对其进行响应。例如，当一个消息发生时，您会收到一个关于它的事件，您可以对其进行回复。
  </p>
  <p class="graf graf--p">
   让我们做一个机器人，它可以回复特定的消息。这个简单的机器人代码以及代码说明取自
   <a class="markup--anchor markup--p-anchor" data-href="https://discordpy.readthedocs.io/en/latest/quickstart.html#a-minimal-bot" href="https://discordpy.readthedocs.io/en/latest/quickstart.html#a-minimal-bot" rel="noopener" target="_blank">
    the discord.py documentation
   </a>
   。稍后我们将为机器人添加更多的功能。
  </p>
  <p class="graf graf--p">
   将这段代码添加到 main.py 中。(如果你喜欢的话，可以给这个文件起个其他名字，但不要用 discord.py)：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">import discord
import os

client = discord.Client()

@client.event
async def on_ready():
    print('We have logged in as {0.user}'.format(client))

@client.event
async def on_message(message):
    if message.author == client.user:
        return

    if message.content.startswith('$hello'):
        await message.channel.send('Hello!')

client.run(os.getenv('TOKEN'))</code></pre>
  <p class="graf graf--p">
   刚才在 Discord 上创建机器人用户时，您复制了一个令牌。现在我们要创建一个 .env 文件来存储这个令牌。如果您在本地运行代码，就不需要 .env文件，只要把 os.getenv(‘TOKEN’) 换成这个令牌就行了。
  </p>
  <p class="graf graf--p">
   .env 文件是用来声明环境变量的。在 Repl.it 上，您创建的大多数文件对任何人都是可见的，但 .env 文件只对您自己可见。 其他查看公共repl的人将无法看到.env文件的内容。
  </p>
  <p class="graf graf--p">
   所以，如果您在 Repl.it 上进行开发，请只在 .env 文件中包含令牌或密钥等私人信息。
  </p>
  <p class="graf graf--p">
   点击 “添加文件” 按钮，创建一个名为.env 的文件。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="284" data-image-id="0*bk_K7xD-tX8_MQF_.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*bk_K7xD-tX8_MQF_.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="934" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*bk_K7xD-tX8_MQF_.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="284" data-image-id="0*bk_K7xD-tX8_MQF_.png" data-recalc-dims="1" data-width="934" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*bk_K7xD-tX8_MQF_.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   在文件内添加以下行，包括您先前复制的实际令牌：
  </p>
  <pre class="graf graf--pre"><code>TOKEN=[paste token here]</code></pre>
  <p class="graf graf--p">
   来看看每行代码的作用。
  </p>
  <p class="graf graf--p">
   1、第一行导入 discord.py 库。
  </p>
  <p class="graf graf--p">
   2、第二行导入 os 库，但这只是用来从 .env 文件中获取 TOKEN 变量。如果您没有使用.env文件就不需要这一行。
  </p>
  <p class="graf graf--p">
   3、接下来，创建一个Client，这是与 Discord 的连接。
  </p>
  <p class="graf graf--p">
   4、@client.event() 装饰器用于注册一个事件。这是一个异步库，所以要通过回调来完成。回调是指当其他事情发生时被调用的函数。在这段代码中，当机器人准备好时就会调用 on_ready() 事件。然后，当机器人收到消息时，就会调用 on_message() 事件。
  </p>
  <p class="graf graf--p">
   5、on_message() 事件在每次收到消息时都会触发，但如果消息是来自您自己，您就不希望它做任何事。所以如果 Message.author 等于 Client.user，代码就会返回。
  </p>
  <p class="graf graf--p">
   6、接下来检查 Message.content 是否以 ‘$hello’ 开头。如果是，那么机器人就会用 ‘Hello！’来回复。
  </p>
  <p class="graf graf--p">
   7、现在机器人已经设置好了，最后一行使用登录令牌运行机器人。它从 .env 文件中获取令牌。
  </p>
  <p class="graf graf--p">
   现在运行它就可以了。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何运行这个机器人
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在，单击顶部的运行按钮以在 repl.it 中运行您的机器人。
  </p>
  <p class="graf graf--p">
   如果您是在本地编写机器人，可以在终端中使用以下命令来运行机器人。
  </p>
  <p class="graf graf--p">
   在 Windows 上：
  </p>
  <pre class="graf graf--p">py -3 main.py</pre>
  <p class="graf graf--p">
   在其他系统上：
  </p>
  <pre class="graf graf--p">python3 main.py</pre>
  <p class="graf graf--p">
   现在转到您的Discord房间，然后键入“ $ hello”。您的机器人应返回 “ Hello！”。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="248" data-image-id="0*C8UEL-3cLJW7mv3l.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*C8UEL-3cLJW7mv3l.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="620" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*C8UEL-3cLJW7mv3l.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="248" data-image-id="0*C8UEL-3cLJW7mv3l.png" data-recalc-dims="1" data-width="620" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*C8UEL-3cLJW7mv3l.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何改善机器人
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在您已经有了一个最基本的机器人，您需要改进它。它被称为 “鼓励机器人” 是有原因的。
  </p>
  <p class="graf graf--p">
   每当有人发送包含悲伤或压抑字眼的消息时，这个机器人就会回复一条鼓励的消息。
  </p>
  <p class="graf graf--p">
   任何人都可以添加鼓励信息供机器人使用，用户提交的信息将被存储在 Repl.it 数据库中。
  </p>
  <p class="graf graf--p">
   当有人在聊天中输入消息 “$inspire” 时，这个机器人也会从API中随机返回一句励志的话。
  </p>
  <p class="graf graf--p">
   我们将从添加 “$inspire” 功能开始。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何在机器人中添加励志名言
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   我们将从一个名为 zenquotes.io 的API中获取励志名言。需要再导入几个 Python 模块，添加一个 get_quote() 函数，更新机器人代码来调用该函数。
  </p>
  <p class="graf graf--p">
   下面是更新后的代码。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">import discord
import os
import requests
import json

client = discord.Client()

def get_quote():
  response = requests.get("https://zenquotes.io/api/random")
  json_data = json.loads(response.text)
  quote = json_data[0]['q'] + " -" + json_data[0]['a']
  return(quote)

@client.event
async def on_ready():
  print('We have logged in as {0.user}'.format(client))

@client.event
async def on_message(message):
  if message.author == client.user:
    return

  if message.content.startswith('$inspire'):
    quote = get_quote()
    await message.channel.send(quote)

client.run(os.getenv('TOKEN'))</code></pre>
  <p class="graf graf--p">
   现在要导入 requests 模块。这个模块允许代码进行HTTP请求从API中获取数据。API返回的是JSON，所以json模块可以更容易处理返回的数据。
  </p>
  <p class="graf graf--p">
   get_quote() 函数非常简单。首先，它使用 requests 模块从 API URL 中请求数据。API返回一个随机的励志名言。如果当前的API停止工作，这个函数可以很容易地重写成从不同的API获取名言。
  </p>
  <p class="graf graf--p">
   接下来使用 json.load() 将API的响应转换为JSON。励志名言从该函数中以字符串的形式返回。
  </p>
  <p class="graf graf--p">
   最后的更新部分在结尾处。之前它寻找的是以 “$hello” 开头的消息，现在它寻找的是 “$inspire”。它不是返回 “Hello!”，而是用 quote = get_quote() 获取一个励志名言，并返回这句名言。
  </p>
  <p class="graf graf--p">
   此时，您可以运行您的代码尝试一下。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何向机器人添加励志消息
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在我们将实现该功能，当用户发布带有悲伤字眼的消息时，机器人会通过励志消息来响应。
  </p>
  <p class="graf graf--p">
   首先需要创建一个 Python 列表，其中包含机器人将响应的悲伤字眼。
  </p>
  <p class="graf graf--p">
   创建 client 变量后，添加以下行：
  </p>
  <pre class="graf graf--p">sad_words = [“sad”, “depressed”, “unhappy”, “angry”, “miserable”]</pre>
  <p class="graf graf--p">
   您可以随时在该列表中添加更多单词。
  </p>
  <p class="graf graf--p">
   现在将添加一个鼓励机器人响应的励志消息列表。 在您创建的 sad_words 列表之后添加以下列表：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">starter_encouragements = [
  "Cheer up!",
  "Hang in there.",
  "You are a great person / bot!"
]</code></pre>
  <p class="graf graf--p">
   像以前一样，您可以随意在这个列表中添加更多您选择的短语。我现在只用了三个，因为稍后会增加更多功能。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何响应消息
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在我们需要更新这个机器人来使用我们创建的两个列表。首先，导入随机模块，因为机器人会随机选择励志信息。在代码顶部添加以下一行：import random。
  </p>
  <p class="graf graf--p">
   现在将更新 on_message() 函数，检查所有消息是否包含 sad_words 列表中的单词。如果发现一个悲伤的单词，机器人将随机发送一条鼓励的消息。
  </p>
  <p class="graf graf--p">
   下面是更新后的代码。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">async def on_message(message):
  if message.author == client.user:
    return

  msg = message.content

  if msg.startswith('$inspire'):
    quote = get_quote()
    await message.channel.send(quote)
    
  if any(word in msg for word in sad_words):
    await message.channel.send(random.choice(starter_encouragements))</code></pre>
  <p class="graf graf--p">
   这是测试机器人的好时机。您现在已经足够了解如何创建自己的机器人了，接下来您将学习如何使用 Repl.it 数据库实现更多高级功能并存储数据。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何启用用户提交的消息
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在我们可以通过Discord更新这个机器人。用户应该能够为机器人添加更多的励志信息，让它在检测到一个悲伤的词时可以使用。
  </p>
  <p class="graf graf--p">
   我们将使用 Repl.it 的内置数据库来存储用户提交的消息。这个数据库是每个repl.it内置的键值存储。
  </p>
  <p class="graf graf--p">
   在代码的顶部，在其他导入语句下，添加 from replit import db。这将允许您使用 Repl.it 数据库。
  </p>
  <p class="graf graf--p">
   用户将可以直接从 Discord 聊天中为机器人添加自定义的鼓励信息。在为机器人添加新命令之前，先创建两个辅助函数，以将自定义消息添加到数据库并删除它们。
  </p>
  <p class="graf graf--p">
   在 get_quote() 函数后添加以下代码。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">def update_encouragements(encouraging_message):
  if "encouragements" in db.keys():
    encouragements = db["encouragements"]
    encouragements.append(encouraging_message)
    db["encouragements"] = encouragements
  else:
    db["encouragements"] = [encouraging_message]

def delete_encouragment(index):
  encouragements = db["encouragements"]
  if len(encouragements) &gt; index:
    del encouragements[index]
  db["encouragements"] = encouragements</code></pre>
  <p class="graf graf--p">
   update_encouragements() 函数接受一个鼓励性信息作为参数。
  </p>
  <p class="graf graf--p">
   首先它检查 “encouragements” 是否是数据库中的一个键。如果是，它就会得到数据库中已有的鼓励性信息列表，将新的鼓励性信息添加到列表中，并将更新后的列表存储到数据库中。
  </p>
  <p class="graf graf--p">
   如果数据库中还没有 “encouragements” 键，则创建一个新的键，并将新的鼓励信息作为该列表中的第一个元素添加进去。
  </p>
  <p class="graf graf--p">
   delete_encouragement() 函数接受一个索引作为参数。它从数据库中获取存储在 “鼓励” 键下的鼓励性信息列表。如果鼓励性信息列表中的项目数量大于索引，那么该索引处的列表项就会被删除。
  </p>
  <p class="graf graf--p">
   最后，更新后的列表会被存储回数据库中。
  </p>
  <p class="graf graf--p">
   下面是 on_message() 函数的更新代码。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">async def on_message(message):
  if message.author == client.user:
    return

  msg = message.content
 
  if msg.startswith("$inspire"):
    quote = get_quote()
    await message.channel.send(quote)

  options = starter_encouragements
  if "encouragements" in db.keys():
    options = options + db["encouragements"]

  if any(word in msg for word in sad_words):
    await message.channel.send(random.choice(options))

  if msg.startswith("$new"):
    encouraging_message = msg.split("$new ",1)[1]
    update_encouragements(encouraging_message)
    await message.channel.send("New encouraging message added.")

  if msg.startswith("$del"):
    encouragements = []
    if "encouragements" in db.keys():
      index = int(msg.split("$del",1)[1])
      delete_encouragment(index)
      encouragements = db["encouragements"]
    await message.channel.send(encouragements)</code></pre>
  <p class="graf graf--p">
   上面的第一行新代码是 options = starter_encouragements。之所以要复制 starter_encouragements，是因为要在为机器人选择随机消息发送之前，将用户提交的消息添加到该列表中。
  </p>
  <p class="graf graf--p">
   我们检查 “encouragement” 是否已经在数据库中（意味着用户至少提交了一条自定义消息）。如果是，就将用户消息添加到鼓励列表中。
  </p>
  <p class="graf graf--p">
   然后，机器人现在不是从 starter_encouragements 中随机发送消息，而是从 options 中随机发送消息。
  </p>
  <p class="graf graf--p">
   下面的代码用于将用户提交的新消息添加到数据库中。如果一条 Discord 消息以 “$new” 开头，那么 “$new” 之后的文本将被用作新的鼓励性消息。
  </p>
  <p class="graf graf--p">
   msg.split(“$new ”,1)[1] 将消息从 “$new” 命令中分离出来，并将消息存储在一个变量中。请注意 “$new ” 中的空格，我们需要空格后的所有内容。
  </p>
  <p class="graf graf--p">
   用新消息调用 update_encouragements 助手函数，然后机器人会向 discord 聊天室发送一条消息，确认消息已被添加。
  </p>
  <p class="graf graf--p">
   第三个新的部分（在上面代码的最后）检查新的Discord消息是否以 “$del” 开头。这是删除数据库中 “鼓励” 列表中某项的命令。
  </p>
  <p class="graf graf--p">
   首先，一个名为 encouragements 的新变量被初始化为一个空数组。这样做的原因是，如果数据库中没有包含 “鼓励” 键，这部分代码将以一个空数组发送消息。
  </p>
  <p class="graf graf--p">
   如果 “鼓励” 键在数据库中，那么索引将从 Discord 消息中以 “$del” 开头分割出来。然后，调用 delete_encouragement() 函数，传递要删除的索引。更新后的鼓励列表会被加载到鼓励变量中，然后机器人会向Discord发送一条包含当前列表的消息。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     最后添加功能
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   机器人应该可以工作了，所以现在是测试它的好时机。现在我们将添加一些最后的功能。
  </p>
  <p class="graf graf--p">
   将添加从Discord直接获取用户提交的消息列表的能力，还将添加关闭和开启机器人是否对悲伤的对话做出回应的能力。
  </p>
  <p class="graf graf--p">
   下面是完整程序的最终代码。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">import discord
import os
import requests
import json
import random
from replit import db

client = discord.Client()

sad_words = ["sad", "depressed", "unhappy", "angry", "miserable"]

starter_encouragements = [
  "Cheer up!",
  "Hang in there.",
  "You are a great person / bot!"
]

if "responding" not in db.keys():
  db["responding"] = True

def get_quote():
  response = requests.get("https://zenquotes.io/api/random")
  json_data = json.loads(response.text)
  quote = json_data[0]["q"] + " -" + json_data[0]["a"]
  return(quote)

def update_encouragements(encouraging_message):
  if "encouragements" in db.keys():
    encouragements = db["encouragements"]
    encouragements.append(encouraging_message)
    db["encouragements"] = encouragements
  else:
    db["encouragements"] = [encouraging_message]

def delete_encouragment(index):
  encouragements = db["encouragements"]
  if len(encouragements) &gt; index:
    del encouragements[index]
  db["encouragements"] = encouragements

@client.event
async def on_ready():
  print("We have logged in as {0.user}".format(client))

@client.event
async def on_message(message):
  if message.author == client.user:
    return

  msg = message.content

  if msg.startswith("$inspire"):
    quote = get_quote()
    await message.channel.send(quote)

  if db["responding"]:
    options = starter_encouragements
    if "encouragements" in db.keys():
      options = options + db["encouragements"]

    if any(word in msg for word in sad_words):
      await message.channel.send(random.choice(options))

  if msg.startswith("$new"):
    encouraging_message = msg.split("$new ",1)[1]
    update_encouragements(encouraging_message)
    await message.channel.send("New encouraging message added.")

  if msg.startswith("$del"):
    encouragements = []
    if "encouragements" in db.keys():
      index = int(msg.split("$del",1)[1])
      delete_encouragment(index)
      encouragements = db["encouragements"]
    await message.channel.send(encouragements)

  if msg.startswith("$list"):
    encouragements = []
    if "encouragements" in db.keys():
      encouragements = db["encouragements"]
    await message.channel.send(encouragements)
    
  if msg.startswith("$responding"):
    value = msg.split("$responding ",1)[1]

    if value.lower() == "true":
      db["responding"] = True
      await message.channel.send("Responding is on.")
    else:
      db["responding"] = False
      await message.channel.send("Responding is off.")

client.run(os.getenv("TOKEN"))</code></pre>
  <p class="graf graf--p">
   添加到代码的第一部分就在 starter_encouragements 列表下面：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">if "responding" not in db.keys():
  db["responding"] = True</code></pre>
  <p class="graf graf--p">
   在数据库中创建一个名为 “回应” 的新键，并将其设置为 “True”，将用它来决定机器人是否应该对悲伤的词语做出回应。
  </p>
  <p class="graf graf--p">
   下一个新的部分是，响应悲伤的话的部分现在在这个 if 语句里面：if db[“responseing”]:。只有在 db[“responseing”]=True 的情况下，机器人才会响应悲伤的话。
  </p>
  <p class="graf graf--p">
   接下来，在让机器人响应 “$del” 命令的代码之后，有新的代码来响应作为Discord消息发送的 “$list” 命令。
  </p>
  <p class="graf graf--p">
   本节首先创建一个名为鼓励的空列表，然后如果数据库中已经有了鼓励，这些鼓励就会替换刚刚创建的空列表。
  </p>
  <p class="graf graf--p">
   最后，机器人将鼓励列表作为 Discord 消息发送。
  </p>
  <p class="graf graf--p">
   接下来是最后一个新的部分。这段代码让机器人响应 “$responding” 命令。这个命令的参数为 “true” 或 “false”。下面是一个使用示例: “$responding true”.
  </p>
  <p class="graf graf--p">
   代码是 value = msg.split(“$responding ”,1)[1] （和之前一样，注意 “$responding ” 中的空格）。然后是一个 if/else 语句，适当地设置数据库中的 “responding”，并向 Discord 发送一个通知消息。如果参数不是 “true”，代码就会假设为 “false”。
  </p>
  <p class="graf graf--p">
   机器人的代码就完成了。现在您可以运行机器人并试用它。但还有一个重要的步骤，下面讨论。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何将机器人设置为连续运行
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   如果您在 repl.it 中运行机器人，然后关闭正在运行的标签页，您的机器人将停止运行。
  </p>
  <p class="graf graf--p">
   为了让机器人持续运行，我们将使用另一个免费服务，名为 Uptime Robot，网址为
   <a class="markup--anchor markup--p-anchor" data-href="https://uptimerobot.com/" href="https://uptimerobot.com/" rel="nofollow noopener" target="_blank">
    https://uptimerobot.com/
   </a>
   。
  </p>
  <p class="graf graf--p">
   Uptime Robot 可以被设置为每5分钟ping一次 repl.it上的机器人的web服务器。通过不断的ping，机器人永远不会进入睡眠阶段。
  </p>
  <p class="graf graf--p">
   所以我们还要做两件事来让机器人持续运行：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    在 repl.it上创建一个web服务器
   </li>
   <li class="graf graf--li">
    设置 Uptime Robot 持续 ping 这个服务器
   </li>
  </ul>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何在 repl.it 中创建Web服务器
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   很简单，只需要在您的项目中创建一个名为 keep_alive.py 的新文件。
  </p>
  <p class="graf graf--p">
   然后添加以下代码：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">from flask import Flask
from threading import Thread

app = Flask('')

@app.route('/')
def home():
    return "Hello. I am alive!"

def run():
  app.run(host='0.0.0.0',port=8080)

def keep_alive():
    t = Thread(target=run)
    t.start()</code></pre>
  <p class="graf graf--p">
   在这段代码中，我们使用 Flask 来启动一个Web服务器。服务器会向访问它的人返回 “你好。我还活着。” 服务器将在一个独立的线程上运行，与机器人无关。
  </p>
  <p class="graf graf--p">
   现在我们只需要机器人来运行这个web服务器。
  </p>
  <p class="graf graf--p">
   在 main.py 的顶部添加以下一行来导入服务器：
  </p>
  <pre class="graf graf--pre"><code>from keep_alive import keep_alive</code></pre>
  <p class="graf graf--p">
   要在运行 main.py 时启动Web服务器，请将以下行作为倒数第二行添加，就在机器人运行之前：
  </p>
  <pre class="graf graf--p">keep_alive()</pre>
  <p class="graf graf--p">
   添加此代码后，在 repl.it 上运行机器人时，将打开一个新的Web服务器窗口。显示了Web服务器的URL。复制该URL，以便您可以在下一部分中使用它。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="407" data-image-id="0*t9coZ0AV1I5EHXvO.png" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*t9coZ0AV1I5EHXvO.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="2000" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*t9coZ0AV1I5EHXvO.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="407" data-image-id="0*t9coZ0AV1I5EHXvO.png" data-recalc-dims="1" data-width="2000" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*t9coZ0AV1I5EHXvO.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     如何设置Uptime Robot
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在我们需要设置 Uptime Robot 以每五分钟ping一次Web服务器，这将导致机器人不断运行。
  </p>
  <p class="graf graf--p">
   在
   <a class="markup--anchor markup--p-anchor" data-href="https://uptimerobot.com/" href="https://uptimerobot.com/" rel="noopener" target="_blank">
    https://uptimerobot.com/
   </a>
   上创建一个免费帐户。
  </p>
  <p class="graf graf--p">
   登录到帐户后，单击 “Add New Monitor”。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="290" data-image-id="0*hkx03tE4poduHgz8.png" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*hkx03tE4poduHgz8.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1116" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*hkx03tE4poduHgz8.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="290" data-image-id="0*hkx03tE4poduHgz8.png" data-recalc-dims="1" data-width="1116" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*hkx03tE4poduHgz8.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   请选择 “ HTTP（s）” 作为监视器类型，可将其命名为任意名称。然后，从 repl.it 粘贴Web服务器的URL。最后，单击 “Create Monitor”。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1376" data-image-id="0*kcy3WVcirflTQwGO.png" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*kcy3WVcirflTQwGO.png?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1660" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*kcy3WVcirflTQwGO.png?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1376" data-image-id="0*kcy3WVcirflTQwGO.png" data-recalc-dims="1" data-width="1660" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*kcy3WVcirflTQwGO.png?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   大功告成！现在，该机器人将连续运行，以便人们可以始终在 Repl.it 上与它进行交互。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     最后
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   discord.py 库还可以做很多其他事。因此，如果您想为 Discord 机器人提供更多功能，那么下一步就是查看
   <a class="markup--anchor markup--p-anchor" data-href="https://discordpy.readthedocs.io/en/latest/index.html" href="https://discordpy.readthedocs.io/en/latest/index.html" rel="noopener" target="_blank">
    这里的文档
   </a>
   。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://www.freecodecamp.org/news/create-a-discord-bot-with-python/" href="https://www.freecodecamp.org/news/create-a-discord-bot-with-python/" rel="noopener" target="_blank">
    How to Create a Discord Bot for Free with Python — Full Tutorial
   </a>
  </p>
  <div id="atatags-1611829871-60afa1602821c">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-15679" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8python%e5%85%8d%e8%b4%b9%e5%88%9b%e5%bb%badiscord-bot-%e5%ae%8c%e6%95%b4%e6%95%99%e7%a8%8b/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-15679" href="https://www.iyouport.org/%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8python%e5%85%8d%e8%b4%b9%e5%88%9b%e5%bb%badiscord-bot-%e5%ae%8c%e6%95%b4%e6%95%99%e7%a8%8b/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-15679-60afa16028c0b" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=15679&amp;origin=www.iyouport.org&amp;obj_id=161182987-15679-60afa16028c0b" id="like-post-wrapper-161182987-15679-60afa16028c0b">
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
    <a href="https://www.iyouport.org/tag/discord-bot/" rel="tag">
     Discord Bot
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/python/" rel="tag">
     Python
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
   <time class="entry-date published" datetime="2021-04-05T23:03:58+08:00">
    2021年4月5日
   </time>
   <time class="updated" datetime="2021-04-05T23:18:01+08:00">
    2021年4月5日
   </time>
  </div>
 </div>
</article>

