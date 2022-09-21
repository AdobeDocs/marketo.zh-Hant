---
unique-page-id: 10096683
description: ON24事件註冊更新 — Marketo檔案 — 產品檔案
title: ON24事件註冊更新
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# ON24事件註冊更新 {#on-event-registration-updates}

## 手動批准註冊者 {#manually-approving-registrants}

您可以在向註冊者發送確認電子郵件之前，手動核准他們。 若要這麼做，您需要設定促銷活動以處理此額外步驟：

1. 針對註冊觸發程式促銷活動：

   * 在「智慧清單」中，將觸發器設定為 **填寫表單**.
   * 在「流」中，將「進展狀態」設定為 **待批准**.

1. 前往「事件」 ，然後按一下 **成員** 標籤。 此頁簽顯示已填寫表單的所有人員。 其狀態應設為 **待批准**.
1. 使用格線頂端的篩選器，只檢視狀態為 **待批准**.
1. 選擇要註冊的人員（按住Shift鍵、按住Control鍵、按一下或選擇全部）。
1. 在功能表中，按一下 **更改狀態**. 選擇 **已註冊**, **已拒絕**，或任何其他適用狀態。

## 處理有註冊錯誤的人員 {#handling-people-with-a-registration-error}

如果某人最終未註冊，而是設定為狀態「註冊錯誤」，則恢復為時尚晚。

1. 從「成員」頁簽中，篩選狀態為的人員清單 **註冊錯誤**.
1. 繼續之前，請確定您已確定並修正整合的問題（請檢查以確定下沒有錯誤） **活動合作夥伴** 中)。
1. 問題解決後，請選擇所有狀態為「註冊錯誤」的人員，並將其狀態更改為 **已註冊**. 這將嘗試在ON24中重新註冊它們。

## 從ON24更新成員狀態 {#updating-member-status-from-on}

Marketo會每天晚上約11點自動提取出勤資訊。 要手動更新考勤資訊，請按一下 **從網路研討會提供者重新整理** 在 **事件動作**.

>[!MORELIKETHIS]
>
>[了解Marketo ON24適配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}
