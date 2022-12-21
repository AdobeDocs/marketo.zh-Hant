---
description: 設定Salesforce活動詳細資訊自訂 — Marketo檔案 — 產品檔案
title: 配置Salesforce活動詳細資訊定制
hide: true
hidefromtoc: true
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
source-git-commit: 43878490538ad5485c9e6d7aa0c7f8f1b443ad8c
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# 配置Salesforce活動詳細資訊定制 {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce和Sales Insight Actions [必須已連接](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* 透過API記錄電子郵件活動 [必須啟用](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)


「活動詳細資訊定制」允許管理員配置當將Sales Insight Actions活動/提醒任務同步到Salesforce時，將登錄到「Salesforce任務 — 主題」欄位的資訊。

>[!NOTE]
>
>* 對提醒任務的「銷售分析活動」主題欄位所做的更新將反映在相應的Salesforce任務的主題欄位中(如果您使用 `{{activity_subject}}` 「活動詳細資料自訂」中的「動態」欄位。
>* 將資訊記錄到Salesforce主題欄位時不支援分行。 更新銷售任務主體時，「活動詳細資訊自訂」編輯器中的任何分行將被刪除。


![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>InMail提醒任務</td>
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

* 透過自訂主題欄位上可見的資訊，在Salesforce中可輕鬆掃描活動詳細資訊以供銷售。
* 管理員可以使用唯一識別碼（例如「Mkto_sales」）標籤主旨欄位，以便輕鬆識別「銷售分析動作」中的活動，並區別於其他電子郵件活動、呼叫活動和任務。
* 減少對自訂活動欄位的需求。 Salesforce會對自訂活動欄位的數量強制執行限制，而自訂活動欄位可限制可用於報表的資料。 使用活動動態欄位將關鍵資料新增至主旨行，可減少您在Salesforce例項中建立的自訂活動欄位數。
* 活動和任務的主題欄位將遵循Sales Insight Actions Admin定義的一致模式。

>[!NOTE]
>
>如果您將電子郵件回覆記錄為Salesforce的活動，則它們將不使用Salesforce活動詳細資訊自訂設定。 改為會以「回覆：電子郵件主旨。」

## 支援的活動動態欄位 {#activity-dynamic-fields-supported}

活動動態欄位參考有關要填入資料的銷售活動的資訊。 現在，它們可與Salesforce活動詳細資訊自訂搭配使用。

>[!NOTE]
>
>如果沒有值可為特定活動/任務填入動態欄位，則更新Salesforce任務 — 主體欄位時，它將不會為該動態欄位填入任何資料。

<table>
 <tr>
  <th>欄位</th>
  <th>說明</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>會將任務類型填入為「電子郵件」、「呼叫」、「InMail」或「自訂」。</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>將填入任務的主題。</p>
      <p>若是電子郵件，則會填入電子郵件的主旨行。</p>
      <p>如果是呼叫、inMail或自訂，如果在任務名稱/主旨欄位中建立了提醒任務，則會填入值。</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>如果活動是從銷售促銷活動起始的，則會填入銷售促銷活動的名稱。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>如果活動是從銷售促銷活動起始的，它將填入此活動發生的銷售促銷活動日期編號。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>如果活動是從銷售促銷活動起始的，它將在發生此活動的銷售促銷活動日期內填入步驟號。</td>
 </tr>
 <tr>
  <td>{{call_out}}</td>
  <td>如果活動是呼叫，且選取了呼叫結果，則會填入呼叫結果值。</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>如果活動是呼叫，且選取了呼叫原因，則會填入呼叫原因值。</td>
 </tr>
</table>

## 配置Salesforce活動詳細資訊定制 {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**需要管理員權限。**

在設定活動詳細資訊時，請在檢閱Salesforce中的任務歷史記錄時，考慮哪些資料與銷售最相關。

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. 按一下 **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. 按一下 **同步設定**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. 在「活動詳細資訊自訂」編輯器中，新增您想要的任何自由文字。 您新增的文字非動態，且同步至Salesforce之所有工作的主旨欄位將維持不變。

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >雖然不需要，但將新增的文字以直方括弧括住，可讓某些人在資料填入至Salesforce中的主旨欄位時，更輕鬆地在資料之間進行辨識。 範例： `[Sales Insight Actions] - {{Activity_type}}`

1. 按一下 **新增動態欄位** 按鈕。

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. 選取所需的動態欄位。

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. 按一下 **儲存**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce可強制執行255個字元的限制。 如果活動詳細資訊超過此值，則會截斷，以確保資訊儲存在Salesforce主題欄位中。

>[!MORELIKETHIS]
>
>* [同步設定](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [與Salesforce的提醒任務同步](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)

