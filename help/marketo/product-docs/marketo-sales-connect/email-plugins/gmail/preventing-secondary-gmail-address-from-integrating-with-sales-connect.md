---
unique-page-id: 14352546
description: 防止次要Gmail位址與Sales Connect整合 — Marketo檔案 — 產品檔案
title: 防止次要Gmail位址與Sales Connect整合
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 正在防止次要Gmail位址與[!DNL Sales Connect]整合 {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Gmail整合中斷（為什麼我的個人Gmail會傳送電子郵件） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail連線中斷的最常見原因是意外整合使用者的個人帳戶。 當使用者按一下「連線」或嘗試從個人帳戶傳送電子郵件時，就可能發生這種情況。 這可能非常誘人，因為當您存取Gmail帳戶時，該選項會與您的工作電子郵件位於同一個[!DNL Chrome]執行個體中。

## 為什麼[!DNL Sales Connect]會嘗試與我的個人Gmail整合？ {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect]透過[!DNL Chrome]瀏覽器中安裝的擴充功能與Gmail整合。 每當擴充功能偵測到Gmail執行個體開啟時，它都會提供整合選項。 若要避免與您的個人Gmail帳戶整合，我們建議您執行下列三件事之一……

以其他[!DNL Chrome]使用者登入（建議）

按一下[此連結](https://support.google.com/chrome/answer/2364824?hl=en)以瞭解如何建立另一個[!DNL Chrome]設定檔。

**優點**：以其他使用者身分登入將會開啟[!DNL Chrome]的新執行個體。 此執行個體是[!DNL Chrome]的全新視窗，舊擴充功能將不會存在於此執行個體中。 它也會保留Cookie，因此您不必每次都登入Gmail。

**缺點**：必須開啟兩個[!DNL Chrome]視窗。

使用其他瀏覽器

**優點：**&#x200B;使用其他未安裝擴充功能的網際網路瀏覽器（IE或Firefox）將可防止發生此情況。

**缺點**：使用多個瀏覽器可能會很麻煩。

使用無痕視窗

**優點：**&#x200B;無痕視窗就像開啟裸體版本的[!DNL Chrome]。 表示它不會安裝您的任何擴充功能，[!DNL Sales Connect]將不會在那裡連線。

**缺點**：每次開始工作時，您必須登入Gmail，如果意外關閉視窗，請再登入一次。
