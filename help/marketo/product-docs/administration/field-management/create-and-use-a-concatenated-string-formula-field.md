---
unique-page-id: 2360337
description: 建立和使用串連字串（公式）欄位 — Marketo檔案 — 產品檔案
title: 建立和使用串連字串（公式）欄位
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# 建立和使用串連字串（公式）欄位 {#create-and-use-a-concatenated-string-formula-field}

您可以結合多個欄位的值，或使用Marketo公式欄位建立條件值。

1. 前往 **管理** 按一下 **欄位管理**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. 按一下 **新自訂欄位**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. 選擇 **公式** 針對 **類型**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. 輸入 **名稱** ，然後按一下 **建立**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. 查找並選擇公式欄位，然後按一下 **編輯規則**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. 新增兩個選項，並像下方的螢幕擷取一樣加以定義。

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >深入了解 [流程步驟的代號](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. 現在，您可以將公式欄位新增為電子郵件中的代號。

   ![](assets/seven.png)

>[!NOTE]
>
>公式欄位可用於登錄頁面、電子郵件和智慧清單欄（不會匯出）。 含有公式欄位的電子郵件可 **not** 使用批次促銷活動來傳送。 請使用 [電子郵件指令碼Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) 在此案例中。

幹得好！ 現在，您擁有一個智慧的領域，知道根據性別應包含哪些稱呼。 玩得開心一點，有創意。
