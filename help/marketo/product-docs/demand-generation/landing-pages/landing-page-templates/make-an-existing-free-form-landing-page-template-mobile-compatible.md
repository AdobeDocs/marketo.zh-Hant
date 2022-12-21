---
unique-page-id: 5472348
description: 讓現有的自由格式登錄頁面範本行動相容 — Marketo檔案 — 產品檔案
title: 讓現有的自由格式登陸頁面範本行動相容
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 讓現有的自由格式登陸頁面範本行動相容 {#make-an-existing-free-form-landing-page-template-mobile-compatible}

這可以在兩個位置執行：範本編輯器和登錄頁面編輯器。

## 從範本編輯器升級 {#upgrade-from-the-template-editor}

1. 前往 **Design Studio**.

   ![](assets/designstudio-1.png)

1. 選擇 **範本**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. 選取範本，其中 **行動相容** is **否**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. 按一下 **編輯草稿**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. 按一下 **讓行動相容**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. 按一下 **升級**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   您的登錄頁面範本現在與行動相容！

   >[!NOTE]
   >
   >升級應不會造成傷害，但請務必檢查頁面中是否有任何差異。 升級將使用該範本建立任何登錄頁面的草稿。

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## 什麼讓範本行動相容？ {#what-makes-a-template-mobile-compatible}

好問題！ 您的範本必須具備下列標籤：

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

如果一切都好，你會看到這條消息。

![](assets/image2015-1-22-20-3a41-3a31.png)

如果發生錯誤，將顯示錯誤訊息，按一下「修復」以修正問題，並重複驗證程式。

![](assets/image2015-1-22-20-3a43-3a20.png)

如果您對範本進行任何變更，請按一下範本動作，然後選取驗證行動相容性。

## 從自由格式登錄頁面編輯器升級範本 {#upgrading-a-template-from-the-free-form-landing-page-editor}

當您編輯登錄頁面並按一下行動標籤時，有時您會發現範本尚未升級。 別怕！ 您可以在那裡升級。

1. 按一下 **行動** 標籤。

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. 按一下核取方塊，然後按一下 **啟動**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >啟用行動版範本，將會建立使用該範本的任何登陸頁面的草稿。

太棒了！ 您現在可以 [自訂行動檢視](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) 使用此範本的所有登錄頁面。
