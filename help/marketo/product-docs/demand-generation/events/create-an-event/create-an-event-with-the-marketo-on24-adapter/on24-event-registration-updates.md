---
unique-page-id: 10096683
description: ON24事件註冊更新 — Marketo檔案 — 產品檔案
title: ON24事件註冊更新
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# ON24事件註冊更新 {#on-event-registration-updates}

## 手動核准註冊者 {#manually-approving-registrants}

您可以在傳送確認電子郵件給註冊者之前，手動核准他們。 若要這麼做，您將需要設定行銷活動以處理此額外步驟：

1. 針對註冊觸發程式行銷活動：

   * 在智慧清單中，將觸發器設定為&#x200B;**填寫表單**。
   * 在「流程」中，將「進行中的狀態」設定為&#x200B;**未決核准**。

1. 移至[事件]，然後按一下[成員] **標籤。**&#x200B;此索引標籤會顯示所有已填寫表單的人。 其狀態應設為&#x200B;**未決核准**。
1. 使用格線頂端的篩選器，只檢視狀態為&#x200B;**未決核准**&#x200B;的人員。
1. 選取您要註冊的人員（按住Shift鍵並按一下、按住Control鍵並按一下，或選取全部）。
1. 在功能表中按一下&#x200B;**變更狀態**。 選取&#x200B;**已註冊**、**已拒絕**&#x200B;或任何其他適用狀態。

## 處理發生註冊錯誤的人員 {#handling-people-with-a-registration-error}

如果人員最後並未註冊，而是設定為註冊錯誤狀態，現在復原還為時不晚。

1. 從[成員]索引標籤，篩選狀態為&#x200B;**註冊錯誤**&#x200B;的人員清單。
1. 在繼續之前，請確定您已決定並修正整合的問題（請檢查以確定在Admin中的&#x200B;**事件合作夥伴**&#x200B;下沒有錯誤）。
1. 問題解決後，請選取所有狀態為「註冊錯誤」的人員，並將其狀態變更為&#x200B;**已註冊**。 這將會嘗試再次向ON24註冊。

## 從ON24更新成員狀態 {#updating-member-status-from-on}

Marketo每晚大約會在太平洋時間晚上11點自動提取出勤資訊。 若要手動更新出席資訊，請按一下&#x200B;**事件動作**&#x200B;底下的&#x200B;**網路研討會提供者重新整理**。

>[!MORELIKETHIS]
>
>[瞭解Marketo ON24介面卡事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
