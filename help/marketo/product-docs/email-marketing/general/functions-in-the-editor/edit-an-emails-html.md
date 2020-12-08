---
unique-page-id: 1900554
description: 編輯電子郵件的HTML —— 行銷檔案——產品檔案
title: 編輯電子郵件的HTML
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 編輯電子郵件的HTML {#edit-an-emails-html}

有時，您可能需要修改電子郵件的基礎HTML。 有時，您可能會使用外部系統來設計和建立電子郵件的程式碼。 無論如何，您都可從電子郵件編輯器中輕鬆匯入和／或編輯程式碼。

## 編輯HTML {#edit-html}

1. 選取您的電子郵件，然後按一下「 **編輯草稿**」。

   ![](assets/teamspidey.jpg)

1. 按一 **下編輯代碼**。

   ![](assets/two-4.png)

1. 進行任何變更。 完成時 **按一下** 「儲存」。

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >隨心所欲地改變。 您可以取代整個HTML，或進行小幅調整。

1. 按一 **下「程式碼動作** 」下拉式清單，將程式碼下載為。html檔案、內嵌CSS或驗證HTML。

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >電子郵件的最佳實務是讓所有樣式都內嵌在內。 有數位電子郵件客戶不支援區段中的CSS `<head>` 功能。

## 從電子郵件範本中斷電子郵件 {#breaking-an-email-from-its-template}

這些程式碼 **變更不會** 中斷電子郵件範本：

* 編輯任何模組的內容（包括在模組中添加新的元素）
* 新增模組至容器
* 從容器中刪除模組

* 變更模組外部之任何元素的mkto特定屬性（例如&quot;mktoName&quot;或&quot;mktoImgUrl&quot;）
* 編輯任何元素（豐富式文字、影像、視訊等）的內容 模組外部

您在程式碼編輯器中可執行的下列 **動作** ，會中斷電子郵件範本：

* 變更元素或模組以外的程式碼中的任何項目
* 新增或變更模組外部任何元素的非mkto屬性（例如「id」或「樣式」）
* 刪除模組外的元素

## 搜尋代碼 {#search-code}

使用搜尋代碼功能，以有效率地尋找並取代電子郵件HTML代碼中的內容。

1. 在您電子郵件的程式碼中，按一下「搜 **尋程式碼」**。

   ![](assets/five-2.png)

1. 輸入要查找的內容，然後按一下「查找下 **一步」** (Find Next **)向前搜索，或** 按一下「查找上一步」(Find Previous)向後搜索。 您也可以選擇「取 **代** 」 **和「全部取代」**。

   ![](assets/six-1.png)

1. 完成時 **按一下** 「關閉」。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >「電子郵件範本」編輯器中也提供 [搜尋代碼](http://docs.marketo.com/display/DOCS/Create+a+New+Email+Template)。

我們建議您繼續使用Marketo的內建功能來編輯電子郵件，但此程式碼編輯器可讓您視需要提供彈性。
