---
unique-page-id: 1900554
description: 編輯電子郵件的HTML —— 行銷檔案——產品檔案
title: 編輯電子郵件的HTML
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# 編輯電子郵件的HTML {#edit-an-emails-html}

有時，您可能需要修改電子郵件的基礎HTML。 有時，您可能會使用外部系統來設計和建立電子郵件的程式碼。 無論如何，您都可從電子郵件編輯器中輕鬆匯入和／或編輯程式碼。

## 編輯HTML {#edit-html}

1. 選擇您的電子郵件，然後按一下「編輯草稿」。****

   ![](assets/teamspidey.jpg)

1. 按一下「編輯代碼&#x200B;**」。**

   ![](assets/two-4.png)

1. 進行任何變更。 完成時，按一下「保存」。****

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >隨心所欲地改變。 您可以取代整個HTML，或進行小幅調整。

1. 按一下「程式碼動作」下拉式清單，以。html檔案形式下載程式碼、內嵌CSS或驗證HTML。****

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >電子郵件的最佳實務是讓所有樣式都內嵌在內。 有數位電子郵件用戶端不支援`<head>`區段中的CSS。

## 從電子郵件範本中斷{#breaking-an-email-from-its-template}

這些程式碼變更&#x200B;**將不會**&#x200B;中斷電子郵件範本：

* 編輯任何模組的內容（包括在模組中添加新的元素）
* 新增模組至容器
* 從容器中刪除模組

* 變更模組外部之任何元素的mkto特定屬性（例如&quot;mktoName&quot;或&quot;mktoImgUrl&quot;）
* 編輯任何元素（豐富式文字、影像、視訊等）的內容 模組外部

在代碼編輯器&#x200B;**will**&#x200B;中，您可以執行下列操作：

* 變更元素或模組以外的程式碼中的任何項目
* 新增或變更模組外部任何元素的非mkto屬性（例如「id」或「樣式」）
* 刪除模組外的元素

## 搜尋代碼{#search-code}

使用搜尋代碼功能，以有效率地尋找並取代電子郵件HTML代碼中的內容。

1. 在電子郵件的代碼中，按一下&#x200B;**搜索代碼**。

   ![](assets/five-2.png)

1. 輸入要查找的內容，然後按一下「查找下一個」(**Find Next**)向前搜索，或按一下「查找上一個」(**Find Previous)**&#x200B;向後搜索。 您也可以選擇「取代&#x200B;****」和「取代所有&#x200B;**」。**

   ![](assets/six-1.png)

1. 完成時，按一下&#x200B;**關閉**。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >[電子郵件範本編輯器](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md)中也提供搜尋代碼。

我們建議您繼續使用Marketo的內建功能來編輯電子郵件，但此程式碼編輯器可讓您視需要提供彈性。
