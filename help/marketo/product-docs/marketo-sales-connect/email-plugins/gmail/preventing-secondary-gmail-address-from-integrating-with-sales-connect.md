---
unique-page-id: 14352546
description: 防止次要Gmail位址與Sales Connect整合 — Marketo檔案 — 產品檔案
title: 阻止輔助Gmail地址與Sales Connect整合
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 阻止輔助Gmail地址與Sales Connect整合 {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## 中斷的Gmail整合（為什麼我的個人Gmail會傳送電子郵件） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail連線中斷的最常見原因，是使用者個人帳戶意外整合。 當使用者按一下「連線」或嘗試從其個人帳戶傳送電子郵件時，就會發生此情況。 這麼做可能會很誘人，因為在與您工作電子郵件相同的Chrome例項中存取您的Gmail帳戶時，將會存在此選項。

## Sales Connect為何還嘗試與我的個人Gmail整合？ {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect透過Chrome瀏覽器中安裝的擴充功能與Gmail整合。 每當Gmail的擴充功能偵測到某個例項開啟時，就能提供整合的選項。 為防止與您個人的Gmail帳戶整合，我們建議您執行下列三項其中一項操作……

以其他Chrome使用者身分登入（建議）

按一下 [此連結](https://support.google.com/chrome/answer/2364824?hl=en) 以閱讀如何建立其他Chrome設定檔。

**優點**:以其他使用者身分登入時，會開啟Chrome的新例項。 此例項是Chrome的全新視窗，此例項中不會有任何舊擴充功能。 它還保留Cookie，這樣您就不必每次都登入Gmail。

**缺點**:必須開啟兩個Chrome視窗。

使用其他瀏覽器

**優點：** 使用未安裝擴充功能的其他網際網路瀏覽器（IE或Firefox）將會阻止此情況發生。

**缺點**:使用多個瀏覽器可能會很煩人。

使用無痕窗口

**優點：** 無痕窗口就像開啟了Chrome的裸體版本。 這表示它將不會安裝您的任何擴充功能，而Sales Connect將不會在那裡進行連接。

**缺點**:每次開始使用時，您都必須登入Gmail，如果不小心關閉視窗，也必須登入。
