---
unique-page-id: 9437903
description: 建立自訂Dynamics同步篩選 — Marketo檔案 — 產品檔案
title: 建立自訂Dynamics同步篩選器
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
source-git-commit: ed4699ea4a94c787b8af109599f2a0c50591b956
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# 建立自訂Dynamics同步篩選器 {#create-a-custom-dynamics-sync-filter}

不想將Dynamics CRM中的所有項目同步至Marketo嗎？ 別擔心！ Marketo可讓您設定同步篩選器，並僅同步部分記錄。

## 概觀 {#overview}

要設定Dynamics同步篩選器，請執行以下操作：

1. 在您的Dynamics CRM中，為任何物件（銷售機會、連絡人、帳戶、商機和其他自訂實體）建立名為new_synctomkto的自訂兩個選項（布林值）欄位。
1. 為此欄位指派「是/否」值，或將其留空。

>[!NOTE]
>
>您必須在Dynamics CRM中進行這些變更，而不是在您的資料庫或Marketo中。

Marketo在自動背景同步期間會尋找此欄位，並根據此邏輯決定要同步的記錄：

| 欄位值 | 同步至Marketo? |
|---|---|
| 欄位不存在 | 是 |
| 欄位為空 | 是 |
| 欄位的值是 | 是 |
| 欄位的值為否 | 否 |

>[!CAUTION]
>
>要告訴Marketo略過記錄，唯一的方法是明確將欄位值設為 **否**. 即使欄位值空白，Marketo仍會同步記錄。

>[!PREREQUISITES]
>
>安裝最新版的Marketo外掛程式（3.0.0.1或更新版本）。 前往「Marketo >管理員> Microsoft Dynamics >下載Marketo解決方案」。

## 建立SyncToMkto欄位 {#create-synctomkto-field}

1. 登入Dynamics CRM。 按一下 **設定** 然後按一下 **自訂**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 按一下 **自訂系統**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 按一下 ![](assets/image2015-8-10-21-3a44-3a23.png) 下一頁 **實體**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 按一下 ![](assets/image2015-8-10-21-3a44-3a23.png) 下一頁 **銷售機會** 選取 **欄位**. 然後按一下 **新增**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. 輸入 **SyncToMkto** 在 **顯示名稱** 欄位和選取 **兩個選項** 作為 **資料類型**. 然後按一下 **儲存並關閉**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >為此欄位選擇任何顯示名稱，但「名稱」欄位必須準確 **new_synctomkto**. 您必須使用 **new** 作為預設首碼。 如果您已變更預設值，請前往此處， [重設自訂欄位名稱的預設首碼](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md). 建立新欄位後，您可以將其重新變更。

   >[!NOTE]
   >
   >如果您設定了非同步工作流，記錄將獲取您在欄位中設定的預設SyncToMkto值，並在工作流完成運行幾秒後獲取正確值。 如果預設值設為「是」，系統會在Marketo中建立這些記錄，然後過時。 使用 **否** 作為預設值，以避免此情況。

1. 重複此程式，並建立 **SyncToMkto** 欄位，用於您要限制同步的任何其他實體，如聯繫人、帳戶、機會和自定義實體。

## 在Marketo中選取篩選 {#select-the-filter-in-marketo}

即使您已完成初始同步，請移入並選取要與Marketo同步的欄位。

1. 前往「管理」並選取 **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **編輯** 在欄位同步詳細資訊上。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 實際名稱必須為new_synctomkto，但「顯示名稱」可以是任何值。 按一下 **儲存**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

很好，現在您已啟用Marketo的同步篩選器。

## 建立動態工作流以自動分配同步篩選值 {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

您始終可以手動為記錄的SyncToMkto欄位指定值。 但是，在建立或更新記錄時，為什麼不利用動態工作流的強大功能，自動將值分配給SyncToMkto欄位？

>[!NOTE]
>
>您無法在資料庫級別執行此操作。 您必須在CRM中手動或使用工作流程來完成此作業。
>
>動態工作流程僅適用於日後建立的新記錄，不適用於歷史資料。 使用批更新來移動現有記錄。

1. 轉至Dynamics CRM。 按一下 **設定** 然後按一下 **程式**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 按一下 **新增**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. 輸入工作流的名稱，然後選擇 **工作流程** 作為類別和 **銷售機會** 作為實體。 然後按一下 **確定**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 建立規則以指派true或false值至 **SyncToMkto** 欄位。 按一下 **儲存並關閉**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >在您按一下「 **新增步驟** 以新增「檢查條件」。 這會設定您不想同步的記錄 **否**. 否則，它們會同步。

1. 選取工作流程，然後按一下 **啟動**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >請參閱 [電子郵件地址的自訂同步篩選規則](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) 設定規則，僅同步具有電子郵件地址之人員的記錄。

## 同步篩選器詳細資訊 {#sync-filter-details}

以下是我們認為您應知道的實作詳細資料：

1. 啟動同步操作

   當 **SyncToMkto** 值從 **否** to **是**,Dynamics會立即通知Marketo以開始同步此記錄。 如果記錄已存在，Marketo會更新它。 否則，Marketo會建立記錄。

   >[!TIP]
   >
   >A `Create [StartSync]` 操作會新增至Marketo記錄。

1. 停止同步操作

   當記錄將其SyncToMkto值從「是」更改為「否」時，會通知Marketo停止同步此記錄。 但是記錄並未刪除，而是會停止收到更新，而變成過時。

>[!MORELIKETHIS]
>
>* [Microsoft Dynamics同步篩選器：合格](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Microsoft Dynamics同步篩選器：合併](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [電子郵件地址的自訂同步篩選規則](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

