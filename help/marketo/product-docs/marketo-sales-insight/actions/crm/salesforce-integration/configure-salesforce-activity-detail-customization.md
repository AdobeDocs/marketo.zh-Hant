---
description: 設定Salesforce活動詳細資料自訂 — Marketo檔案 — 產品檔案
title: 設定Salesforce活動詳細資料自訂
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# 設定Salesforce活動詳細資料自訂 {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce與Sales Insight動作 [必須連線](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* 透過API記錄電子郵件活動 [必須啟用](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)

活動詳細資料自訂可讓管理員設定當Salesforce分析動作活動/提醒任務同步到Salesforce時，將記錄到Salesforce任務 — 主題欄位的資訊。

>[!NOTE]
>
>* 如果您使用「 」，提醒任務的「銷售分析動作」中主題欄位所做的更新將會反映在對應Salesforce任務的主題欄位中 `{{activity_subject}}` 活動詳細資料自訂中的動態欄位。
>* 將資訊記錄到Salesforce主旨欄位時不支援分行符號。 更新銷售作業主旨時，會移除活動詳細資料自訂編輯器中的任何分行符號。

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

* 藉由自訂主旨欄位上顯示的資訊，Salesforce中的銷售人員可輕鬆掃描活動詳細資料。
* 管理員可以使用唯一識別碼（例如「Mkto_sales」）標籤主旨欄位，以便輕鬆識別銷售分析動作的活動，並與其他電子郵件活動、通話活動和任務區分開來。
* 減少自訂活動欄位的需求。 Salesforce會強制限制自訂活動欄位的數量，這會限制報表中可用的資料。 透過使用活動動態欄位將關鍵資料新增到主旨行，您可以減少需要在Salesforce執行個體中建立的自訂活動欄位數量。
* 活動和任務的主旨欄位將遵循銷售分析動作管理員定義的一致模式。

>[!NOTE]
>
>如果您將電子郵件回覆記錄為Salesforce的活動，則不會使用Salesforce活動詳細資料自訂設定。 他們將會以「回覆：電子郵件主旨」的形式記錄。

## 支援的活動動態欄位 {#activity-dynamic-fields-supported}

活動動態欄位會參考與銷售活動相關的資訊，以填入資料。 現在，它們可以與Salesforce活動詳細資料自訂一起使用。

>[!NOTE]
>
>如果沒有值可填入特定活動/任務的動態欄位，則在Salesforce任務 — 主題欄位更新時，不會填入該動態欄位的任何資料。

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

## 設定Salesforce活動詳細資料自訂 {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**需要管理員許可權。**

設定活動詳細資料時，請考慮在Salesforce中檢閱任務歷史記錄時，哪些資料與銷售最相關。

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. 按一下 **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. 按一下 **同步設定**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. 在活動詳細資料自訂編輯器中，新增您想要的任何任意任意文字。 您新增的文字為非動態，且同步至Salesforce的所有任務的主題欄位將維持不變。

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >雖然不一定要加上括弧，但如果將新增文字換成直括弧，有些人在Salesforce中的主旨欄位填入資料時，就能比較輕鬆地分辨資料。 範例： `[Sales Insight Actions] - {{Activity_type}}`

1. 按一下「 」，新增您想要的其他動態欄位 **新增動態欄位** 按鈕。

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. 選取所需的動態欄位。

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. 按一下 **儲存**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce強制使用255個字元的上限。 如果您的活動詳細資料超過此限制，則會截斷以確保資訊儲存在Salesforce主旨欄位中。

>[!MORELIKETHIS]
>
>* [將銷售活動同步至Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [提醒任務與Salesforce同步](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
