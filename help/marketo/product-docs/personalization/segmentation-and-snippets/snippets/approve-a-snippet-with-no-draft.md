---
unique-page-id: 10095644
description: 使用非草稿即可核准程式碼片段 — Marketo檔案 — 產品檔案
title: 以非草稿方式核准程式碼片段
exl-id: a06aa77a-68f1-41a4-b2bd-bf1882b81578
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 以非草稿方式核准程式碼片段 {#approve-a-snippet-with-no-draft}

## 核准程式碼片段 {#approve-the-snippet}

每次核准程式碼片段時，都會觸發非草稿。 這包括由其他工作區中的資產共用或參考的程式碼片段。

1. 前往 **Design Studio**.

   ![](assets/go-to-design-studio.png)

1. 選取程式碼片段，並在 **程式碼片段動作** 下拉式清單，選擇 **核准**.

   ![](assets/approve-snippet.png)

1. 在核准程式碼片段對話方塊中選取選項，然後按一下 **核准**:

   * **全部更新**:此選項不會使用程式碼片段建立已核准資產的草稿。 所有資產都會取得更新並維護其先前狀態。 畫面右上方會顯示進度模組；可隨時關閉。 若要還原，請以滑鼠右鍵按一下程式碼片段名稱，然後選取「顯示核准狀態」 。
   * **建立草稿**:此選項會使用程式碼片段建立已核准資產的草稿。 如果需要先審核程式碼片段變更，請選取此選項。 必須手動批准所有草稿。

   ![](assets/snippet-dialog-box.png)

   >[!NOTE]
   >
   >對於尚未使用的新程式碼片段，此「核准草稿」畫面不會顯示。 此參數會在一或多個資產中使用程式碼片段時顯示。

>[!CAUTION]
>
>此功能的設計目的是透過程式碼片段核准工作流程節省時間。 不過，您仍須注意幾項限制。 請參閱 [此文檔](https://nation.marketo.com/docs/DOC-4415) 以取得詳細資訊。 該文檔還包含錯誤處理和故障排除資訊。

>[!MORELIKETHIS]
>
>[為片段啟用非草稿](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md)
