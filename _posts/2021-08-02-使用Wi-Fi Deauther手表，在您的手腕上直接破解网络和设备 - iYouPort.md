---
layout: post
title: "使用Wi-Fi Deauther手表，在您的手腕上直接破解网络和设备 - iYouPort"
date: 2021-08-02T16:04:15+00:00
author: iYouPort
from: https://www.iyouport.org/%e4%bd%bf%e7%94%a8wi-fi-deauther%e6%89%8b%e8%a1%a8%ef%bc%8c%e5%9c%a8%e6%82%a8%e7%9a%84%e6%89%8b%e8%85%95%e4%b8%8a%e7%9b%b4%e6%8e%a5%e7%a0%b4%e8%a7%a3%e7%bd%91%e7%bb%9c%e5%92%8c%e8%ae%be%e5%a4%87/
tags: [ iYouPort ]
categories: [ iYouPort ]
---

<article class="post-16846 post type-post status-publish format-standard has-post-thumbnail hentry category-knowledge-node category-289 category-67 tag-deauther-watch tag-hacking tag-hacktivist tag-technology tag-wi-fi-hacking" id="post-16846">
 <header class="entry-header">
  <h1 class="entry-title">
   使用Wi-Fi Deauther手表，在您的手腕上直接破解网络和设备
  </h1>
 </header>
 <div class="entry-meta">
  <span class="byline">
   <a href="https://www.iyouport.org/author/gabrielfornard/" rel="author" title="文章作者 Gabriel Fornard">
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
   <a href="https://www.iyouport.org/category/%e7%bb%99%e8%a1%8c%e5%8a%a8%e8%80%85%e7%9a%84%e6%8a%a4%e8%ba%ab%e7%ac%a6%e5%92%8c%e6%ad%a6%e5%99%a8/" rel="category tag">
    给行动者的护身符和武器
   </a>
  </span>
  <span class="published-on">
   <time class="entry-date published" datetime="2021-08-03T00:04:15+08:00">
    2021年8月3日
   </time>
   <time class="updated" datetime="2021-05-24T15:43:05+08:00">
    2021年5月24日
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
       针对联网摄像头可能是最有趣的玩法，但是！绝对不是在建议您这样做！如果您的当地法律禁止未经授权的干扰网络连接，您需要警惕触犯法律
      </strong>
     </em>
    </span>
   </li>
  </ul>
  <figure class="graf graf--figure">
   <img class="graf-image aligncenter jetpack-lazy-image" data-height="720" data-image-id="0*vwiGhOoy2IrsKPSl.jpg" data-lazy-src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vwiGhOoy2IrsKPSl.jpg?w=1100&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1280" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vwiGhOoy2IrsKPSl.jpg?w=1100&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"/>
   <noscript>
    <img class="graf-image aligncenter" data-height="720" data-image-id="0*vwiGhOoy2IrsKPSl.jpg" data-recalc-dims="1" data-width="1280" src="https://i0.wp.com/cdn-images-1.medium.com/max/1067/0*vwiGhOoy2IrsKPSl.jpg?w=1100&amp;ssl=1"/>
   </noscript>
  </figure>
  <p class="graf graf--p">
   Travis Lin 的 Deauther 手表是德国黑客 Spacehuhn 的 Wi-Fi Deauther 项目的物理表现，它的设计是为了让您从手腕上直接操作Deauther而不需要电脑。如果您想做 Wi-Fi Deauther 能做的所有有趣的事，而不需要把它插入一个设备，那么您会知道，这种方法是最酷的。
  </p>
  <p class="graf graf--p">
   关于 Deauther，首先，它可以创建取消认证和取消关联程序包，这可以将目标设备从Deauther攻击的同一Wi-Fi网络中踢出去。它可以一次又一次地这样做，不断干扰网络，使设备无法连接或保持连接。
  </p>
  <p class="graf graf--p">
   Wi-Fi监视摄像头是这种类型的攻击的一个有趣的用例。您可以使用 Deauther Watch 的可穿戴黑客工具，然后寻找您遇到的监视摄像头所连接的Wi-Fi网络，然后发出一个deauth攻击，将目标摄像头踢出网络，这样您就可以神不知鬼不觉地溜走了。
  </p>
  <p class="graf graf--p">
   Wi-Fi Deauther 项目可以扫描附近的接入点和连接的设备，它甚至可以克隆它看到的任何Wi-Fi网络。它还可以用您想要的任何名字生成几十个假的Wi-Fi网络，监测设备之间的数据包流量通道，并在一个漂亮的内置界面上完成所有这些工作。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    您将需要什么？
   </strong>
  </h3>
  <p class="graf graf--p">
   现在，如果您想单独购买所有部件，您实际上可以自己建造一个 Deauther Watch，您也可以从下面挑选一个包含所有部件的预装版：
  </p>
  <ul class="postList">
   <li class="graf graf--li">
    Amazon:
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.de/KKmoon-Deauther-Programmable-Development-Watchband/dp/B089ZZ3JN8/?tag=wnbde-21&amp;language=en_GB" href="https://www.amazon.de/KKmoon-Deauther-Programmable-Development-Watchband/dp/B089ZZ3JN8/?tag=wnbde-21&amp;language=en_GB" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v1
    </a>
   </li>
   <li class="graf graf--li">
    Amazon:
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.de/MakerFocus-Deauther-Programmable-Development-Wristband/dp/B088LPLN9V/?tag=wnbde-21&amp;language=en_GB" href="https://www.amazon.de/MakerFocus-Deauther-Programmable-Development-Wristband/dp/B088LPLN9V/?tag=wnbde-21&amp;language=en_GB" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v2
    </a>
   </li>
   <li class="graf graf--li">
    Amazon:
    <a class="markup--anchor markup--li-anchor" data-href="https://www.amazon.de/MakerFocus-ESP8266-Deauther-Detector-Pre-flashed/dp/B08DHNJ266/?tag=wnbde-21&amp;language=en_GB" href="https://www.amazon.de/MakerFocus-ESP8266-Deauther-Detector-Pre-flashed/dp/B08DHNJ266/?tag=wnbde-21&amp;language=en_GB" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v3
    </a>
   </li>
   <li class="graf graf--li">
    DSTIKE:
    <a class="markup--anchor markup--li-anchor" data-href="https://dstike.com/products/dstike-deauther-watch-v1" href="https://dstike.com/products/dstike-deauther-watch-v1" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v1
    </a>
   </li>
   <li class="graf graf--li">
    DSTIKE:
    <a class="markup--anchor markup--li-anchor" data-href="https://dstike.com/products/dstike-deauther-watch-v2" href="https://dstike.com/products/dstike-deauther-watch-v2" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v2
    </a>
   </li>
   <li class="graf graf--li">
    DSTIKE:
    <a class="markup--anchor markup--li-anchor" data-href="https://dstike.com/collections/frontpage/products/dstike-deauther-watch-v3" href="https://dstike.com/collections/frontpage/products/dstike-deauther-watch-v3" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v3
    </a>
   </li>
   <li class="graf graf--li">
    Aliexpress:
    <a class="markup--anchor markup--li-anchor" data-href="https://www.aliexpress.com/item/1005002147702348.html" href="https://www.aliexpress.com/item/1005002147702348.html" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v1
    </a>
   </li>
   <li class="graf graf--li">
    Aliexpress:
    <a class="markup--anchor markup--li-anchor" data-href="https://www.aliexpress.com/item/4000522565001.html" href="https://www.aliexpress.com/item/4000522565001.html" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v2
    </a>
   </li>
   <li class="graf graf--li">
    Aliexpress:
    <a class="markup--anchor markup--li-anchor" data-href="https://www.aliexpress.com/item/1005002142572106.html" href="https://www.aliexpress.com/item/1005002142572106.html" rel="nofollow noopener" target="_blank">
     DSTIKE Deauther Watch v3
    </a>
   </li>
  </ul>
  <p class="graf graf--p">
   如果您需要从头开始安装固件，则还需要Python 3。
  </p>
  <p class="graf graf--p">
   <iframe allowfullscreen="allowfullscreen" height="449" loading="lazy" src="//www.youtube.com/embed/H0kRS5zR3-w" width="800">
   </iframe>
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤1：从头开始刷新固件（如有必要）
   </strong>
  </h3>
  <p class="graf graf--p">
   Deauther Watch 应该预先刷上了正确的固件，但如果缺少软件、软件损坏、或有什么地方不对，您随时可以安装或重新安装它。在任何这些情况下，请确保您安装了esptool：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ pip3 install esptool

Collecting esptool
  Downloading https://files.pythonhosted.org/packages/68/91/08c182f66fa3f12a96e754ae8ec7762abb2d778429834638f5746f81977a/esptool-2.8.tar.gz (84kB)
    100% |████████████████████████████████| 92kB 928kB/s
Requirement already satisfied: ecdsa in /usr/lib/python3/dist-packages (from esptool) (0.13)
Collecting pyaes (from esptool)
  Downloading https://files.pythonhosted.org/packages/44/66/2c17bae31c906613795711fc78045c285048168919ace2220daa372c7d72/pyaes-1.6.1.tar.gz
Requirement already satisfied: pyserial&gt;=3.0 in /usr/lib/python3/dist-packages (from esptool) (3.4)
Building wheels for collected packages: esptool, pyaes
  Running setup.py bdist_wheel for esptool ... done
  Stored in directory: /root/.cache/pip/wheels/56/9e/fd/06e784bf9c77e9278297536f3df36a46941c885eb23593bb16
  Running setup.py bdist_wheel for pyaes ... done
  Stored in directory: /root/.cache/pip/wheels/bd/cf/7b/ced9e8f28c50ed666728e8ab178ffedeb9d06f6a10f85d6432
Successfully built esptool pyaes
Installing collected packages: pyaes, esptool
Successfully installed esptool-2.8 pyaes-1.6.1</code></pre>
  <p class="graf graf--p">
   接下来，去 GitHub 上 Spacehuhn 的
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/SpacehuhnTech/esp8266_deauther" href="https://github.com/SpacehuhnTech/esp8266_deauther" rel="noopener" target="_blank">
    Wi-Fi Deauther
   </a>
   项目的
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/SpacehuhnTech/esp8266_deauther/releases" href="https://github.com/SpacehuhnTech/esp8266_deauther/releases" rel="noopener" target="_blank">
    发布页面
   </a>
   看一下，确保您得到的是最新的固件版本。找到并下载最新的 Deauther Watch 的BIN文件，目前应该是以下文件之一：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">https://github.com/SpacehuhnTech/esp8266_deauther/releases/download/2.6.0/esp8266_deauther_2.6.0_DSTIKE_DEAUTHER_WATCH.bin

https://github.com/SpacehuhnTech/esp8266_deauther/releases/download/2.6.0/esp8266_deauther_2.6.0_DSTIKE_DEAUTHER_WATCH_V2.bin</code></pre>
  <p class="graf graf--p">
   如果您在安装固件时有任何问题，可以在 GitHub上 Spacehuhn 的
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/SpacehuhnTech/esp8266_deauther/wiki" href="https://github.com/SpacehuhnTech/esp8266_deauther/wiki" rel="noopener" target="_blank">
    Wi-Fi Deauther Wiki
   </a>
   上找到所需的命令和一些在手表上安装BIN文件的技巧和窍门。
  </p>
  <p class="graf graf--p">
   使用 Micro-USB 电缆将 Deauther手表上的 ESP8266 微控制器插入您的电脑，然后找到它所连接的端口。要做到这一点，在macOS上使用 ls /dev/cu.*，在Linux上使用 dmesg | grep tty，或者在Windows上通过设备管理器查找com端口。
  </p>
  <p class="graf graf--p">
   当您找到正确的端口时，用下面的命令刷新固件。确保用您的 Deauther所连接的端口替换 /dev/ttyUSB0，如果BIN文件不是同一版本，则改变其文件名。
  </p>
  <pre class="graf graf--pre"><code>esptool.py -p /dev/ttyUSB0 write_flash -fm dout 0x0000 esp8266_deauther_2.6.0_DSTIKE_DEAUTHER_WATCH.bin</code></pre>
  <p class="graf graf--p">
   这应该会把固件写入设备，但屏幕可能不会打开。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤2：打开屏幕（如果需要）
   </strong>
  </h3>
  <p class="graf graf--p">
   如果您的 Deauther Watch 的屏幕不起作用，那么您将需要手动打开它。Wi-Fi Deauther Wiki 有一个很好的
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/SpacehuhnTech/esp8266_deauther/wiki/Setup-Display-&amp;-Buttons" href="https://github.com/SpacehuhnTech/esp8266_deauther/wiki/Setup-Display-&amp;-Buttons" rel="noopener" target="_blank">
    设置显示和按钮
   </a>
   资源，如果您在任何时候需要它。
  </p>
  <p class="graf graf--p">
   在您的 Deauther Watch 仍然通过 Micro-USB电缆连接到您的电脑时，用以下命令连接到它的屏幕。您需要用您的 Deauther Watch 所连接的端口来替换该端口。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">~$ screen /dev/ttyUSB0 115200

MicroPython v1.15 on 2021-05-14; ESP module with ESP8266
Type "help()" for more information.
&gt;&gt;&gt;</code></pre>
  <p class="graf graf--p">
   或者，您可以在 Arduino IDE 中连接到它。如果您想这样做，打开 Arduino IDE，点击菜单中的 “工具”，选择 “端口”，并选择您连接的 Deauther Watch 的端口。然后，按键盘上的 Command-Shift-M 或点击当前窗口中的串行监视器按钮来打开串行监视器。
  </p>
  <p class="graf graf--p">
   连接后，无论是通过终端还是 Arduino IDE，输入help来查看命令列表，并确认您的连接是正确的。您应该看到像下面这样的输出：
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">&gt;&gt;&gt; help

[===== List of commands =====]
help
scan [&lt;all/aps/stations&gt;] [-t &lt;time&gt;] [-c &lt;continue-time&gt;] [-ch &lt;channel&gt;]
show [selected] [&lt;all/aps/stations/names/ssids&gt;]
select [&lt;all/aps/stations/names&gt;] [&lt;id&gt;]
deselect [&lt;all/aps/stations/names&gt;] [&lt;id&gt;]
add ssid &lt;ssid&gt; [-wpa2] [-cl &lt;clones&gt;]
add ssid -ap &lt;id&gt; [-cl &lt;clones&gt;] [-f]
add ssid -s [-f]
add name &lt;name&gt; [-ap &lt;id&gt;] [-s]
add name &lt;name&gt; [-st &lt;id&gt;] [-s]
add name &lt;name&gt; [-m &lt;mac&gt;] [-ch &lt;channel&gt;] [-b &lt;bssid&gt;] [-s]
set name &lt;id&gt; &lt;newname&gt;
enable random &lt;interval&gt;
disable random
load [&lt;all/ssids/names/settings&gt;] [&lt;file&gt;]
save [&lt;all/ssids/names/settings&gt;] [&lt;file&gt;]
remove &lt;ap/station/name/ssid&gt; &lt;id&gt;
remove &lt;ap/station/names/ssids&gt; [all]
attack [beacon] [deauth] [deauthall] [probe] [nooutput] [-t &lt;timeout&gt;]
attack status [&lt;on/off&gt;]
stop &lt;all/scan/attack/script&gt;
sysinfo
clear
format
print &lt;file&gt; [&lt;lines&gt;]
delete &lt;file&gt; [&lt;lineFrom&gt;] [&lt;lineTo&gt;]
replace &lt;file&gt; &lt;line&gt; &lt;new-content&gt;
copy &lt;file&gt; &lt;newfile&gt;
rename &lt;file&gt; &lt;newfile&gt;
run &lt;file&gt;
write &lt;file&gt; &lt;commands&gt;
get &lt;setting&gt;
set &lt;setting&gt; &lt;value&gt;
reset
chicken
reboot
info
// &lt;comments&gt;
send deauth &lt;apMac&gt; &lt;stMac&gt; &lt;rason&gt; &lt;channel&gt;
send beacon &lt;mac&gt; &lt;ssid&gt; &lt;ch&gt; [wpa2]
send probe &lt;mac&gt; &lt;ssid&gt; &lt;ch&gt;
led &lt;r&gt; &lt;g&gt; &lt;b&gt; [&lt;brightness&gt;]
led &lt;#rrggbb&gt; [&lt;brightness&gt;]
led &lt;enable/disable&gt;
draw
screen &lt;on/off&gt;
screen mode &lt;menu/packetmonitor/buttontest/loading&gt;
========================================================================
for more information please visit github.com/spacehuhn/esp8266_deauther
========================================================================</code></pre>
  <p class="graf graf--p">
   现在，在终端或Arduino IDE中运行以下命令以启用屏幕：
  </p>
  <pre class="graf graf--pre"><code>&gt;&gt;&gt; set display true;;save settings</code></pre>
  <p class="graf graf--p">
   您可能需要重新启动设备，使设置生效。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤3：创建一个反应式目标（可选）
   </strong>
  </h3>
  <p class="graf graf--p">
   为了有合法的东西来练习，最好创建一个反应式目标，这基本上是一个Wi-Fi黑客测试网络上的设备。可以在 Arduino IDE 默认的 “WiFiAccessPoint” 草图基础上，为基于ESP8266的微控制器（如D1 Mini）制作一个。
  </p>
  <p class="graf graf--p">
   Kody Kinzie 在GitHub上的
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/skickar/WiFiHackingWorkshop/" href="https://github.com/skickar/WiFiHackingWorkshop/" rel="noopener" target="_blank">
    WiFiHackingWorkshop
   </a>
   项目中有一个修改过的草图。该草图是
   <a class="markup--anchor markup--p-anchor" data-href="https://github.com/skickar/WiFiHackingWorkshop/blob/master/ReactiveTarget.ino" href="https://github.com/skickar/WiFiHackingWorkshop/blob/master/ReactiveTarget.ino" rel="noopener" target="_blank">
    ReactiveTarget.ino
   </a>
   文件，下载该文件，然后将其刷到您的ESP8266上。下面的代码框显示了 ReactiveTarget.ino 文件的内容，如果您想要重新构建它的话。
  </p>
  <pre class="graf graf--pre"><code class="markup--code markup--pre-code">// SIMPLE Wi-FI LINK MONITOR BY SKICKAR - Based on Henry's Bench Wi-Fi link checker
// This project has the goal to connect an ioT device to a Wi-Fi network and monitor the ability to establish a normal wireless connection.
// The project uses only three componants - A nodeMCU, a breadboard, and one RGB LED.
    #include &lt;ESP8266WiFi.h&gt; // First, we include the libraries we need to make this work on the ESP8266
#include &lt;ESP8266WiFi.h&gt;
#include &lt;ESP8266HTTPClient.h&gt;

    const char* ssid     = "Control"; // Next, we set the name of the network to monitor.
    const char* password = "testytest"; // After that, we enter the password of the network to monitor.
    int wifiStatus; // Here, we create a variable to check the status of the Wi-Fi connection.
    int connectSuccess = 0, highTime = 500, lowtime = 500; // And now, we set a variable to count the number of times we've been able to successfully connect, and how long the LED will stay on and off for.

void red() { // Here, we will map a function called "red" to the right pin that will light up the red LED for the amount of time we defined in hightTime for how long it is lit, and lowTime for how long it is off each time we pulse a red LED.
      digitalWrite(D1, HIGH), delay(highTime), digitalWrite(D1, LOW), delay(lowtime);  // We map the red function to the D5 pin, so that each time we call red() it will pulse power on the D5 pin.
}
void green() { // We do the same with green, mapping the D6 pin to the green() function.
      digitalWrite(D2, HIGH), delay(highTime), digitalWrite(D2, LOW), delay(lowtime);
}
void blue() { // Finally, we do the same with blue, mapping it to the D7 pin.
      digitalWrite(D3, HIGH), delay(highTime), digitalWrite(D3, LOW), delay(lowtime);
}
void setup() { // The setup function runs only once when the device starts up.
  unsigned long previousMillis = 0;        // will store last time LED was updated

// constants won't change:
const long interval = 1000;           // interval at which to blink (milliseconds)

  pinMode(D1, OUTPUT), pinMode(D2, OUTPUT), pinMode(D3, OUTPUT); // In this case, we will activate the D5, D6, and D7 pins for output mode.
      WiFi.begin(ssid, password); // The last part of setup we will write is to start the Wi-Fi connection process.
      }

void loop() { // This loop will run over and over again, unlike the setup function, which will only run once.
          HTTPClient http;
          http.begin(/*client, */ "http://192.168.4.1");

        int httpCode   = http.GET();
        String payload = http.getString();

        if (httpCode &gt; 0) {
        } else {
            Serial.printf("ERROR %d\n", httpCode);
        }

      //delay(1000); // Set a delay of one second per cycle of checking the status of the link.
      wifiStatus = WiFi.status(); // First, we'll check the status of the Wi-Fi connection and store the result in the variable we created, wifiStatus.
      if(connectSuccess == 0){ blue();} // If device is not connected and never has successfully connected, flash the blue light. This could mean the network doesn't exist, is out of range, or you misspelled the SSID or password.
      if(wifiStatus == WL_CONNECTED){ green(), connectSuccess ++; } // If the device is connected, flash the green light, and add one to the count of the "connectSuccess" variable. This way, we will know to flash the red light if we lose the connection.
      else if(connectSuccess != 0){ red(); } // If the connection is not active but we have been able to connect before, flash the red LED. That means the AP is down, a jamming attack is in progress, or a normal link is otherwise impossible.

}</code></pre>
  <p class="graf graf--p">
   这个草图会不断检查Wi-Fi网络是否可以访问，设备是否可以成功连接到它，或者它是否被阻止。如果它被阻止，那么ESP8266将以红色闪光警告您，如果它能够成功连接，它将以绿色闪光告诉您。如果它根本无法连接，意味着接入点出了问题，ESP8266 将闪烁蓝色。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤4：扫描目标网络
   </strong>
  </h3>
  <p class="graf graf--p">
   现在，我们可以通过翻转侧面的开关来打开 Deauther Watch。在主菜单中，使用滚动开关选择SCAN选项，然后按下开关进入扫描菜单。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 1067px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="1032" data-image-id="0*9yIAog9C7fxdU1V9.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*9yIAog9C7fxdU1V9.jpg?resize=1067%2C756&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" height="756" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*9yIAog9C7fxdU1V9.jpg?resize=1067%2C756&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1067"/>
     <noscript>
      <img alt="" class="graf-image" data-height="1032" data-image-id="0*9yIAog9C7fxdU1V9.jpg" data-recalc-dims="1" data-width="1456" height="756" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*9yIAog9C7fxdU1V9.jpg?resize=1067%2C756&amp;ssl=1" width="1067"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Image by Retia/Null Byte
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   在扫描菜单中，您可以决定扫描接入点（SCAN APs）、设备端（SCAN STATIONS）或两者（SCAN AP + ST）。在您决定扫描哪一个并通过滚动开关选择后，按下开关开始扫描。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 1067px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="1022" data-image-id="0*2B2CdvA3jS1RbL7_.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*2B2CdvA3jS1RbL7_.jpg?resize=1067%2C748&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" height="748" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*2B2CdvA3jS1RbL7_.jpg?resize=1067%2C748&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1067"/>
     <noscript>
      <img alt="" class="graf-image" data-height="1022" data-image-id="0*2B2CdvA3jS1RbL7_.jpg" data-recalc-dims="1" data-width="1456" height="748" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*2B2CdvA3jS1RbL7_.jpg?resize=1067%2C748&amp;ssl=1" width="1067"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Image by Retia/Null Byte
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   扫描完成后，它将显示发现了多少个AP、stations 或两者。现在，回到主菜单，打开 SELECT 菜单。在这里，您可以看到扫描所检测到的东西。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 1067px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="1132" data-image-id="0*wqudQ3C9iWZfWrfr.jpg" data-lazy-src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*wqudQ3C9iWZfWrfr.jpg?resize=1067%2C829&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" height="829" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*wqudQ3C9iWZfWrfr.jpg?resize=1067%2C829&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1067"/>
     <noscript>
      <img alt="" class="graf-image" data-height="1132" data-image-id="0*wqudQ3C9iWZfWrfr.jpg" data-recalc-dims="1" data-width="1456" height="829" src="https://i2.wp.com/cdn-images-1.medium.com/max/1067/0*wqudQ3C9iWZfWrfr.jpg?resize=1067%2C829&amp;ssl=1" width="1067"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Image by Retia/Null Byte
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   接下来，浏览 APs、Stations、Names 和 SSIDs 选项，直到您找到您的反应目标。选择您的目标，并按下滚轮，用星号（*）突出显示目标，并将其保存到目标列表中。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    步骤5: 攻击目标网络
   </strong>
  </h3>
  <p class="graf graf--p">
   回到主菜单，这次选择 “攻击”，在那里，您可以选择使用 DEAUTH、BEACON 或 PROBE 攻击。
  </p>
  <p class="graf graf--p">
   如果您想一次又一次地克隆，可以使用 BEACON 攻击。如果想发送一些探测帧以寻找这个网络或设备，可以尝试使用 PROBE 攻击。
  </p>
  <p class="graf graf--p">
   这里将选择DEAUTH攻击。选择DEAUTH，然后往下走到START，按下按钮，开始。这应该会使目标与它的网络断开，ESP8266反应式目标应该开始闪烁红色信号。
  </p>
  <figure class="graf graf--figure">
   <p>
    <figure class="wp-caption aligncenter" style="width: 1067px">
     <img alt="" class="graf-image jetpack-lazy-image" data-height="1025" data-image-id="0*ushKVNEnGQqi8QQF.jpg" data-lazy-src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*ushKVNEnGQqi8QQF.jpg?resize=1067%2C751&amp;is-pending-load=1#038;ssl=1" data-recalc-dims="1" data-width="1456" height="751" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*ushKVNEnGQqi8QQF.jpg?resize=1067%2C751&amp;ssl=1" srcset="data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7" width="1067"/>
     <noscript>
      <img alt="" class="graf-image" data-height="1025" data-image-id="0*ushKVNEnGQqi8QQF.jpg" data-recalc-dims="1" data-width="1456" height="751" src="https://i1.wp.com/cdn-images-1.medium.com/max/1067/0*ushKVNEnGQqi8QQF.jpg?resize=1067%2C751&amp;ssl=1" width="1067"/>
     </noscript>
     <figcaption class="wp-caption-text">
      Image by Retia/Null Byte
     </figcaption>
    </figure>
   </p>
  </figure>
  <p class="graf graf--p">
   您应该成功地干扰了目标的Wi-Fi，而目标应该不再连接到Wi-Fi网络。一旦您准备停止，可以再次按下按钮来停止攻击，而目标可以再次加入网络。
  </p>
  <p class="graf graf--p">
   这只是一个简单的小演示，说明您可以如何使用 Deauther Watch 来扫描、选择和攻击一个网络。要再次开始攻击设备，只需再次启动攻击。
  </p>
  <h3 class="graf graf--p">
   <strong class="markup--strong markup--p-strong">
    安全使用您的 DeautherWatch
   </strong>
  </h3>
  <p class="graf graf--p">
   Deauther Watch 是一个非常了不起的项目，也是支持 Wi-Fi Deauther 项目开发者的一个好方法。请记住，它可能在做一些在您的国家或地区可能是非法的事，比如入侵一个您没有权限攻击的Wi-Fi网络。这可能是一个严重的问题，所以，在您开始对您没有权限测试的网络使用这个设备之前，请确保您检查了当地的法律。⚪️
  </p>
  <p class="graf graf--p">
   <a class="markup--anchor markup--p-anchor" data-href="https://null-byte.wonderhowto.com/how-to/hack-networks-devices-right-from-your-wrist-with-wi-fi-deauther-watch-0296283/" href="https://null-byte.wonderhowto.com/how-to/hack-networks-devices-right-from-your-wrist-with-wi-fi-deauther-watch-0296283/" rel="noopener" target="_blank">
    Hack Networks &amp; Devices Right from Your Wrist with the Wi-Fi Deauther Watch
   </a>
  </p>
  <div id="atatags-1611829871-6108a0c28af9f">
  </div>
  <div class="sharedaddy sd-sharing-enabled">
   <div class="robots-nocontent sd-block sd-social sd-social-icon sd-sharing">
    <h3 class="sd-title">
     共享此文章：
    </h3>
    <div class="sd-content">
     <ul>
      <li class="share-twitter">
       <a class="share-twitter sd-button share-icon no-text" data-shared="sharing-twitter-16846" href="https://www.iyouport.org/%e4%bd%bf%e7%94%a8wi-fi-deauther%e6%89%8b%e8%a1%a8%ef%bc%8c%e5%9c%a8%e6%82%a8%e7%9a%84%e6%89%8b%e8%85%95%e4%b8%8a%e7%9b%b4%e6%8e%a5%e7%a0%b4%e8%a7%a3%e7%bd%91%e7%bb%9c%e5%92%8c%e8%ae%be%e5%a4%87/?share=twitter" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到Twitter">
        <span>
        </span>
        <span class="sharing-screen-reader-text">
         点击分享到Twitter（在新窗口中打开）
        </span>
       </a>
      </li>
      <li class="share-facebook">
       <a class="share-facebook sd-button share-icon no-text" data-shared="sharing-facebook-16846" href="https://www.iyouport.org/%e4%bd%bf%e7%94%a8wi-fi-deauther%e6%89%8b%e8%a1%a8%ef%bc%8c%e5%9c%a8%e6%82%a8%e7%9a%84%e6%89%8b%e8%85%95%e4%b8%8a%e7%9b%b4%e6%8e%a5%e7%a0%b4%e8%a7%a3%e7%bd%91%e7%bb%9c%e5%92%8c%e8%ae%be%e5%a4%87/?share=facebook" rel="nofollow noopener noreferrer" target="_blank" title="点击分享到 Facebook ">
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
  <div class="sharedaddy sd-block sd-like jetpack-likes-widget-wrapper jetpack-likes-widget-unloaded" data-name="like-post-frame-161182987-16846-6108a0c28b758" data-src="https://widgets.wp.com/likes/#blog_id=161182987&amp;post_id=16846&amp;origin=www.iyouport.org&amp;obj_id=161182987-16846-6108a0c28b758" id="like-post-wrapper-161182987-16846-6108a0c28b758">
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
    <a href="https://www.iyouport.org/tag/deauther-watch/" rel="tag">
     Deauther Watch
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
    <a href="https://www.iyouport.org/tag/technology/" rel="tag">
     Technology
    </a>
   </li>
   <li>
    <a href="https://www.iyouport.org/tag/wi-fi-hacking/" rel="tag">
     Wi-Fi hacking
    </a>
   </li>
  </ul>
 </div>
 <div class="entry-author-wrapper">
  <div class="site-posted-on">
   <strong>
    Published
   </strong>
   <time class="entry-date published" datetime="2021-08-03T00:04:15+08:00">
    2021年8月3日
   </time>
   <time class="updated" datetime="2021-05-24T15:43:05+08:00">
    2021年5月24日
   </time>
  </div>
 </div>
</article>

