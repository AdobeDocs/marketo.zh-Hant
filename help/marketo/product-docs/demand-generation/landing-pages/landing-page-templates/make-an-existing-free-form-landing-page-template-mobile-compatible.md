---
unique-page-id: 5472348
description: 讓現有的自由表單登陸頁面範本與行動裝置相容 — Marketo檔案 — 產品檔案
title: 讓現有的自由表單登陸頁面範本與行動裝置相容
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 讓現有的自由表單登陸頁面範本與行動裝置相容 {#make-an-existing-free-form-landing-page-template-mobile-compatible}

您可以在範本編輯器和登入頁面編輯器兩個位置執行此操作。

## 從範本編輯器升級 {#upgrade-from-the-template-editor}

1. 前往 **Design Studio**.

   ![](assets/designstudio-1.png)

1. 選取 **範本**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. 選取範本，其中 **與行動裝置相容** 是 **否**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. 按一下 **編輯草稿**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. 按一下 **讓行動裝置相容**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. 按一下 **升級**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   您的登入頁面範本現在與行動裝置相容！

   >[!NOTE]
   >
   >升級應該不會有害，但請務必檢查頁面是否有任何差異。 升級會使用該範本建立任何登入頁面的草稿。

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## 是什麼讓範本行動裝置相容？ {#what-makes-a-template-mobile-compatible}

好問題！ 您的範本必須有下列標籤：

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

如果一切正常，您會看到此訊息。

![](assets/image2015-1-22-20-3a41-3a31.png)

如果發生錯誤，會顯示錯誤訊息，請按一下「修復」以修正問題並重複驗證程式。

![](assets/image2015-1-22-20-3a43-3a20.png)

如果您對範本進行任何變更，請按一下範本動作並選取驗證行動相容性。

## 從自由格式登陸頁面編輯器升級範本 {#upgrading-a-template-from-the-free-form-landing-page-editor}

當您編輯登入頁面並按一下行動標籤時，您有時會注意到範本尚未升級。 不要害怕！ 您可以在這裡進行升級。

1. 按一下 **行動** 標籤。

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. 按一下核取方塊並按一下 **啟動**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >啟用行動版範本將會建立使用該範本之任何登入頁面的草稿。

棒極了！ 您現在可以 [自訂行動檢視](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) 使用此範本的所有登入頁面中。
