---
unique-page-id: 9437903
description: 建立自訂動態同步篩選——行銷檔案——產品檔案
title: 建立自訂動態同步篩選
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---


# 建立自訂動態同步篩選 {#create-a-custom-dynamics-sync-filter}

您不想將Dynamics CRM中的一切同步到Marketo嗎？ 別擔心！ Marketo可讓您設定同步篩選，並僅同步部分記錄。

## 概觀 {#overview}

若要設定動態同步篩選：

1. 在Dynamics CRM中為任何物件（銷售機會、連絡人、帳戶、業務機會和其他自訂實體）建立名為new_synctomkto的自訂「兩個選項」（布林值）欄位。
1. 將此欄位指定為「是／否」值，或將其留空。

>[!NOTE]
>
>您必須在Dynamics CRM中進行這些變更，而不是在您的資料庫或Marketo中進行。

Marketo會在自動背景同步期間尋找此欄位，並根據此邏輯判斷要同步的記錄：

| 欄位值 | 與Marketo同步？ |
|---|---|
| 欄位不存在 | 是 |
| 欄位為空 | 是 |
| 欄位有值是 | 是 |
| 欄位的值為否 | 否 |

>[!CAUTION]
>
>告訴Market要略過記錄的唯一方法，就是將欄位值明確設為 **否**。 即使欄位值空白，Marketo仍會同步記錄。

>[!PREREQUISITES]
>
>安裝最新版的Marketo外掛程式（3.0.0.1或更新版本）。 前往「行銷人員>管理員> Microsoft Dynamics >下載行銷人員解決方案」。

## 建立SyncToMkto欄位 {#create-synctomkto-field}

1. 登入Dynamics CRM。 按一 **下「設定** 」，然後按一 **下「自訂」**。

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 按一下 **自定義系統**。

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 按一下 ![](assets/image2015-8-10-21-3a44-3a23.png) 「實體」( **Entities)旁邊**。

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 按一 ![](assets/image2015-8-10-21-3a44-3a23.png) 下「**銷售機會**」旁，然後選取「欄 **位」**。 然後按一 **下新**。

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. 在「顯 **示名稱****」欄位中輸入SyncToMkto，並選** 擇兩個選項 **，作為Data Type****** Chandit。 然後按一 **下儲存並關閉**。

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >為此欄位選擇任何顯示名稱，但「名稱」欄位必須完全 **是new_synctomkto**。 您必須使 **用** new作為預設首碼。 如果您已變更預設值，請前往此處 [重設自訂欄位名稱的預設首碼](create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md)。 在建立新欄位後，您可以重新變更欄位。

   >[!NOTE]
   >
   >如果您已設定非同步工作流程，記錄會取得您在欄位中設定的預設SyncToMkto值，並在工作流程完成執行幾秒後取得正確值。 如果預設值設為「是」，這些記錄會在Marketto中建立，然後變成過時。 請使 **用** 「否」作為預設值以避免此情況。

1. 重複此過程，並為您希望限制同步的其他實體（如聯繫人、帳戶、業務機會和自定義實體）建立 **SyncToMkto** 欄位。

## 在Marketo中選取篩選 {#select-the-filter-in-marketo}

即使您已完成初始同步，請移至並選取要與Marketo同步的欄位。

1. 前往「管理員」並選取「 **MiCrosoft Dynamics」**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下 **欄位同步** 「詳細資訊」上的「編輯」。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並加以檢查。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下 **儲存**。

   ![](assets/image2015-10-9-9-3a56-3a23.png)

很好，現在您已啟用Marketo的同步篩選。

## 建立動態工作流程以自動指派同步篩選值 {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

您始終可以手動為記錄的SyncToMkto欄位指定值。 但是，在建立或更新記錄時，為什麼不利用動態工作流的強大功能並自動為SyncToMkto欄位指定值？

>[!NOTE]
>
>不能在資料庫級別執行此操作。 必須在CRM中手動或使用工作流程來完成。
>
>「動態」工作流程僅適用於日後建立的新記錄，而不適用於歷史資料。 使用批更新來移動現有記錄。

1. 前往Dynamics CRM。 按一 **下「設定** 」，然後按 **一下「流程**」。

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 按一 **下新**。

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. 輸入工作流的名稱，然後選擇「工 **作流** 」作為類別， **「銷售線索** 」作為實體。 然後按一 **下確定**。

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 建立規則，以根據您組織的偏好設定，為 **SyncToMkto** 欄位指派真或假值。 按一 **下儲存並關閉**。

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >在按一下「新增步驟」以新增「檢查條 **件」後** ，定義預設動作。 這會將您不想同步的記錄設定為 **否**。 否則，它們會同步。

1. 選擇工作流，然後按一下「 **激活」**。

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >請參 [閱電子郵件地址的自訂同步篩選規則](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) ，以設定規則，僅同步具有電子郵件地址之人員的記錄。

## 同步篩選詳細資訊 {#sync-filter-details}

以下是我們認為您應該知道的一些實施詳細資訊：

1. 啟動同步操作

   當 **SyncToMkto值從「否****」變更為「是」** 時 ****,Dynamics會通知Market以立即開始同步此記錄。 如果記錄已存在，Marketo會更新記錄。 否則，Marketo會建立記錄。

   >[!TIP]
   >
   >當發 **生此 [情況時，Create]** StartSync操作會新增至Marketo Log。

1. 停止同步操作

   當記錄將其SyncToMkto值從「是」變更為「否」時，Marketo會收到通知，以停止同步此記錄。 但是，該記錄並未刪除，而是會停止收到更新並變成過時。

>[!NOTE]
>
>**相關文章**
>
>* [Microsoft Dynamics Sync篩選器：符合資格](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Microsoft Dynamics Sync篩選器：合併](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [電子郵件地址的自訂同步篩選規則](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

>



