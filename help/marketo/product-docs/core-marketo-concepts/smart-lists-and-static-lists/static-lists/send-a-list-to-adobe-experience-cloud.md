---
unique-page-id: 37356194
description: 將清單發送到Adobe Experience Cloud-Marketo文檔 — 產品文檔
title: 將清單發送到Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
source-git-commit: a82a2dd0a9c3a27b9b6bf3b352cd81d59932a31b
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 將清單發送到Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Marketo實例的HIPAA就緒部署無法使用此功能。

>[!PREREQUISITES]
>
>[設定Adobe Experience Cloud觀眾共用](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## 支援的目標應用程式 {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics **僅** 如果你有Adobe Audience Manager執照)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## 如何發送靜態清單 {#how-to-send-a-static-list}

靜態清單就是靜態的。 除非您手動進行更改，否則不會對Adobe Experience Cloud的清單進行任何更改。

1. 在Marketo，找到要導出的清單。 按一下右鍵它並選擇 **發送到Experience Cloud**。

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. 按一下 **Audience Manager資料夾** 下拉並選擇Experience Cloud中所需的目標資料夾。

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. 選擇是建立新受眾還是覆蓋現有受眾（在本示例中，我們正在建立新受眾）。 輸入新受眾名稱，然後按一下 **發送**。

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. 按一下 **確定**。

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >觀眾會員在Adobe中完全填充可能需要6到8個小時。

## 如何發送同步清單 {#how-to-send-a-synced-list}

同步清單意味著，只要您在Marketo更新清單，該更改將自動同步到Adobe Experience Cloud的受眾。

1. 在Marketo，找到要導出的清單。 按一下右鍵它並選擇 **發送到Experience Cloud**。

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. 按一下 **訪問群體庫資料夾** 下拉並選擇Experience Cloud中所需的目標資料夾。

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. 選擇是建立新受眾還是覆蓋現有受眾（在本示例中，我們正在建立新受眾）。 輸入新受眾名稱，檢查 **保持受眾成員身份同步** 框，然後按一下 **發送**。

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. 按一下 **確定**。

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## 如何停止清單同步 {#how-to-stop-a-list-sync}

您可以隨時停止同步清單。

1. 在Marketo，查找並按一下右鍵要停止同步的清單。 按一下 **停止清單同步**。

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. 選擇要停止同步的受眾，然後按一下 **停止**。

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. 按一下 **停止** 確認。

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## 要注意的事項 {#things-to-note}

**與Adobe Analytics共用**

對於同時擁有Adobe Audience Manager和Adobe Analytics的客戶，此整合將使受眾能夠從Marketo共用到您的Adobe Analytics報告套件，但是，在Adobe Audience Manager需要執行一些其他配置步驟來實現此功能。 請查閱Adobe Audience Manager的文檔，瞭解有關如何設定此設定的詳細資訊： [https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html)。

**Adobe Audience Manager客戶的特性使用**

在Marketo啟動清單導出時，您會注意到Adobe Audience Manager實例中反映的以下更改：

* 對於導出清單中的所有Lead,Marketo將使用Leads的散列電子郵件作為跨設備標識符來寫一個特性。 特性的名稱將與導出期間指定的目標受眾名稱匹配。
* 對於Marketo已設法與導出清單中的Lead匹配的所有ECID,Marketo將使用ECID設備標識符編寫一個特性。 特性的名稱將與導出期間指定的目標受眾名稱匹配。
* Marketo還將在您的Audience Manager實例中使用ECID特性作為唯一分割標準建立段。 段的名稱將與導出期間指定的目標受眾名稱匹配。

## 常見問題 {#faq}

**為什麼Marketo的名單大小與Adobe的名單大小不同？**

在引擎蓋下，通過將Marketo·蒙奇金Cookie與相應的AdobeECID Cookie同步，使受眾整合工作。 Marketo只能共用Marketo已同步ECID的線索的成員資格資料。 為獲得最佳結果，建議您將Marketo的munchkin.js跟蹤指令碼與Adobe的visitor.js跟蹤代碼並行載入到您感興趣的所有頁面上，以用於營銷目的。

**Cookie同步如何工作？**

為您的Marketo訂閱啟用cookie同步後，Marketo的munchkin.js將嘗試捕獲和儲存在整合設定期間指定的Adobe IMS組織的AdobeECID，並將這些ECID與相應的Marketocookie標識符匹配。 這使Marketo的匿名用戶配置檔案能夠用AdobeECID豐富。

還需要進一步步驟將匿名用戶配置檔案與使用純文字檔案電子郵件標識的潛在客戶配置檔案相關聯。 這是怎麼運作的 [此處](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)。

**共用了哪些資訊？**

這種整合僅分享從Marketo到Adobe的名單成員資訊（例如，Lead X是List Y成員的知識）。 沒有通過此整合將其他Lead屬性共用給Adobe。
