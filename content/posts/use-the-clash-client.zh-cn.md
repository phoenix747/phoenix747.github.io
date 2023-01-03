---
title: "使用clash客户端"
date: 2022-12-26T17:11:48+08:00
draft: false
summary: "最强客户端之一"
weight: 14
series: ["Do-It-Yourself Free Ladder Building Guide"]
---

单服务端节点极容易触发短时防火墙屏蔽，怀疑触发了防火墙异常流量大小检测。

既然 Google Cloud 可以免费用，而且单节点 3 个月自用根本用不完 300 美金。

那自然我们要多搭几个服务端来用。clash 在自动切流上比较优秀（IOS 上我用的小火箭），比较适合 PC 和软路由场景。

clash 默认不支持 vless 比较蛋疼，我的 xray 服务端设置了 Trojan 协议，客户端使用 Trojan 了。

小火箭支持 vless。

mac 版本 clashX: <https://github.com/yichengchen/clashX>

openwrt 插件: <https://github.com/vernesong/OpenClash>

使用 clash 记得设置 load-balance 模式，这样就可以在多节点自动切流了，省去了很大一部分日常维护工作量。
