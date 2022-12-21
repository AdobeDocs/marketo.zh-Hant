---
unique-page-id: 1900554
description: 編輯電子郵件的HTML- Marketo檔案 — 產品檔案
title: 編輯電子郵件的HTML
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 編輯電子郵件的HTML {#edit-an-emails-html}

有時候，您可能需要修改電子郵件的基礎HTML。 有時候，您可能會使用外部系統來設計和建立電子郵件的代碼。 無論使用哪種方式，您都可以在電子郵件編輯器中輕鬆匯入和/或編輯代碼。

## 編輯HTML {#edit-html}

1. 選取您的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/teamspidey.jpg)

1. 按一下 **編輯代碼**.

   ![](assets/two-4.png)

1. 進行任何變更。 按一下 **儲存** 時才能使用。

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >隨便你改變。 您可以取代整個HTML或進行微幅調整。

1. 按一下 **程式碼動作** 下拉式清單，將程式碼下載為.html檔案、內嵌您的CSS或驗證HTML。

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >電子郵件的最佳作法是內嵌所有樣式。 若干電子郵件用戶端不支援 `<head>` 區段。

## 從其範本中斷電子郵件 {#breaking-an-email-from-its-template}

這些程式碼會變更 **不會** 從其範本中斷電子郵件：

* 編輯任何模組的內容（包括在模組內新增元素）
* 新增模組至容器
* 從容器中刪除模組

* 變更模組外部任何元素的mkto特定屬性（例如&quot;mktoName&quot;或&quot;mktoImgUrl&quot;）
* 編輯任何元素的內容（RTF、影像、視訊等） 模組外部

您可以在程式碼編輯器中執行的這些操作 **will** 從其範本中斷電子郵件：

* 變更元素或模組以外的程式碼中的任何項目
* 新增或變更模組以外任何元素的非mkto屬性（例如「id」或「style」）
* 刪除模組外部的元素

## 搜尋代碼 {#search-code}

使用搜尋代碼功能，以有效率地尋找和取代電子郵件HTML代碼中的內容。

1. 在電子郵件的程式碼中，按一下 **搜尋代碼**.

   ![](assets/five-2.png)

1. 輸入要查找的內容，然後按一下 **查找下一個** 向前搜索或 **查找上一個** 來回搜尋。 您也可以選擇 **取代** 和 **全部替換**.

   ![](assets/six-1.png)

1. 按一下 **關閉** 時才能使用。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >搜尋代碼也可在 [電子郵件範本編輯器](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

建議您繼續使用Marketo的內建功能編輯電子郵件，但如有需要，此程式碼編輯器確實提供彈性。
