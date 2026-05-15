---
unique-page-id: 12983101
description: 瞭解如何將Facebook潛在客戶廣告自訂欄位對應至Marketo。 確保潛在客戶廣告資料對應至Marketo中的正確人員欄位。
title: 將自訂欄位對應至 Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
TQID: https://experienceleague.adobe.com/whJl1biZjBUAZp0w3kkmM5AplWTDXcV3-2KayHmsMnE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 6%

---

# 將自訂欄位對應至 Marketo {#map-custom-fields-to-marketo}

依預設，您可能想要收集超過標準資訊[!DNL Facebook]儲存的資訊，例如某人使用您的線上傳遞服務的頻率。 您可以透過[在您的[!DNL Facebook]潛在客戶廣告中建立自訂問題](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink)來完成此作業。

但是，**Marketo不會自動開始收集此資料**。 為了讓Marketo開始擷取自訂欄位值，您&#x200B;**必須**&#x200B;將這些自訂欄位對應到Marketo中的欄位。

請依照下列步驟，在Admin的LaunchPoint區域中設定此專案。

>[!NOTE]
>
>**需要管理員權限**

1. 移至[管理]區域並按一下&#x200B;**[!UICONTROL LaunchPoint]**。 在[已安裝服務]下，尋找並編輯&#x200B;**[!UICONTROL Facebook Lead Ads]**。

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. 將授權帳戶維持原狀，請&#x200B;**不**&#x200B;進行任何變更。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. 和以前一樣，將選取的頁面保持原樣，**不會**&#x200B;進行任何變更。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. 將自訂[!DNL Facebook]欄位對應到您的Marketo欄位。 按一下&#x200B;**[!UICONTROL Add].**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. 在新列中，輸入[!DNL Facebook]自訂欄位的名稱。

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >只有已儲存至[!DNL Facebook]表單範本的欄位才會在這裡顯示為選項。

1. 按一下&#x200B;**[!UICONTROL Marketo Field]**&#x200B;欄。 輸入以搜尋您要對應的欄位。 選取欄位後，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >如果您在Marketo中還沒有欄位可將[!DNL Facebook]欄位對應到，請瞭解如何[建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

>[!CAUTION]
>
>您&#x200B;**必須**&#x200B;針對任何新[!DNL Facebook]欄位進行此程式，以便Marketo收集資料。
