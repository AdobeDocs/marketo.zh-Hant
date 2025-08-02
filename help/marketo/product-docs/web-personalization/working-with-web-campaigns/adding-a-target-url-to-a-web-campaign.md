---
unique-page-id: 6094879
description: 將Target URL新增至網站行銷活動 — Marketo檔案 — 產品檔案
title: 新增目標URL至網站行銷活動
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 1%

---

# 新增目標URL至網站行銷活動 {#adding-a-target-url-to-a-web-campaign}

目標URL位於「設定行銷活動」頁面下方，並定義要顯示網頁行銷活動的特定URL。

## 新增Dialog或Widget Web行銷活動的目標URL {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. 移至&#x200B;**[!UICONTROL Web Campaigns]**。

   ![](assets/web-campaigns-hand-5.jpg)

1. 選擇「**[!UICONTROL Create New Web Campaign]**」。

   ![](assets/create-new-web-campaign-hand.jpg)

1. 新增&#x200B;**[!UICONTROL Campaign Name]**。 選取&#x200B;**[!UICONTROL Target Segment]**。 新增&#x200B;**[!UICONTROL Target URL]**。

   ![](assets/set-web-campaign-hands.jpg)

<table>
 <thead>
  <tr>
   <th colspan="1" rowspan="1">名稱</th>
   <th colspan="1" rowspan="1">說明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td colspan="1" rowspan="1"><strong>[!UICONTROL Any Page]</strong></td>
   <td colspan="1" rowspan="1"><p>允許行銷活動出現在任何頁面上。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL Include URL parameter when matching]</strong></p></td>
   <td colspan="1" rowspan="1">新增URL引數以在包含此引數的URL上比對和顯示促銷活動。 例如： campaign=cpc</td>
  </tr>
 </tbody>
</table>

## 新增多個URL至目標URL {#adding-multiple-urls-to-target-url}

按一下加號圖示(![—](assets/image2015-2-18-8-3a40-3a59.png))將會開啟[!UICONTROL Multiple Value Entry]對話方塊以新增多個URL。 每行新增一個URL。

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* 對話方塊和Widget網頁行銷活動可以使用任何頁面和萬用字元(&#42;)選項。
>* 在進階使用案例中，在區域中網路行銷活動可在URL路徑末端使用萬用字元。 範例： [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* URL區分大小寫

## 為區域網路行銷活動新增目標URL {#adding-a-target-url-for-in-zone-web-campaigns}

1. 移至&#x200B;**[!UICONTROL Web Campaigns]**。

   ![](assets/web-campaigns-hand-5.jpg)

1. 選擇「**[!UICONTROL Create New Web Campaign]**」。

   ![](assets/create-new-web-campaign-hand.jpg)

1. 新增&#x200B;**[!UICONTROL Campaign Name]**。 選取&#x200B;**[!UICONTROL Target Segment]**。 新增&#x200B;**[!UICONTROL Target URL]**。

   >[!NOTE]
   >
   >具有「在區域中」的目標URL必須定義一或多個URL。 在進階使用案例中，在區域中網路行銷活動可在URL路徑末端使用萬用字元。 範例： [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [建立對話方塊行銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [在區域行銷活動中建立RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [建立RTP Widget行銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
