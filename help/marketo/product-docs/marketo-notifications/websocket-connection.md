---
description: 收到無法建立Websocket連線通知的Marketo Engage使用者通知詳細資料
title: 通知 — Websocket連線
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 30%

---

# 通知：Websocket 連線 {#notification-websocket-connection}

此檔案適用於在其Marketo執行個體中收到下列通知的Marketo Engage使用者： `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

如果您或您的組織使用限制性的防火牆或 Proxy 伺服器設定，您或您的網路管理員可能需要將特定網域與 IP 位址範圍加入允許清單，以確保 Adobe Marketo Engage 如預期般運作。

Marketo支援未設定為協助實作下列通訊協定。 如果您需要協助，請與您的IT團隊共用此檔案。 如果他們使用允許清單限制網頁存取，請要求他們新增以下網域（包括星號），以允許所有Marketo資源和網頁通訊端：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
