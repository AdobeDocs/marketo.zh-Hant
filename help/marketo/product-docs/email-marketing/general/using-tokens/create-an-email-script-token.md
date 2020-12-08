---
unique-page-id: 1900577
description: 建立電子郵件指令碼Token —— 行銷檔案——產品檔案
title: 建立電子郵件指令碼Token
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---


# 建立電子郵件指令碼Token {#create-an-email-script-token}

對於進階開發人員，您可以在電子郵件 [中使用](http://velocity.apache.org/engine/1.7/user-guide.html) Velocity指令碼。 這是如何做到的。

1. 前往行 **銷活動**。

   ![](assets/ma.png)

1. 尋找並選取任何方案（事件、預設或參與等）。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 在「我的 **代號** 」索引標籤下，拖曳 **電子郵件指令碼代號** 。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. 命名您的電子郵件指令碼Token, **然後按一下以編輯** 其內容。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 使用右側的樹狀結構拖 **曳Person、Opportunity****或Custom Object** Token。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >訪問陣列（業務機會或自定義對象）時，您只能訪問與該人員關聯的最近10個項目。

1. 請注意，將Token拖曳至指令碼編輯器後，Token會變為勾選／作用中。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >如果您輸入Token自由格式，請確定檢查／啟用樹狀結構中所有對應的Token，否則這些Token將被視為純文字而無法運作。

1. 以Velocity編寫您的指令碼。 以下是一些有用的資源：

   * [行銷人員電子郵件指令碼檔案](http://developers.marketo.com/email-scripting/)
   * [Velocity使用指南](http://velocity.apache.org/engine/devel/user-guide.html)
   * [速度參考指南](http://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity工具Javadoc](http://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. 完成指令碼後，按一下「保 **存」**。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 再按 **一下** 「儲存」。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

現在，您可以在電子郵件中使用此Token。 每次傳送電子郵件時，都會執行指令碼。

>[!NOTE]
>
>**相關文章**
>
>* [將電子郵件指令碼Token新增至您的電子郵件](add-an-email-script-token-to-your-email.md)

>



