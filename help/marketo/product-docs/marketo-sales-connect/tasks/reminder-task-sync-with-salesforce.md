---
description: 提醒任務與Salesforce同步 — Marketo檔案 — 產品檔案
title: 提醒任務與Salesforce同步
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 與[!DNL Salesforce]同步處理提醒工作 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>若要瞭解如何啟用工作同步處理，請簽出[同步處理 [!DNL Sales Connect] 工作/提醒至 [!DNL Salesforce] 工作](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks)。

啟用工作同步設定後，使用者會看到他們的提醒工作與[!DNL Salesforce]雙向同步。 這表示使用者可以管理來自[!DNL Salesforce]或[!DNL Sales Connect]的工作，並確信系統將會保持一致。

## 提醒工作列位同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下是[!DNL Sales Connect]中的提醒工作列位清單，以及透過雙向任務同步支援的其對應的[!DNL Salesforce]欄位。

<table>
 <tr>
  <th>[!DNL Sales Connect] 工作列位</th>
  <th>[!DNL Salesforce] 工作列位</th>
  <th>[!DNL Salesforce] 任務</th>
 </tr>
 <tr>
  <td>[!UICONTROL Task Name]</td>
  <td>[!UICONTROL Subject Field]</td>
  <td>旨在顯示任務標題的簡短摘要欄位。</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status]</td>
  <td>[!UICONTROL Task Status]</td>
  <td><p>顯示工作的狀態。 [!DNL Sales Connect]個任務有兩個狀態，對應至[!DNL Salesforce]任務狀態選擇清單中的兩個值。</p>
  <p>在[!DNL Sales Connect]中開啟=未在[!DNL Salesforce]中啟動。</p>
  <p>完成於[!DNL Sales Connect] =完成於[!DNL Salesforce]。</p>
  <p>[!DNL Salesforce]中的其他狀態值將不會同步至[!DNL Sales Connect]。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Priority]</td>
  <td>[!UICONTROL Priority]</td>
  <td><p>[!DNL Sales Connect] 優先順序可以是「一般」或「高」，對應到[!DNL Salesforce]中的「一般」和「高」優先順序值。</p>
  <p>[!DNL Salesforce]中的低優先順序值將不會同步至[!DNL Sales Connect]。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Due Date]</td>
  <td>[!UICONTROL Due Date]</td>
  <td>任務的到期日。</td>
 </tr>
 <tr>
  <td>[!UICONTROL Details]</td>
  <td>[!UICONTROL Comments]</td>
  <td>顯示有關應該完成提醒工作的詳細資訊。</td>
 </tr>
</table>

## 第一次將[!DNL Sales Connect]個任務與[!DNL Salesforce]同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

當您首次開啟[!DNL Sales Connect]與[!DNL Salesforce]個任務之間的同步時，我們會匯入您的[!DNL Salesforce]個任務。 我們&#x200B;**不會**&#x200B;將您在[!DNL Sales Connect]中擁有的任何目前任務推播到[!DNL Salesforce]。 若要減少雜訊和重複專案，從[!DNL Sales Connect]同步到[!DNL Salesforce]的唯一工作是在您將&#x200B;*與SFDC同步*&#x200B;後[!DNL Sales Connect]建立的工作。

以下是當您同步[!DNL Sales Connect]和SFDC任務時發生的情況：

* 當您在同步處理任務時按一下「儲存」，任務就會開始進行同步處理。 這最初需要一些時間。

* 任何在過去24小時內已更新或建立的提醒將會從SFDC提取至[!DNL Sales Connect]。 同步是以到期日為基礎，所有這些工作都會在後端進行同步，但在指揮中心，您只會看到今天和明天到期的工作。

* 如果先前已開啟同步功能，而您又刪除了SFDC中的任何工作，則任何過去15天中刪除的工作都會從命令中心刪除。

* 只要同步處理已啟用，我們就會持續在[!DNL Sales Connect]和SFDC之間同步處理工作。

初次同步之後，您在[!DNL Sales Connect]中建立、編輯、完成或刪除的任何工作都會同步至[!DNL Salesforce]中的工作清單。 在[!DNL Salesforce]中建立、編輯、完成或刪除的任何專案都會在[!DNL Sales Connect]中更新您的任務清單。

若要開啟此同步，只要在Web應用程式的[設定頁面](https://toutapp.com/login)中勾選同步方塊即可。

>[!NOTE]
>
>若您在[!DNL Sales Connect]活動詳細資料自訂[!DNL Salesforce]設定中使用`{{activity_subject}}`動態欄位，則可在[中更新任務的主旨欄位，且此更新將會同步至對應同步任務的](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md)主旨欄位。 相反地，對[!DNL Salesforce]中主旨欄位所做的任何更新將&#x200B;_不會_&#x200B;同步到[!DNL Sales Connect]提醒任務主旨欄位。
