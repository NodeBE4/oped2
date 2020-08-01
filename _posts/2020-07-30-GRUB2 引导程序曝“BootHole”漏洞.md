---
layout: post
title: "GRUB2 引导程序曝“BootHole”漏洞"
date: 2020-07-30T13:50:00.000Z
author: Solidot
from: https://www.solidot.org/story?sid=65102
tags: [ Solidot ]
categories: [ news, Solidot ]
---
<!--1596117000000-->
[GRUB2 引导程序曝“BootHole”漏洞](https://www.solidot.org/story?sid=65102)
------

<div>
GRUB2 引导程序曝出名为“<a href="https://www.debian.org/security/2020-GRUB-UEFI-SecureBoot/" target="_blank"><u>BootHole</u></a>”的漏洞，允许恶意攻击者完全绕过 UEFI Secure Boot。UEFI Secure Boot 是一个验证机制，确保 UEFI 固件运行的代码是可信的，防止在引导阶段就加载和运行恶意代码。GRUB2 引导程序代码中发现了一个严重 bug，它破坏了信任链，通过利用该 bug 将能突破安全环境，在早期引导阶段加载未签名代码。该漏洞由 Eclypsium 的研究人员发现，被命名为 BootHole。修复该问题不能只靠新的 GRUB2 安全程序，而是需要更新 <a href="https://uefi.org/revocationlistfile"><u>UEFI revocation list</u></a> 文件，一旦完成更新，之前的 GRUB2 程序将无法再使用。                      <img src="https://img.solidot.org//0/446/liiLIZF8Uh6yM.jpg" style="display:block;margin:5px 0" referrerpolicy="no-referrer">
</div>
