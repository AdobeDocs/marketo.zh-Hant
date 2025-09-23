---
description: 傳送清單至廣告網路 — Marketo檔案 — 產品檔案
title: 傳送清單至廣告網路
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 8%

---

# 傳送清單至廣告網路 {#send-a-list-to-an-ad-network}

瞭解如何將靜態清單傳送至[!DNL LinkedIn]、[!DNL Facebook]或Google。

## 如何傳送清單 {#how-to-send-a-list}

1. 在Marketo中，選取您的清單，按一下&#x200B;**[!UICONTROL List Actions]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL Send to Ad Network]**。

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. 在[!DNL LinkedIn]、[!DNL Facebook]或Google （其他選專案前無法使用）之間選擇。 在此範例中，我們選擇&#x200B;**[!DNL LinkedIn]**。 按一下「**[!UICONTROL Next]**」。

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. 按一下&#x200B;**[!UICONTROL Audience]**&#x200B;下拉式清單，然後選取您想要的對象。

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >如果您需要檢查，可以透過「狀態」標籤檢視清單同步到的目標對象。

1. 選擇您想要的[!UICONTROL Push Type]並按一下&#x200B;**[!UICONTROL Update]**。

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >如果您選取「[!UICONTROL Enable continuous audience sync]」，Marketo會在您的Marketo執行個體中清單變更時，保持所選廣告網路中的清單為最新。 我們都會新增&#x200B;**和**&#x200B;人員，如果他們是從靜態清單中新增或移除的，則會從對象中移除這些人員。

1. 就是這樣！ 按一下&#x200B;**[!UICONTROL OK]**&#x200B;結束。

   ![](assets/send-a-list-to-an-ad-network-5.png)

## 常見問題 {#faq}

**單一靜態清單可以與多個廣告對象同步嗎？**

否，清單只能同步至單一目的地對象。

**如果我啟用與現有廣告對象的連續同步，是否會取代現有對象？**

否，現有對象將會新增至，而非取代。
