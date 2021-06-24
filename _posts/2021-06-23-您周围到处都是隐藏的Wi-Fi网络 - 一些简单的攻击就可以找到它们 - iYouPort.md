---
layout: post
title: "您周围到处都是隐藏的Wi-Fi网络 - 一些简单的攻击就可以找到它们 - iYouPort"
date: 2021-06-23T16:04:05+00:00
author: iYouPort
from: https://www.iyouport.org/%e6%82%a8%e5%91%a8%e5%9b%b4%e5%88%b0%e5%a4%84%e9%83%bd%e6%98%af%e9%9a%90%e8%97%8f%e7%9a%84wi-fi%e7%bd%91%e7%bb%9c-%e4%b8%80%e4%ba%9b%e7%ae%80%e5%8d%95%e7%9a%84%e6%94%bb%e5%87%bb%e5%b0%b1%e5%8f%af/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16334 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-54 tag-hacking tag-hidden-wi-fi-networks tag-security tag-technology" id="post-16334">
 <header class="entry-header">
  <h1 class="entry-title">
   您周围到处都是隐藏的Wi-Fi网络 — 一些简单的攻击就可以找到它们
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
   <time class="entry-date published" datetime="2021-06-24T00:04:05+08:00">
    2021年6月24日
   </time>
   <time class="updated" datetime="2021-03-25T19:56:51+08:00">
    2021年3月25日
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
       隐藏网络名并不是真正好的安全做法。因为人们不仅可以看到它的存在，而且还可以轻松地提取名称
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="666" data-image-id="0*hCAvvgQobX28Ap4Z" data-lazy-src="https://cdn-images-1.medium.com/max/1067/0*hCAvvgQobX28Ap4Z?is-pending-load=1" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*hCAvvgQobX28Ap4Z" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="666" data-image-id="0*hCAvvgQobX28Ap4Z" data-width="1000" src="https://cdn-images-1.medium.com/max/1067/0*hCAvvgQobX28Ap4Z"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   在您周围有一些隐藏的Wi-Fi网络 — — 这些网络永远不会显示在您的手机或电脑可以看到的热点列表中  — — 但它们比向任何附近设备广播其名称的常规网络更安全吗？
  </p>
  <p class="graf graf--p">
   简短的答案是否定的，这可能是出于任何原因。
  </p>
  <p class="graf graf--p">
   隐藏的网络实际上与常规的Wi-Fi网络一样；只是它们不会在常规网络发送的信标帧中广播它们的名字(ESSID)。如果不包含名称，您的手机或电脑仅仅通过扫描附近的热点加入就永远也找不到它。要加入一个隐藏的网络，您需要先知道它的名字，有一些攻击可以达到这个目的。
  </p>
  <p class="graf graf--p">
   要发现您所在区域的隐藏Wi-Fi网络，并不需要复杂、疯狂的攻击，几乎任何能在电脑上工作的人都能找到一个。您不需要是黑客、渗透测试专家、网络安全专业人员，或者拥有其他类型花哨网络技能的人。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     发现隐藏网络的方法
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   方法有多种。例如，您可以监视一个曾经连接过隐藏网络的人的手机、电脑或其他设备，因为他们的设备会用纯文本 “喊出” 网络的名称。这是因为设备永远不知道自己什么时候在物理上接近该网络，因为该网络并没有宣布它的存在，所以设备一直在寻找它。
  </p>
  <p class="graf graf--p">
   您也可以对当前连接到隐藏网络的人进行解除身份验证攻击 deauth，然后，当它们试图重新连接到热点的时候，您就可以截获网络名。不管是这种方式还是上面的方式，您都可以使用 airodump 和 Wireshark 来获取名称，您很快就会看到具体做法。
  </p>
  <p class="graf graf--p">
   本文将展示的是另一种方案，用MDK3攻击网络，并通过词典暴力获取名称。要做到这点，您需要有一台电脑，Arduino IDE，Wireshark，以及一个无线网卡或可以进入监控模式的适配器。
  </p>
  <p class="graf graf--p">
   其中一个这样的适配器是 Alfa AWUS036NEH（29.99美元）；其他可能的选择包括 Alfa AWUS036NHA（35.99美元）、TP-Link Nano（14.99美元）、Alfa AWUS036NH（49.99美元）、Panda PAU05（19.99美元）和 Alfa AWUS036ACH（59.99美元）。
  </p>
  <p class="graf graf--p">
   您还需要一个隐藏的网络来进行攻击。一个简单的方法是自己创建一个，很好的方法是使用 D1 Mini 和 Arduino IDE。这里是
   <a class="markup--anchor markup--p-anchor" data-href="https://null-byte.wonderhowto.com/how-to/generate-crackable-wi-fi-handshakes-with-esp8266-based-test-network-0236794/" href="https://null-byte.wonderhowto.com/how-to/generate-crackable-wi-fi-handshakes-with-esp8266-based-test-network-0236794/" rel="noopener" target="_blank">
    相关指南
   </a>
   。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff9900;">
    <strong class="markup--strong markup--p-strong">
     步骤1: 在 D1 Mini 上创建一个隐藏网络（可选）
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   假设您还没有一个隐藏的网络可以猎取，所以首先用D1 Mini 和 Arduino IDE 创建一个网络。
  </p>
  <p class="graf graf--p">
   将 D1 Mini 连接到电脑上，然后在 Arduino IDE 中打开 “WiFiAccessPoint” 示例草图。您可以通过 File -&gt; Examples -&gt; ESP8266WiFi -&gt; WiFiAccessPoint 找到这个草图。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="1082" data-image-id="0*d4p_JBVjSnb0AOn-.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*d4p_JBVjSnb0AOn-.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1370" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*d4p_JBVjSnb0AOn-.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="1082" data-image-id="0*d4p_JBVjSnb0AOn-.jpg" data-recalc-dims="1" data-width="1370" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*d4p_JBVjSnb0AOn-.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   这个草图非常好，只需要进行一点小的修改就可以创建一个隐藏的网络。由于该示例草图用于创建可见的访问点，因此您需要对其进行一些调整。转到脚本中的这一行：
  </p>
  <pre class="graf graf--pre"><code>WiFi.softAP(ssid, password);</code></pre>
  <p class="graf graf--p">
   然后把它改成：
  </p>
  <pre class="graf graf--pre"><code>WiFi.softAP(ssid, password, 1, 1);</code></pre>
  <p class="graf graf--p">
   第一个 “1” 将其设置为通道1，而第二个 “1” 则表示它是一个隐藏网络。完整的草图现在应如下所示：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">/*
   Copyright (c) 2015, Majenko Technologies
   All rights reserved.

   Redistribution and use in source and binary forms, with or without modification,
   are permitted provided that the following conditions are met:

 * * Redistributions of source code must retain the above copyright notice, this
     list of conditions and the following disclaimer.

 * * Redistributions in binary form must reproduce the above copyright notice, this
     list of conditions and the following disclaimer in the documentation and/or
     other materials provided with the distribution.

 * * Neither the name of Majenko Technologies nor the names of its
     contributors may be used to endorse or promote products derived from
     this software without specific prior written permission.

   THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
   ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
   WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
   DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
   ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
   (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
   LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
   ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
   (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
   SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
*/

/* Create a WiFi access point and provide a web server on it. */

#include &lt;ESP8266WiFi.h&gt;
#include &lt;WiFiClient.h&gt;
#include &lt;ESP8266WebServer.h&gt;

#ifndef APSSID
#define APSSID "ESPap"
#define APPSK  "thereisnospoon"
#endif

/* Set these to your desired credentials. */
const char *ssid = APSSID;
const char *password = APPSK;

ESP8266WebServer server(80);

/* Just a little test message.  Go to http://192.168.4.1 in a web browser
   connected to this access point to see it.
*/
void handleRoot() {
  server.send(200, "text/html", "&lt;h1&gt;You are connected&lt;/h1&gt;");
}

void setup() {
  delay(1000);
  Serial.begin(115200);
  Serial.println();
  Serial.print("Configuring access point...");
  /* You can remove the password parameter if you want the AP to be open. */
  WiFi.softAP(ssid, password, 1, 1);

  IPAddress myIP = WiFi.softAPIP();
  Serial.print("AP IP address: ");
  Serial.println(myIP);
  server.on("/", handleRoot);
  server.begin();
  Serial.println("HTTP server started");
}

void loop() {
  server.handleClient();
}</code></pre>
  <p class="graf graf--p">
   现在，点击 “上传” 按钮以编译草图并将其存入 D1 Mini。完成后，您的 D1 Mini 现在应该广播一个隐藏的访问点，其名称为 “ESPap”，密码为 “thereisnospoon”，如示例所示。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff9900;">
    <strong class="markup--strong markup--p-strong">
     步骤2：将设备连接到新的隐藏网络
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   要想看到一个设备猎取隐藏的网络，先用手机或其他设备使用默认名（ESPap）和密码（thereisnospoon）连接到它。然后，将其从网络中断开。将无线适配器置于监控模式，并在通道1上进行快速扫描后，应该能够尝试自动连接设备，稍后还可以进行更多连接。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff9900;">
    <strong class="markup--strong markup--p-strong">
     步骤3：将无线适配器置于监控模式
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   把您的Wi-Fi卡或适配器置于监听模式下，可以让您监听不仅限于电脑的无线流量。不用担心，它只会专注于您查看的内容，因此监听模式对于这种攻击的工作很重要。这里将假设您知道如何做到这一点，如果您还不知道，请查看这里关于启用监听模式的
   <a class="markup--anchor markup--p-anchor" data-href="https://null-byte.wonderhowto.com/how-to/check-if-your-wireless-network-adapter-supports-monitor-mode-packet-injection-0191221/" href="https://null-byte.wonderhowto.com/how-to/check-if-your-wireless-network-adapter-supports-monitor-mode-packet-injection-0191221/" rel="noopener" target="_blank">
    完整指南
   </a>
   。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff9900;">
    <strong class="markup--strong markup--p-strong">
     步骤4：扫描通道1的流量
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   当卡处于监听模式下，现在是时候去看下我们要监听的频道了，在这里是频道1，包括在上面的示例草图。这将极大地缩小您的搜索范围。要做到这一点，只要在终端窗口中使用：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ sudo airodump-ng CARDNAME -c 1

[sudo] password:</code></pre>
  <p class="graf graf--p">
   Airodump 应该开始扫描了，如果您的手机已经打开，并试图找到隐藏的网络，您应该看到它正疯狂地试图连接到该网络。它可能看起来像许多不同的设备，但实际上只是一个设备，它的MAC地址是随机的。
  </p>
  <p class="graf graf--p">
   在实际操作中，您可以用 airodump 开始扫描，等待目标人回家、进入工作状态，或者其他一些场景，他们的设备会自动开始猎取附近他们之前加入的隐藏网络，并连接到它。如果房间里没有其他设备之前连接过隐藏AP，那么目标设备是很明显的，但如果目标设备上保存了很多网络，就会有点棘手。
  </p>
  <p class="graf graf--p">
   找到您的隐藏网络后，复制网络设备的MAC地址，然后关闭手机或禁用手机上的Wi-Fi。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff9900;">
    <strong class="markup--strong markup--p-strong">
     步骤5：打开Wireshark
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   现在是时候开始监听流量了。打开 Wireshark：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ sudo wireshark

[sudo] password:</code></pre>
  <p class="graf graf--p">
   它应该在正确的信道上捕获数据包，但请确保首先选择处于监控模式的同一无线网络适配器。然后，使用下面的过滤器将流量缩小到只有该隐藏网络：
  </p>
  <pre class="graf graf--pre"><code>wlan.ta == HIDDEN-MAC-ADDRESS</code></pre>
  <p class="graf graf--p">
   这个 Wireshark 过滤器应该显示来自该隐藏网络的所有传输。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="310" data-image-id="0*PurBXn1djj4oHQCv.gif" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*PurBXn1djj4oHQCv.gif?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="480" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*PurBXn1djj4oHQCv.gif?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="310" data-image-id="0*PurBXn1djj4oHQCv.gif" data-recalc-dims="1" data-width="480" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*PurBXn1djj4oHQCv.gif?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   在此您应该看到很多详细信息，包括SSID，它应该是一堆零：
  </p>
  <pre class="graf graf--pre"><code>SSID=\000\000\000\000\000</code></pre>
  <p class="graf graf--p">
   所以，即使这个AP没有名字，但它仍然需要传输它连接到的详细细节，只是掩盖了SSID。
  </p>
  <p class="graf graf--p">
   如果您用类似 Wigle WiFi 这样的东西来扫描网络，它同样会记录下来，这就是为什么连MAC地址都会是可以地理定位的东西，以后可以在 Wigle WiFi 这样的服务上找到。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #ff9900;">
    <strong class="markup--strong markup--p-strong">
     步骤6：再次开启手机
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   为了找到这个隐藏网络的名称，把之前连接到该网络的手机或其他设备重新打开，确保设备的Wi-Fi已启用。一旦准备好开始猎取网络，它就会强制探测响应。这基本上是一个包含网络名称的数据包，因为它是必要的，以形成两者将用于连接的密钥。
  </p>
  <p class="graf graf--p">
   然后您应该在 Wireshark 中看到显示SSID名称 “ESPap” 的行。正如您所看到的，没有办法让它完全保密。
  </p>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="309" data-image-id="0*7NORt-luXwd_OwJt.gif" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*7NORt-luXwd_OwJt.gif?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="480" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*7NORt-luXwd_OwJt.gif?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="309" data-image-id="0*7NORt-luXwd_OwJt.gif" data-recalc-dims="1" data-width="480" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*7NORt-luXwd_OwJt.gif?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <h3 class="graf graf--p">
   <span style="color: #ff9900;">
    <strong class="markup--strong markup--p-strong">
     第7步：使用MDK3
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   另一种查找SSID的方法是使用一个叫MDK3的工具，它可以通过暴力攻击来找出网络的名称。要做到这一点，需要一个很好的暴力词表。在此处的测试中只用下面的
   <a class="markup--anchor markup--p-anchor" data-href="https://gist.githubusercontent.com/jgamblin/da795e571fb5f91f9e86a27f2c2f626f/raw/0e5e53b97e372a21cb20513d5064fde11aed844c/commonssids.txt" href="https://gist.githubusercontent.com/jgamblin/da795e571fb5f91f9e86a27f2c2f626f/raw/0e5e53b97e372a21cb20513d5064fde11aed844c/commonssids.txt" rel="noopener" target="_blank">
    “commonssids” 词
   </a>
   表。将其下载到您的桌面上：
  </p>
  <pre class="graf graf--pre"><code>https://gist.githubusercontent.com/jgamblin/da795e571fb5f91f9e86a27f2c2f626f/raw/0e5e53b97e372a21cb20513d5064fde11aed844c/commonssids.txt</code></pre>
  <p class="graf graf--p">
   然后，在新的终端窗口中，可以移至桌面并
   <strong class="markup--strong markup--p-strong">
    cat
   </strong>
   该文件以查看其列出的所有常用网络名称：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ cd Desktop
~$/Desktop$ cat commonssids.txt

ssid
xfinitywifi
linksys
&lt;no ssid&gt;
BTWiFi-with-FON
NETGEAR
Ziggo
dlink
BTWifi-X
default
FreeWifi
hpsetup
UPC Wi-Free
optimumwifi
FreeWifi_secure
AndroidAP
eduroam
BTWIFI
TELENETHOMESPOT
cablewifi
...</code></pre>
  <p class="graf graf--p">
   接下来将使用MDK3迫使设备透露它的网络名称，只要让它做出回应即可。然后，它会尝试将网络与我们的词表中的各种Wi-Fi名称关联起来，看看是否得到了肯定的回应。如果前几次没有成功，就用这种传统的暴力方法。
  </p>
  <p class="graf graf--p">
   使用下面的命令。如果您使用了不同的词表，只需在此处改变 “commonssids” 这个名字。目标(-t)是检测到MAC地址，文件(-f)是词表：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~/Desktop$ sudo mdk3 CARDNAME p -t HIDDEN-MAC-ADDRESS -f commonssids.txt

[sudo] password:</code></pre>
  <p class="graf graf--p">
   现在，在运行命令之前，进入 Wireshark，这样您就可以监控发生了什么。运行词表并监控 Terminal 和 Wireshark 后，您会发现它不起作用，这是因为该词表中实际上没有 “ESPap”。
  </p>
  <p class="graf graf--p">
   您可以使用不同的词表，或者在当前词表中添加新的名称。在这个演示中，只要用下面的命令进入文件，用nano将 “ESPap” 添加到词表中即可。保存并退出。
  </p>
  <pre class="graf graf--pre"><code>~$ nano commonssids.txt</code></pre>
  <p class="graf graf--p">
   然后再次测试暴力破解，看会发生什么：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~/Desktop$ sudo mdk3 CARDNAME p -t HIDDEN-MAC-ADDRESS -f commonssids.txt

[sudo] password:</code></pre>
  <p class="graf graf--p">
   现在您应该看到，它能够正确地猜到网络名称，在不一定有设备连接到它的情况下，暴露之前隐藏的网络。因此，即使没有设备试图连接或被踢掉后试图重新连接，我们也应该能够扫描MAC地址进行暴力攻击。
  </p>
  <p class="graf graf--p">
   一旦知道了网络名，就可以开始对其进行攻击，就像对付一个未被隐藏的网络那样。如果您想保持网络的隐蔽性，隐藏网络名并不是真正好的安全做法。因为人们不仅可以看到它的存在，而且还可以轻松地提取名称。
  </p>
  <h3 class="graf graf--p">
   <span style="color: #339966;">
    <strong class="markup--strong markup--p-strong">
     没有哪个隐藏网络是真正隐藏的
    </strong>
   </span>
  </h3>
  <p class="graf graf--p">
   虽然隐藏Wi-Fi网络可能不会让它出现在附近的人的手机上，但这确实不是一种安全的隐藏网络的方式，也不是让网络更安全的方式。当手机在范围内时，它可以不断地喊出网络的纯文本名称。
  </p>
  <p class="graf graf--p">
   如果您想让您的网络更安全，建议把您的Wi-Fi功率调低，这样它就不会传输得那么远。另外，一定要设置一个非常长且复杂的Wi-Fi密码，而且是独特的，您永远不会在其他地方使用。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://null-byte.wonderhowto.com/how-to/there-are-hidden-wi-fi-networks-all-around-you-these-attacks-will-find-them-0237630/" href="https://null-byte.wonderhowto.com/how-to/there-are-hidden-wi-fi-networks-all-around-you-these-attacks-will-find-them-0237630/" rel="noopener" target="_blank">
    There Are Hidden Wi-Fi Networks All Around You — These Attacks Will Find Them
   </a>
  </p>
  <div id="atatags-1611829871-60d3e2064bf7b">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16334" href="https://www.iyouport.org/%e6%82%a8%e5%91%a8%e5%9b%b4%e5%88%b0%e5%a4%84%e9%83%bd%e6%98%af%e9%9a%90%e8%97%8f%e7%9a%84wi-fi%e7%bd%91%e7%bb%9c-%e4%b8%80%e4%ba%9b%e7%ae%80%e5%8d%95%e7%9a%84%e6%94%bb%e5%87%bb%e5%b0%b1%e5%8f%af/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16334" href="https://www.iyouport.org/%e6%82%a8%e5%91%a8%e5%9b%b4%e5%88%b0%e5%a4%84%e9%83%bd%e6%98%af%e9%9a%90%e8%97%8f%e7%9a%84wi-fi%e7%bd%91%e7%bb%9c-%e4%b8%80%e4%ba%9b%e7%ae%80%e5%8d%95%e7%9a%84%e6%94%bb%e5%87%bb%e5%b0%b1%e5%8f%af/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16334-60d3e2064c55a" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16334&amp;origin=www.iyouport.org&amp;obj_id=161182987-16334-60d3e2064c55a" id="like-post-wrapper-161182987-16334-60d3e2064c55a">
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
    <a href="https://www.iyouport.org/tag/hacking/" rel="tag">
     hacking
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/hidden-wi-fi-networks/" rel="tag">
     hidden Wi-Fi networks
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
   <time class="entry-date published" datetime="2021-06-24T00:04:05+08:00">
    2021年6月24日
   </time>
   <time class="updated" datetime="2021-03-25T19:56:51+08:00">
    2021年3月25日
   </time>
  </div>
 </div>
</article>

