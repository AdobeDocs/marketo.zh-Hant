---
description: 變更Velocity指令碼中的自訂物件擷取限制 — Marketo檔案 — 產品檔案
title: 更改Velocity指令碼中的自定義對象檢索限制
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 更改Velocity指令碼中的自定義對象檢索限制 {#change-custom-object-retrieval-limits-in-velocity-scripting}

如果您使用Velocity指令碼在電子郵件中顯示自訂物件資料，則此功能可能適用於您。 預設情況下，您可以從Velocity指令碼訪問10個父自定義對象。 如果您需要存取更多資訊，請閱讀。

## 什麼是Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/) 是以Java為基礎所建置的語言，專為範本和指令碼HTML內容而設計。 Marketo可讓您透過使用 [指令碼Token](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). 除了其他功能，這可讓您存取儲存在自訂物件中的資料。

您可以參考直接連接到銷售機會或聯繫人的父自定義對象和子自定義對象，但不能參考第三級自定義對象。 對於每個自訂物件，每人/聯絡人最近更新的10筆記錄可在執行階段使用，並從最近更新(0)排序至最舊更新(9)。

## 如何變更限制 {#how-to-change-the-limit}

1. 前往 **管理** 區段。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 按一下 **電子郵件**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在「自定義對象檢索限制」(Custom Object Retrieval Limits)表中，輸入新的父檢索限制，然後按一下 **儲存變更**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>父檢索限制值必須在10 - 100的範圍內。 系統會自動為您設定子檢索限制。 這是透過將1000除以父項擷取限制來完成。 例如，如果您將父項限制設定為50，子項限制將變為20(1000 ÷ 50 = 20)。

真貼心！ 現在，您可以從Velocity指令碼存取更多自訂物件。
