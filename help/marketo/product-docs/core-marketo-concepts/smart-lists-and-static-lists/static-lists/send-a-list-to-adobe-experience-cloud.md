---
unique-page-id: 37356194
description: 傳送清單至Adobe Experience Cloud - Marketo檔案 — 產品檔案
title: 傳送清單至Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 1%

---

# 傳送清單至Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Marketo執行個體的HIPAA就緒部署無法使用此功能。

>[!PREREQUISITES]
>
>[設定Adobe組織對應](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## 支援的目的地應用程式 {#supported-destination-applications}

* Adobe Advertising Cloud
* ADOBE ANALYTICS (**僅限** 如果您擁有Adobe Audience Manager授權)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## 如何傳送靜態清單 {#how-to-send-a-static-list}

靜態清單就是這樣、靜態。 除非您手動進行變更，否則Adobe Experience Cloud中的清單不會有任何變更。

1. 在Marketo中，找到您要匯出的清單。 以滑鼠右鍵按一下並選取 **傳送至Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. 按一下 **Audience Manager資料夾** 下拉式清單，並在Experience Cloud中選取所需的目的地資料夾。

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. 選擇是建立新受眾還是覆寫現有受眾（在此範例中，我們正在建立新受眾）。 輸入新的對象名稱，然後按一下 **傳送**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. 按一下 **確定**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >完全填入Adobe中的對象成員資格最多可能需要6-8小時。

## 如何傳送同步清單 {#how-to-send-a-synced-list}

同步清單表示只要您更新Marketo中的清單，該變更就會自動同步至其在Adobe Experience Cloud中的對象。

1. 在Marketo中，找到您要匯出的清單。 以滑鼠右鍵按一下並選取 **傳送至Experience Cloud**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. 按一下 **對象庫資料夾** 下拉式清單，並在Experience Cloud中選取所需的目的地資料夾。

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. 選擇是建立新受眾還是覆寫現有受眾（在此範例中，我們正在建立新受眾）。 輸入新的對象名稱，核取 **讓對象成員資格保持同步** 方塊，然後按一下 **傳送**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. 按一下 **確定**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## 如何停止清單同步 {#how-to-stop-a-list-sync}

您可以隨時停止清單同步。

1. 在Marketo中，尋找並右鍵按一下您要停止同步的清單。 按一下 **停止清單同步**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. 選取您要停止同步的對象，然後按一下 **停止**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. 按一下 **停止** 以確認。

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## 注意事項 {#things-to-note}

**共用至Adobe Analytics**

對於同時擁有Adobe Audience Manager和Adobe Analytics的客戶，此整合可讓對象從Marketo分享至您的Adobe Analytics報表套裝，不過您需要在Adobe Audience Manager中執行一些額外的設定步驟才能啟用此功能。 請檢閱Adobe Audience Manager的檔案，以取得如何設定的詳細資訊： [https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Adobe Audience Manager客戶的特徵使用方式**

當您在Marketo中啟動清單匯出時，您會注意到下列變更反映在您的Adobe Audience Manager執行個體中：

* 對於匯出清單中的所有Lead，Marketo會使用Lead的雜湊電子郵件作為跨裝置識別碼來撰寫特徵。 特徵名稱將會符合您在匯出期間指定的目的地對象名稱。
* 對於Marketo已設法與匯出清單中的銷售機會相符的所有ECID，Marketo將使用ECID裝置識別碼來寫入特徵。 特徵名稱將會符合您在匯出期間指定的目的地對象名稱。
* Marketo也將使用ECID特徵作為唯一的分段標準，在您的Audience Manager例項中建立區段。 區段的名稱將會符合您在匯出期間指定的目的地對象名稱。

## 常見問題集 {#faq}

**Marketo中的清單大小為何與Adobe中的清單大小不同？**

在不影響運作的前提下，受眾整合的運作方式是將Marketo Munchkin Cookie與對應的AdobeECID Cookie同步。 Marketo只能為Marketo已同步ECID的潛在客戶共用成員資格資料。 為達到最佳效果，建議您在所有您想要追蹤的頁面上同時載入Marketo的munchkin.js追蹤指令碼和Adobe的visitor.js追蹤程式碼，以用於行銷目的。

**Cookie同步如何運作？**

為您的Marketo訂閱啟用Cookie同步後，Marketo的munchkin.js將嘗試為您在整合設定期間指定的Adobe IMS組織擷取和儲存AdobeECID，並將這些ECID比對至對應的Marketo Cookie識別碼。 這可讓Marketo的匿名使用者設定檔更豐富AdobeECID。

還需要執行另一個步驟，將匿名使用者設定檔與潛在客戶設定檔建立關聯（使用純文字電子郵件識別）。 這是如何運作 [在此說明](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**會共用哪些資訊？**

此整合只會將清單成員資格資訊從Marketo分享到Adobe （例如，知道銷售機會X是清單Y的成員）。 不會透過此整合將其他銷售機會屬性共用給Adobe。
