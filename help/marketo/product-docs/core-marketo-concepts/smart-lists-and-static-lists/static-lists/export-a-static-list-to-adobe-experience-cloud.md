---
unique-page-id: 37356194
description: 將靜態清單匯出至Adobe Experience Cloud —— 行銷人員檔案——產品檔案
title: 將靜態清單匯出至Adobe Experience Cloud
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---


# 將靜態清單匯出至Adobe Experience Cloud {#export-a-static-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Marketo例項的HIPAA適用部署無法使用此功能。

>[!PREREQUISITES]
>
>[設定Adobe Experience Cloud觀眾共用](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## 支援的目標應用程式{#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics（如果您擁有Adobe Audience Manager授權，則僅限&#x200B;****）
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe即時客戶資料平台
* Adobe Target

## 如何導出清單{#how-to-export-a-list}

1. 在Marketo中，尋找並選取您要匯出的清單。

   ![](assets/one.png)

1. 按一下「清單動作&#x200B;**」下拉式清單，並選取「傳送至Experience Cloud」**。****

   ![](assets/two-1.png)

1. 按一下「Audience Manager資料夾」下拉式清單，然後在Experience Cloud中選取所需的目標資料夾。****

   ![](assets/three-1.png)

1. 選擇要建立新對象或覆寫現有對象（在此範例中，我們要建立新對象）。 輸入新的對象名稱，然後按一下「傳送&#x200B;**」。**

   ![](assets/four.png)

1. 按一下&#x200B;**確定**。

   ![](assets/five.png)

   >[!NOTE]
   >
   >觀眾會籍最多需要6-8小時，才能完整填入Adobe。

## 注意事項{#things-to-note}

**共用至Adobe Analytics**

對於同時擁有Adobe Audience Manager和Adobe Analytics的客戶，此整合可讓觀眾從Market共用至您的Adobe Analytics報表套裝，但是Adobe Audience Manager中需要執行一些額外的設定步驟，以啟用此功能。 請參閱Adobe Audience Manager檔案，以取得如何設定此設定的詳細資訊：[https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html)。

**Adobe Audience Manager客戶的特徵使用**

當您在Marketo中啟動清單匯出時，您會注意到Adobe Audience Manager例項中反映的下列變更：

* 對於匯出清單中的所有Lead,Marketo會使用Leads的雜湊電子郵件作為跨裝置識別碼來編寫特徵。 特徵的名稱將符合您在匯出期間指定的目標對象名稱。
* 對於Marketo已設法符合匯出清單中銷售機會的所有ECID,Marketo會使用ECID裝置識別碼來編寫特徵。 特徵的名稱將符合您在匯出期間指定的目標對象名稱。
* Marketo也會在您的Audience Manager例項中，以ECID特性作為唯一的分段標準來建立區段。 區段的名稱將符合您在匯出期間指定的目標對象名稱。

## 常見問答{#faq}

**為何Marketo中的清單大小與Adobe中的清單大小不同？**

在The Hood下，觀眾整合可借由同步Marketo Munchkin Cookie與對應的Adobe ECID Cookie來運作。 Marketo只能分享Marketo為之同步ECID之潛在客源的會籍資料。 為獲得最佳結果，建議您在所有想要追蹤以用於行銷目的的頁面上，同時載入Marketo的munchkin.js追蹤指令碼和Adobe的visitor.js追蹤代碼。

**Cookie如何同步？**

當您的Marketo訂閱啟用Cookie同步時，Marketo的munchkin.js會嘗試擷取並儲存您在整合設定期間指定之Adobe IMS組織的Adobe ECID，並將這些ECID與對應的Marketo Cookie識別碼相符。 這可讓Marketo的匿名使用者個人檔案充份運用Adobe ECID。

需要進一步步驟，將匿名用戶配置檔案與使用純文字檔案電子郵件標識的銷售線索配置檔案關聯。 具體說明如下：[https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People](https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People)。
