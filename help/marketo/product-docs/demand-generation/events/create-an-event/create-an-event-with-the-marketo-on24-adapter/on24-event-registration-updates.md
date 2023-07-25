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

您可以在傳送確認電子郵件給註冊者之前，手動核准他們。 若要這麼做，您需要設定行銷活動以處理此額外步驟：

1. 對於註冊觸發程式行銷活動：

   * 在「智慧列示」中，將觸發器設為 **填寫表單**.
   * 在流程中，將進度中的狀態設定為 **未決核准**.

1. 前往事件並按一下 **成員** 標籤。 此標籤會顯示所有已填寫表單的人。 其狀態應設為 **未決核准**.
1. 使用格線頂端的篩選器，只檢視狀態為「 」的人員 **未決核准**.
1. 選取您要註冊的人員（按住Shift鍵並按一下、按住Control鍵並按一下，或選取全部）。
1. 在功能表中，按一下 **變更狀態**. 選取 **已註冊**， **已拒絕**&#x200B;或任何其他適用狀態。

## 處理發生註冊錯誤的人員 {#handling-people-with-a-registration-error}

如果人員最後並未註冊，而是設定為註冊錯誤，現在復原還為時不晚。

1. 從「成員」索引標籤，篩選具有狀態的人員清單 **註冊錯誤**.
1. 在繼續之前，請確定您已確定並修正整合的問題（請檢查以確定下沒有錯誤） **活動合作夥伴** （在「管理員」中）。
1. 問題解決後，選擇所有狀態為「註冊錯誤」的人員，並將其狀態變更為 **已註冊**. 這將嘗試再次向ON24註冊它們。

## 從ON24更新成員狀態 {#updating-member-status-from-on}

Marketo每晚大約會在太平洋時間晚上11點自動提取出勤資訊。 若要手動更新出勤資訊，請按一下 **從網路研討會提供者重新整理** 在 **事件動作**.

>[!MORELIKETHIS]
>
>[瞭解Marketo ON24介面卡事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
