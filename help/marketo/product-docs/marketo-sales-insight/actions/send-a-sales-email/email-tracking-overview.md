---
description: 電子郵件追蹤概觀 — Marketo檔案 — 產品檔案
title: 電子郵件追蹤概觀
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 電子郵件追蹤概觀 {#email-tracking-overview}

## 回覆追蹤的運作方式 {#how-reply-tracking-works}

「回覆追蹤」是透過檢視您傳送之每封電子郵件中的訊息ID來完成。 每封電子郵件都包含唯一的訊息ID，讓我們擁有一些最佳的回覆追蹤功能。

>[!PREREQUISITES]
>
>與電子郵件伺服器的連線： [!DNL Sales Connect]必須與您的收件匣連線，這樣我們才能知道何時收到新的回覆。 您必須將您的[!DNL Sales Connect]帳戶連線至Gmail。 如果您使用Outlook，我們需要與您的Exchange伺服器整合。

如果[!DNL Sales Connect]無法追蹤潛在客戶對您的電子郵件的回覆，將無法根據回覆偵測停止行銷活動或將回覆記錄到Salesforce。 什麼是任何電子郵件地址可以回覆？

這表示如果您傳送電子郵件給flynn@flynnsarcade.com，而他使用kevinf@flynnsarcade.com回應，我們就能追蹤回應。 此外，如果您以電子郵件傳送flynn@flynnsarcade.com和CC alan@encom.com ，而Alan將您回寫，它也會偵測回覆並結束行銷活動。

## 如何追蹤您的電子郵件附件 {#how-to-track-your-email-attachments}

[!DNL Sales Connect]提供您附件(.doc、.ppt、.pdf)的追蹤功能，讓您檢視附件何時已開啟/下載，以及收件者正在瀏覽的頁面。 我們將允許您使用[網頁應用程式](https://toutapp.com/login)和Gmail (或Google應用程式)中的可追蹤附件功能。

>[!NOTE]
>
>附件追蹤僅適用於我們的團隊計畫（從我們的g3startup計劃開始）。

**如何傳送您的第一個可追蹤附件**

1. 撰寫電子郵件或編輯範本，然後按一下&#x200B;**[!UICONTROL Content]**&#x200B;按鈕。

1. 上傳您的附件並將其寄出。 我們支援PDF、[!DNL Word]檔案和[!DNL Powerpoint]簡報。

1. 選擇「**[!UICONTROL Add to Email]**」。

1. 按一下&#x200B;**[!UICONTROL Send]**&#x200B;並啟動您的即時摘要。 您會在收件者開啟並瀏覽附件時看到收件者。

>[!TIP]
>
>如果您不想追蹤附件，只要按一下[附加檔案]，就不會追蹤此附件。

## 檢視追蹤的運作方式 {#how-view-tracking-works}

我們會在您傳送的電子郵件內放置不可見的影像，以追蹤電子郵件開啟次數。

如果有人回覆您的電子郵件，但[!DNL Sales Connect]指出未檢視，則收件者未在其電子郵件使用者端內啟用影像的機率為何（亦即，按一下電子郵件中的[按一下此處下載影像]訊息）。

在電子郵件上取得更佳追蹤統計資料的一些秘訣：

* 在電子郵件中加入影像（如標誌），鼓勵收件者啟用影像功能來檢視您的訊息。
* 在電子郵件中加入連結作為call to action。

## 測試電子郵件未顯示為已檢視 {#test-email-not-showed-as-viewed}

即使您將訊息傳送至其他電子郵件地址，我們不會記錄您檢視您在即時摘要中傳送給自己的任何電子郵件。 我們的追蹤是以裝置為基礎；只要您使用已用來登入[!DNL Sales Connect]的電腦，我們就會篩選掉該活動。

原因何在？ [!DNL Sales Connect]是聰明的，而且如果每次檢視傳送的電子郵件時，即時摘要活動中都會出現我們自己的資訊，我們的作用中使用者絕不會原諒我們。
