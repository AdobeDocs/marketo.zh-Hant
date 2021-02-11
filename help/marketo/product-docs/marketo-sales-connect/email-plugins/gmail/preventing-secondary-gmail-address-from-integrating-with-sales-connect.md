---
unique-page-id: 14352546
description: 防止次要Gmail位址與Sales Connect - Marketo Docs —— 產品檔案整合
title: 防止次要Gmail位址與Sales Connect整合
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# 防止次Gmail地址與Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}整合

## 中斷的Gmail整合（為什麼我的個人Gmail會傳送電子郵件）{#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail連線中斷的最常見原因，是用戶個人帳戶意外整合。 當使用者按一下「連線」或嘗試從個人帳戶傳送電子郵件時，就會發生這種情況。 這很有誘惑力，因為當您在工作電子郵件中存取您的Chrome帳戶時，會有這個選項。

## 為什麼Sales Connect甚至會嘗試與我的個人Gmail整合？{#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect透過Chrome瀏覽器中安裝的擴充功能與Gmail整合。 每當Gmail開啟時，它就會提供與它整合的選項。 為防止與您個人Gmail帳戶整合，我們建議以下三項之一……

以其他Chrome使用者身分登入（建議）

按一下[此連結](https://support.google.com/chrome/answer/2364824?hl=en)以閱讀如何建立其他Chrome設定檔。

**專業**:以其他使用者身分登入，將會開啟新的Chrome例項。此例項是Chrome的全新視窗，您的舊擴充功能不會存在此視窗中。 它還保存了cookies，因此您不必每次都登入Gmail。

**缺點**:必須開啟兩個Chrome視窗。

使用其他瀏覽器

**專業人** 員：使用未安裝擴充功能的其他網際網路瀏覽器（IE或Firefox），將可避免發生此情況。

**缺點**:使用多種瀏覽器可能會很煩人。

使用Incognito窗口

**專業人** 員：隱姓埋名的視窗就像開啟Chrome的裸體版本。也就是說，它不會安裝您的任何擴充功能，而且Sales Connect也不會連接。

**缺點**:每次開始使用Gmail時，您都必須登入，如果不小心關閉視窗，您必須再次登入。
