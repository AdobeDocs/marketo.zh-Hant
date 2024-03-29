---
unique-page-id: 2950682
description: 建立方案管道 — Marketo檔案 — 產品檔案
title: 建立方案頻道
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 建立方案頻道 {#create-a-program-channel}

方案是一個特定的行銷計畫。 此頻道旨在作為傳遞機制，例如網路研討會、贊助或線上廣告。

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>進一步瞭解 [計畫](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)是Marketo中最重要的元素。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/create-a-program-channel-1.png)

1. 按一下 **[!UICONTROL 標籤]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >為何選擇標籤？ 頻道是描述節目的一種方式，就像其他標籤一樣。 此頻道僅提供特殊的額外功能。

1. 按一下 **+** 在「 」旁邊簽署 [!UICONTROL 頻道] 以展開並檢視現有管道。

   ![](assets/create-a-program-channel-3.png)

1. 在 **[!UICONTROL 新增]**，按一下 **[!UICONTROL 新增頻道]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**範例**
   >
   >頻道：廣告牌
   >
   >* 套用至：預設
   >* 進度：成員、參與（如有疑問，這些功能可正常運作）
   >* 成功：參與
   >
   >頻道：派對
   >
   >* 套用至：事件
   >* 進度：已邀請、已註冊、無節目和已參加
   >* 成功：已出席
   >
   >檢視現有管道的進度，以瞭解如何使用它們。

1. 以派對頻道為例。 為您的新專案命名 **頻道** 並選取要套用的程式型別。

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >套用至什麼？ 有數種型別的計畫。 將管道與正確的型別配對。 如有疑問，請選擇 **[!UICONTROL 預設]**.

   >[!NOTE]
   >
   >使用&quot;[!UICONTROL 含網路研討會的事件]，」系統對應將會鎖定（如網路研討會整合所要求）且無法編輯。

1. 輸入前兩個程式「狀態」名稱，然後按一下 **[!UICONTROL 新增步驟]**.

   ![](assets/create-a-program-channel-6.png)

1. 輸入其他計畫 **[!UICONTROL 狀態]** 和 **[!UICONTROL 步驟]** 編號，然後按一下 **[!UICONTROL 新增步驟]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >此 **[!UICONTROL 步驟]** 編號用於排序程式狀態。 請記住，人們不能在這些循序漸進的步驟中後退。 他們只能將狀態變更為更高或相等的值狀態。 當狀態要來回切換而不是進度時，請使用相等值。

1. 輸入最後一個程式 **[!UICONTROL 狀態]** 和 **[!UICONTROL 步驟]** 數字。

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >使用型別&quot;[!UICONTROL 事件]，」需要已註冊、輪候和已出席狀態的系統對應。 因此，這些狀態無法隱藏。

1. 選取 **[!UICONTROL 行動簽到狀態]** 的 **[!UICONTROL 已註冊]**.

   ![](assets/create-a-program-channel-9.png)

1. 選取 **[!UICONTROL 行動簽到狀態]** 的 **[!UICONTROL 已出席]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**[!UICONTROL 行動簽到狀態]** 只有在頻道適用於活動方案時，選項才可使用。

   >[!NOTE]
   >
   >僅限擁有 **[!UICONTROL 行動簽到狀態]** 之 **[!UICONTROL 已註冊]** 和 **[!UICONTROL 已出席]** 將會顯示在 [行動簽到應用程式](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >如果在行動簽到應用程式中建立新人員，事件程式中會將其設為「已註冊」。 如果有人在應用程式上簽入事件，事件程式中的事件會設為「已參加」 。

1. 選取 **[!UICONTROL 成功]** 程式狀態，然後按一下 **[!UICONTROL 建立]**.

   ![](assets/create-a-program-channel-11.png)

   做得很好！ 當您製作該型別的新節目時，此新頻道將是選項之一。
