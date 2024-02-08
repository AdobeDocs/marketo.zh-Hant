---
description: 通知 — Websocket連線 — Marketo檔案 — 產品檔案
title: 通知 — Websocket連線
hide: true
hidefromtoc: true
source-git-commit: 77300e8d620887b5c1d14a4f979a96488b6eec87
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# 通知： Websocket連線 {#notification-websocket-connection}

本文適用於在Marketo例項中收到下列通知的Marketo Engage使用者： `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

如果您或您的組織使用限制性的防火牆或Proxy伺服器設定，您或您的網路管理員可能需要將某些網域和IP位址範圍列入允許清單，以確保Adobe Marketo Engage如期運作。

Marketo支援未設定為協助實作下列通訊協定。 如果您需要協助，請與您的IT團隊分享此文章。 如果他們使用允許清單限制網頁存取，請要求他們新增以下網域（包括星號），以允許所有Marketo資源和網頁通訊端：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
