---
title: my-token-email-script
description: 我的Token電子郵件指令碼
exl-id: 8dd28274-578a-4184-b7bb-b46b59ebe410
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 我的代號：電子郵件指令碼

<br> 

對於進階開發人員，您可以透過設定電子郵件指令碼Token，在電子郵件中使用[Velocity指令碼](https://velocity.apache.org/engine/1.7/user-guide.html)。 這是如何做到的。

1. 在程式或資料夾的[!UICONTROL My Tokens]標籤中，將&#x200B;**[!UICONTROL Email Script]**&#x200B;代號拖曳至[!UICONTROL Local Tokens]畫布。

   ![影像一](/help/sky/assets/my-tokens/my-token-email-script/my-token-email-script-1.png)

1. 從右側的樹狀結構拖曳Token。

   ![影像2](/help/sky/assets/my-tokens/my-token-email-script/my-token-email-script-2.png)

1. 請注意，標籤新增後會被勾選／啟用。

   ![影像三](/help/sky/assets/my-tokens/my-token-email-script/my-token-email-script-3.png)

   >[!CAUTION]
   >
   >如果您是以自由格式輸入Token，請務必檢查／啟用樹狀結構中所有對應的Token，否則這些Token會被視為純文字，而無法運作。

1. 以Velocity編寫您的指令碼。 以下是一些有用的資源可協助您：

   * [Marketo開發人員電子郵件指令碼檔案](https://developers.marketo.com/email-scripting/)
   * [Velocity使用指南](https://velocity.apache.org/engine/devel/user-guide.html)
   * [速度參考指南](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [VelocityTools 2.0檔案](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. 完成指令碼後，按一下&#x200B;**[!UICONTROL Save]**。

   ![影像4](/help/sky/assets/my-tokens/my-token-email-script/my-token-email-script-4.png)
