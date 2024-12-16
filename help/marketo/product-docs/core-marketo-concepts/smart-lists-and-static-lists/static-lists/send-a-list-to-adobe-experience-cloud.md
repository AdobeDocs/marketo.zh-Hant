---
unique-page-id: 37356194
description: 傳送清單至Adobe Experience Cloud - Marketo檔案 — 產品檔案
title: 傳送清單至Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 1%

---

# 傳送清單至Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Marketo Engage執行個體的HIPAA就緒部署無法使用此功能。

>[!PREREQUISITES]
>
>[設定Adobe組織對應](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## 支援的目的地應用程式 {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (_僅限_&#x200B;如果您擁有Adobe Audience Manager授權)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## 如何傳送靜態清單 {#how-to-send-a-static-list}

靜態清單就是這樣、靜態。 除非您手動變更，否則Adobe Experience Cloud中的清單不會發生任何變更。

1. 在Marketo中，找到您要匯出的清單。 用滑鼠右鍵按一下並選取&#x200B;**[!UICONTROL 傳送至Experience Cloud]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. 按一下&#x200B;**[!UICONTROL Audience Manager資料夾]**&#x200B;下拉式清單，並在Experience Cloud中選取所要的目的地資料夾。

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. 選擇是建立新對象還是覆寫現有對象（在此範例中，我們正在建立新對象）。 輸入新的對象名稱，然後按一下&#x200B;**[!UICONTROL 傳送]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. 按一下&#x200B;**[!UICONTROL 「確定」]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >要完全填入Adobe，對象會籍最多可能需要6-8小時的時間。

## 如何傳送同步清單 {#how-to-send-a-synced-list}

同步清單表示只要您更新Marketo中的清單，該變更就會自動同步至其在Adobe Experience Cloud中的對象。

1. 在Marketo中，找到您要匯出的清單。 用滑鼠右鍵按一下並選取&#x200B;**[!UICONTROL 傳送至Experience Cloud]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. 按一下&#x200B;**[!UICONTROL 對象庫資料夾]**&#x200B;下拉式清單，並在Experience Cloud中選取所要的目的地資料夾。

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. 選擇是建立新對象還是覆寫現有對象（在此範例中，我們正在建立新對象）。 輸入新的對象名稱，核取&#x200B;**[!UICONTROL 保持同步的對象成員資格]**&#x200B;方塊，然後按一下&#x200B;**[!UICONTROL 傳送]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. 按一下&#x200B;**OK**。

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## 如何停止清單同步 {#how-to-stop-a-list-sync}

您可以隨時停止同步清單。

1. 在Marketo中，尋找並按一下右鍵您要停止同步的清單。 按一下&#x200B;**[!UICONTROL 停止清單同步]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. 選取要停止同步的對象並按一下&#x200B;**[!UICONTROL 停止]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. 按一下&#x200B;**[!UICONTROL 停止]**&#x200B;以確認。

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## 注意事項 {#things-to-note}

**共用至Adobe Analytics**

* 對於同時擁有Adobe Audience Manager和Adobe Analytics的客戶，此整合可讓對象從Marketo分享至您的Adobe Analytics報表套裝，不過，若要啟用此功能，必須在Adobe Audience Manager中執行一些額外的設定步驟。 請檢閱[Adobe Audience Manager的檔案](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html){target="_blank"}，以取得如何設定此專案的詳細資訊。

* 如果清單為空白，或沒有具有ECID值的使用者，系統不會推送清單名稱以在Marketo Engage外部參照。

**Adobe Audience Manager客戶的特徵使用情形**

當您在Marketo中啟動清單匯出時，您會注意到下列變更反映在您的Adobe Audience Manager執行個體中：

* 對於匯出清單中的所有人員，Marketo會使用其雜湊電子郵件作為跨裝置識別碼來撰寫特徵。 特徵名稱將會符合您在匯出期間指定的目的地對象名稱。
* 對於Marketo已設法與匯出清單中的人員相符的所有ECID，Marketo將使用ECID裝置識別碼來撰寫特徵。 特徵名稱將會符合您在匯出期間指定的目的地對象名稱。
* Marketo也將使用ECID特徵作為唯一的分段標準，在您的Audience Manager例項中建立區段。 區段的名稱將會符合您在匯出期間指定的目的地對象名稱。

## 常見問題集 {#faq}

**為什麼Marketo中的清單大小與Adobe中的清單大小不同？**

在不影響運作的情況下，受眾整合的運作方式是將Marketo Munchkin Cookie與對應的AdobeECID Cookie同步。 Marketo只能為Marketo已同步ECID的人員共用會籍資料。 為達到最佳效果，建議您在所有您想要追蹤的頁面上同時載入Marketo的munchkin.js追蹤指令碼和Adobe的visitor.js追蹤程式碼，以用於行銷目的。

**Cookie同步如何運作？**

為您的Marketo訂閱啟用Cookie同步後，Marketo的munchkin.js將嘗試為您在整合設定期間指定的Adobe IMS組織擷取和儲存AdobeECID，並將這些ECID比對至對應的Marketo Cookie識別碼。 這可讓Marketo的匿名使用者設定檔更加豐富AdobeECID。

還需要進一步步驟，將匿名使用者設定檔與人員設定檔建立關聯，該設定檔會使用純文字電子郵件識別。 [此處](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}說明此功能的確切運作方式。

**共用哪些資訊？**

此整合只會將Marketo的清單成員資格資訊分享給Adobe （例如，知道人員X是清單Y的成員）。 沒有其他人員屬性可透過此整合分享給Adobe。
