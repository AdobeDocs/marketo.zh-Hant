---
unique-page-id: 1900554
description: 編輯電子郵件HTML- Marketo檔案 — 產品檔案
title: 編輯電子郵件的HTML
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 編輯電子郵件的HTML {#edit-an-emails-html}

有時您可能需要修改電子郵件的基礎HTML。 有時您可以使用外部系統來設計和建置電子郵件的程式碼。 無論是哪種方式，您都可以輕鬆地從電子郵件編輯器匯入及/或編輯程式碼。

## 編輯HTML {#edit-html}

1. 選取您的電子郵件並按一下 **編輯草稿**.

   ![](assets/teamspidey.jpg)

1. 按一下 **編輯程式碼**.

   ![](assets/two-4.png)

1. 進行任何變更。 按一下 **儲存** 完成時。

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >隨心所欲地變更。 您可以取代整個HTML或進行微幅調整。

1. 按一下 **程式碼動作** 下拉式清單，將程式碼下載為.html檔案、內嵌您的CSS或驗證HTML。

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >電子郵件的最佳實務是讓您的所有樣式內嵌。 有數個電子郵件使用者端不支援 `<head>` 區段。

## 從範本中斷電子郵件 {#breaking-an-email-from-its-template}

這些程式碼變更 **不會** 從範本中斷電子郵件：

* 編輯任何模組的內容（包括在模組內新增元素）
* 將新模組新增至容器
* 從容器中刪除模組

* 變更模組外任何元素的mkto特定屬性（例如「mktoName」或「mktoImgUrl」）
* 編輯任何元素的內容（RTF文字、影像、視訊等） 模組外

您可以在程式碼編輯器中執行下列動作 **將** 中斷範本中的電子郵件：

* 在元素或模組之外變更程式碼中的任何專案
* 新增或變更模組外任何元素的非mkto屬性（例如，「id」或「style」）
* 刪除模組以外的元素

## 搜尋代碼 {#search-code}

使用搜尋代碼功能，能夠有效地尋找及取代電子郵件HTML代碼中的內容。

1. 在電子郵件的程式碼中，按一下 **搜尋代碼**.

   ![](assets/five-2.png)

1. 輸入您要尋找的內容，然後按一下 **尋找下一個** 往前搜尋或 **尋找上一個** 以向後搜尋。 您也可選擇 **取代** 和 **全部取代**.

   ![](assets/six-1.png)

1. 按一下 **關閉** 完成時。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >搜尋代碼也可在 [電子郵件範本編輯器](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

我們建議您使用Marketo的內建功能繼續編輯電子郵件，但此程式碼編輯器可讓您在需要時提供彈性。
