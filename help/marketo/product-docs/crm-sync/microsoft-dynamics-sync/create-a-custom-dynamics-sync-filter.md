---
unique-page-id: 9437903
description: 建立自訂 [!DNL Dynamics] 同步篩選器 — Marketo檔案 — 產品檔案
title: 建立自訂 [!DNL Dynamics] 同步篩選器
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 建立自訂[!DNL Dynamics]同步篩選器 {#create-a-custom-dynamics-sync-filter}

不想將您Dynamics CRM中的所有專案同步至Marketo Engage嗎？ 別擔心！ Marketo可讓您設定同步篩選器，並僅同步部分記錄。

## 概觀 {#overview}

若要設定[!DNL Dynamics]同步篩選器：

1. 在您的Dynamics CRM中，為任何物件（銷售機會、連絡人、帳戶、機會和其他自訂實體）建立名為new_synctomkto的自訂兩個選項（布林值）欄位。
1. 將此欄位指定為「是/否」值。

您必須在Dynamics CRM (而非您的資料庫或Marketo)中進行這些變更。

>[!CAUTION]
>
>如果您未指派欄位並保留空白/NULL，它將會同步但不會更新。 Dynamics CRM中欄位值為空白/空的記錄在Marketo中會顯示為「false」。

Marketo在自動背景同步期間會尋找此欄位，並根據此邏輯決定要同步處理的記錄：

| 欄位值 | 同步至Marketo？ |
|---|---|
| 欄位不存在 | 是 |
| 欄位是空的 | 是 |
| 欄位的值為「是」 | 是 |
| 欄位的值否 | 無 |

>[!CAUTION]
>
>告知Marketo跳過記錄的唯一方法是明確將欄位值設為&#x200B;**否**。 即使欄位值為空，Marketo仍會透過同步記錄。

>[!PREREQUISITES]
>
>安裝最新版的Marketo外掛程式（3.0.0.1或更新版本）。 前往Marketo > [!UICONTROL Admin] > [!DNL Microsoft Dynamics] > [!UICONTROL Download Marketo Solution]。

## 建立SyncToMkto欄位 {#create-synctomkto-field}

1. 登入您的Dynamics CRM。 按一下&#x200B;**設定**，然後按一下&#x200B;**自訂**。

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 按一下「**[!UICONTROL Customize the System]**」。

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 按一下![](assets/image2015-8-10-21-3a44-3a23.png)旁的&#x200B;**[!UICONTROL Entities]**。

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 按一下![](assets/image2015-8-10-21-3a44-3a23.png)旁的&#x200B;**[!UICONTROL Lead]**&#x200B;並選取&#x200B;**[!UICONTROL Fields]**。 然後按一下「**[!UICONTROL New]**」。

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. 在&#x200B;**欄位中輸入** SyncToMkto **[!UICONTROL Display Name]**，並選取&#x200B;**[!UICONTROL Two Options]**&#x200B;做為&#x200B;**[!UICONTROL Data Type]**。 然後按一下「**[!UICONTROL Save and Close]**」。

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >選擇此欄位的任何顯示名稱，但[名稱]欄位必須剛好是&#x200B;**new_synctomkto**。 您必須使用&#x200B;**new**&#x200B;做為預設首碼。 如果您已變更預設值，請前往這裡[重設自訂欄位名稱的預設首碼](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}。 您可以在建立新欄位後將其變更回。

   >[!NOTE]
   >
   >如果您設定了非同步工作流程，記錄會取得您在欄位中設定的預設SyncToMkto值，並在工作流程完成執行時幾秒後取得正確值。 若預設值設為「是」，這些記錄將會在Marketo中建立，然後過時。 使用&#x200B;**否**&#x200B;作為預設值以避免此情況。

1. 重複此程式，並為您想要限制同步的任何其他實體（例如連絡人、帳戶、機會和自訂實體）建立&#x200B;**SyncToMkto**&#x200B;欄位。

## 在Marketo中選取篩選器 {#select-the-filter-in-marketo}

即使您已完成初始同步，請前往並選取要與Marketo同步的欄位。

1. 移至[管理]並選取&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 按一下[欄位同步處理詳細資料]上的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下捲動至欄位並進行核取。 實際名稱必須是new_synctomkto，但「顯示名稱」可以是任何內容。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2015-10-9-9-3a56-3a23.png)

太好了，現在您已啟用Marketo的同步篩選器。

## 建立[!DNL Dynamics]工作流程以自動指派同步篩選器值 {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

您一律可以手動將值指派給記錄的SyncToMkto欄位。 但是為什麼不利用[!DNL Dynamics]工作流程的強大功能，在建立或更新記錄時自動指派值給SyncToMkto欄位？

>[!NOTE]
>
>您無法在資料庫層級執行此動作。 這必須在CRM中手動或使用工作流程完成。
>
>[!DNL Dynamics]工作流程僅適用於未來建立的新記錄，不適用於歷史資料。 使用批次更新來移動現有記錄。

1. 前往您的Dynamics CRM。 按一下&#x200B;**設定**，然後按一下&#x200B;**處理序**。

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 按一下「**[!UICONTROL New]**」。

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. 輸入工作流程的名稱，並選取&#x200B;**[!UICONTROL Workflow]**&#x200B;作為[!UICONTROL Category]，**[!UICONTROL Lead]**&#x200B;作為[!UICONTROL Entity]。 然後按一下&#x200B;**確定**。

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 根據您組織的偏好設定建立規則以將true或false值指派給&#x200B;**SyncToMkto**&#x200B;欄位。 按一下「**[!UICONTROL Save and Close]**」。

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >按一下&#x200B;**[!UICONTROL Add Step]**&#x200B;以新增檢查條件後，定義預設動作。 這會設定您不想要同步處理至&#x200B;**否**&#x200B;的記錄。 否則，它們將會同步。

1. 選取工作流程並按一下&#x200B;**[!UICONTROL Activate]**。

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >請參閱電子郵件地址的[自訂同步篩選規則](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}，以設定僅同步具有電子郵件地址之人員的記錄的規則。

## 同步篩選器詳細資訊 {#sync-filter-details}

以下是一些我們認為您應知道的實作詳細資料：

* 啟動同步作業

  當&#x200B;**SyncToMkto**&#x200B;值從&#x200B;**No**&#x200B;變更為&#x200B;**Yes**&#x200B;時，[!DNL Dynamics]會立即通知Marketo開始同步處理此記錄。 如果記錄已經存在，Marketo會更新它。 否則，Marketo會建立記錄。

  >[!TIP]
  >
  >發生此情況時，`Create [StartSync]`作業會新增至Marketo記錄檔。

* 停止同步作業

  當記錄的SyncToMkto值從「是」變更為「否」時，Marketo會收到停止同步處理此記錄的通知。 但記錄不會刪除，而是會停止取得更新並過時。

>[!MORELIKETHIS]
>
>* [Microsoft Dynamics同步篩選器：合格](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Microsoft Dynamics同步篩選器：合併](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [電子郵件地址的自訂同步篩選規則](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
