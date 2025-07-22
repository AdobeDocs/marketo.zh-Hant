---
unique-page-id: 10096683
description: ON24事件註冊更新 — Marketo檔案 — 產品檔案
title: ON24事件註冊更新
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# ON24事件註冊更新 {#on-event-registration-updates}

## 手動核准註冊者 {#manually-approving-registrants}

您可以在傳送確認電子郵件給註冊者之前，手動核准他們。 若要這麼做，您將需要設定行銷活動以處理此額外步驟：

1. 針對註冊觸發程式行銷活動：

   * 在[!UICONTROL Smart List]中，將觸發器設定為&#x200B;**[!UICONTROL Fills Out Form]**。
   * 在流程中，將[!UICONTROL Status in Progression]設定為&#x200B;**[!UICONTROL Pending Approval]**。

1. 前往事件並按一下&#x200B;**[!UICONTROL Members]**&#x200B;標籤。 此索引標籤會顯示所有已填寫表單的人。 其狀態應設為&#x200B;**[!UICONTROL Pending Approval]**。
1. 使用格線頂端的篩選器，只檢視狀態為&#x200B;**[!UICONTROL Pending Approval]**&#x200B;的人員。
1. 選取您要註冊的人員（按住Shift鍵並按一下、按住Control鍵並按一下，或選取全部）。
1. 在功能表中按一下&#x200B;**[!UICONTROL Change Status]**。 選取「**[!UICONTROL Registered]**」、「**[!UICONTROL Rejected]**」或任何其他適用的狀態。

## 處理發生註冊錯誤的人員 {#handling-people-with-a-registration-error}

如果人員最後並未註冊，而是設定為狀態[!UICONTROL Registration Error]，則復原為時已晚。

1. 從[!UICONTROL Members]索引標籤，篩選狀態為&#x200B;**[!UICONTROL Registration Error]**&#x200B;的人員清單。
1. 在繼續之前，請確定您已決定並修正整合的問題（請確定在[管理]中的&#x200B;**[!UICONTROL Event Partners]**&#x200B;下沒有錯誤）。
1. 問題解決後，選取所有狀態為[!UICONTROL Registration Error]的人員，並將其狀態變更為&#x200B;**[!UICONTROL Registered]**。 這將會嘗試再次向ON24註冊。

## 從ON24更新成員狀態 {#updating-member-status-from-on}

Marketo每晚大約會在太平洋時間晚上11點自動提取出勤資訊。 若要手動更新出席資訊，請按一下&#x200B;**[!UICONTROL Refresh from Webinar Provider]**&#x200B;下的&#x200B;**[!UICONTROL Event Actions]**。

>[!MORELIKETHIS]
>
>[瞭解Marketo ON24介面卡事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
