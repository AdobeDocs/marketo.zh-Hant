---
unique-page-id: 2950682
description: 建立方案管道 — Marketo檔案 — 產品檔案
title: 建立方案管道
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 3%

---

# 建立方案管道 {#create-a-program-channel}

方案是一個特定的行銷計畫。 此頻道旨在作為傳遞機制，例如網路研討會、贊助或線上廣告。

>[!NOTE]
>
>**需要管理員許可權**

>[!NOTE]
>
>深入瞭解Marketo中最重要的元素[程式](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/create-a-program-channel-1.png)

1. 按一下「**[!UICONTROL Tags]**」。

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >為何選擇標籤？ 頻道是描述節目的一種方式，就像其他標籤一樣。 此頻道僅提供特殊的額外功能。

1. 按一下「**」旁的「**+[!UICONTROL Channel]」符號以展開並檢視現有管道。

   ![](assets/create-a-program-channel-3.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;底下，按一下&#x200B;**[!UICONTROL New Channel]**。

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

1. 以派對頻道為例。 為您的新&#x200B;**[!UICONTROL Channel]**&#x200B;命名，並選取要套用的程式型別。

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >套用至什麼？ 有數種型別的計畫。 將管道與正確的型別配對。 如有疑問，請選擇&#x200B;**[!UICONTROL Default]**。

   >[!NOTE]
   >
   >使用「[!UICONTROL Event with Webinar]」時，系統將鎖定（根據網路研討會整合的需求）且無法編輯系統對應。

1. 輸入前兩個程式「狀態」名稱，然後按一下&#x200B;**[!UICONTROL Add Step]**。

   ![](assets/create-a-program-channel-6.png)

1. 輸入其他程式&#x200B;**[!UICONTROL Status]**&#x200B;和&#x200B;**[!UICONTROL Step]**&#x200B;號碼，然後按一下&#x200B;**[!UICONTROL Add Step]**。

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >**[!UICONTROL Step]**&#x200B;編號用於排序程式狀態。 請記住，人們不能在這些循序漸進的步驟中後退。 他們只能將狀態變更為更高或相等的值狀態。 當狀態要來回切換而不是進度時，請使用相等值。

1. 輸入最後一個程式&#x200B;**[!UICONTROL Status]**&#x200B;和&#x200B;**[!UICONTROL Step]**&#x200B;數字。

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >使用型別&quot;[!UICONTROL Event]&quot;時，需要系統對應至Registered、Waitlisted和Attended狀態。 因此，這些狀態無法隱藏。

1. 選取&#x200B;**[!UICONTROL Mobile Check-in Status]**&#x200B;的&#x200B;**[!UICONTROL Registered]**。

   ![](assets/create-a-program-channel-9.png)

1. 選取&#x200B;**[!UICONTROL Mobile Check-in Status]**&#x200B;的&#x200B;**[!UICONTROL Attended]**。

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >**[!UICONTROL Mobile Check-in Status]**&#x200B;選項只有在頻道將用於事件節目的情況下才可用。

   >[!NOTE]
   >
   >只有具有&#x200B;**[!UICONTROL Mobile Check-in Status]**&#x200B;個（共&#x200B;**[!UICONTROL Registered]**&#x200B;個）和&#x200B;**[!UICONTROL Attended]**&#x200B;的人，才會顯示在[行動簽入應用程式](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md)中。

   >[!TIP]
   >
   >如果在行動簽到應用程式中建立新人員，事件程式中會將其設為[!UICONTROL Registered]。 如果有人已簽入應用程式上的事件，事件程式中的事件會設為[!UICONTROL Attended]。

1. 選取&#x200B;**[!UICONTROL Success]**&#x200B;程式狀態，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/create-a-program-channel-11.png)

   做得很好！ 當您製作該型別的新節目時，此新頻道將是選項之一。
