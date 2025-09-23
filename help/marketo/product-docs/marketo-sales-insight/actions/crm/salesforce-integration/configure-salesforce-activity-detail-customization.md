---
description: 設定Salesforce活動詳細資料自訂 — Marketo檔案 — 產品檔案
title: 設定 Salesforce 活動詳細資料自訂
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 2%

---

# 設定[!DNL Salesforce]活動詳細資料自訂 {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce和銷售Insight動作[必須連線](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* 必須啟用透過API [記錄電子郵件活動](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)

活動詳細資料自訂可讓管理員設定當[!DNL Salesforce]活動/提醒任務同步到[!DNL Sales Insight Actions]時，將記錄到[!DNL Salesforce]任務 — 主題欄位的資訊。

>[!NOTE]
>
>* 如果您在活動詳細資料自訂中使用[!DNL Sales Insight Actions]動態欄位，提醒任務[!DNL Salesforce]中主題欄位的更新將會反映在對應`{{activity_subject}}`任務的主題欄位中。
>* 將資訊記錄到[!DNL Salesforce]主旨欄位時不支援分行符號。 更新銷售作業主旨時，會移除活動詳細資料自訂編輯器中的任何分行符號。

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>InMail提醒工作</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>電子郵件活動</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>呼叫活動</td>
 </tr>
</table>

此功能可用來解鎖下列優點：

* 藉由自訂主旨欄位上顯示的資訊，在Salesforce中可輕鬆對銷售進行活動詳細資訊掃描。
* 管理員可以使用唯一識別碼（例如「Mkto_sales」）來標籤主旨欄位，以便輕鬆識別來自「銷售Insight動作」的活動，並與其他電子郵件活動、通話活動和任務區分開來。
* 減少自訂活動欄位的需求。 Salesforce會強制限制自訂活動欄位的數量，以限制可用於報表中的資料。 透過使用活動動態欄位將關鍵資料新增到主旨行，您可以減少在Salesforce執行個體中需要建立的自訂活動欄位數量。
* 活動和任務的主旨欄位將遵循銷售Insight動作管理員定義的一致模式。

>[!NOTE]
>
>如果您將電子郵件回覆記錄為[!DNL Salesforce]的活動，則不會使用[!DNL Salesforce]活動詳細資料自訂設定。 相反地，他們將會記錄為「回覆：電子郵件主旨」。

## 支援的活動動態欄位 {#activity-dynamic-fields-supported}

活動動態欄位會參考與銷售活動相關的資訊，以填入資料。 現在，它們可以與[!DNL Salesforce]活動詳細資料自訂一起使用。

>[!NOTE]
>
>如果沒有值可填入特定活動/任務的動態欄位，則當更新「Salesforce任務 — 主題欄位」時，不會填入該動態欄位的任何資料。

<table>
 <tr>
  <th>欄位</th>
  <th>說明</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>將會填入任務型別，如電子郵件、通話、InMail或自訂。</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>將填入任務的主旨。</p>
      <p>如果是電子郵件，則會填入電子郵件的主旨行。</p>
      <p>在呼叫、inMail或自訂的案例中，如果工作名稱/主旨欄位中有使用值建立的提醒工作，則會填入值。</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>如果活動是從銷售行銷活動起始，則會填入銷售行銷活動的名稱。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>如果活動是從銷售行銷活動起始，則會填入此活動發生的銷售行銷活動天數。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>如果活動是從銷售行銷活動起始，則會填入發生此活動之銷售行銷活動日期內的步驟編號。</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>如果活動是呼叫且已選取呼叫結果，則會填入呼叫結果值。</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>如果活動是來電且已選取來電原因，則會填入來電原因值。</td>
 </tr>
</table>

## 正在設定[!DNL Salesforce]活動詳細資料自訂 {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**需要系統管理員許可權。**

設定活動詳細資料時，請考慮在[!DNL Salesforce]中檢閱任務歷史記錄時，哪些資料與銷售最相關。

1. 按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. 按一下「**[!UICONTROL Salesforce]**」。

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. 按一下「**[!UICONTROL Sync Settings]**」。

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. 在活動詳細資料自訂編輯器中，新增您想要的任何任意任意文字。 您新增的文字為非動態文字，且同步至[!DNL Salesforce]的所有任務的主旨欄位將維持不變。

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >雖然並非必要，但以直括弧括住新增的文字，可讓某些人在資料填入[!DNL Salesforce]的主題欄位時，更輕鬆地辨別資料。 範例：`[Sales Insight Actions] - {{Activity_type}}`

1. 按一下&#x200B;**[!UICONTROL Add Dynamic Field]**&#x200B;按鈕，新增您想要的任何其他動態欄位。

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. 選取所需的動態欄位。

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>[!DNL Salesforce]強制使用255個字元的上限。 如果您的活動詳細資料超過此限制，則會截斷以確保資訊儲存在[!DNL Salesforce]主旨欄位中。

>[!MORELIKETHIS]
>
>* [將銷售活動同步至Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [提醒工作與Salesforce同步](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
