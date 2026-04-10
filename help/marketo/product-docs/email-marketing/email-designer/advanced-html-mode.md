---
solution: Marketo Engage
product: marketo
title: 將自訂 CSS 新增至您的電子郵件內容
description: 瞭解如何在電子郵件Designer中新增自訂CSS至電子郵件內容。 使用Marketo Engage中的自訂程式碼設定電子郵件樣式。
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
source-git-commit: af89a1a1fd0246564d0904103f742230a096de04
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 2%

---

# 使用進階HTML編輯器編輯電子郵件範本 {#advanced-html-mode}

進階HTML模式可讓您直接從[!DNL Marketo Engage]電子郵件Designer介面檢視及編輯電子郵件範本的原始原始程式碼。

此功能可讓您直接在來源中插入進階運算式。 當您切換回視覺（案頭）檢視時，內容會重新呈現，因此您可以檢查內容外觀，並繼續在任一檢視中進行編輯。

## 護欄 {#guardrails}

使用進階HTML編輯器時，以下護欄可保護內容相容性並設定預期。

* 進階HTML編輯器&#x200B;**無法驗證**&#x200B;您的程式碼。 它不會檢查語法錯誤或中斷的版面。 儲存前請仔細檢閱您的內容。

* 未來的系統更新可能會覆寫您對預設標籤所做的變更。 **您的變更可能不會持續存在**。

* [!DNL Adobe]支援&#x200B;**無法疑難排解或解決自訂程式碼和手動變更所造成的**&#x200B;問題。 保留內容的備份，以備您需要回覆時使用。

* 您無法在進階HTML檢視中模擬內容。 切換到案頭檢視以預覽您的內容。

* 為確保內容相容性，**您無法在進階HTML檢視中儲存**。 準備儲存變更時，切換回案頭檢視。

## 存取進階HTML模式 {#access-html-mode}

若要開啟進階HTML編輯器並編輯您的範本來源，請依照下列步驟操作。

1. 在電子郵件Designer中開啟或[建立電子郵件範本](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)。

1. 在&#x200B;_編輯電子郵件範本_&#x200B;畫面中，按一下右上角的HTML按鈕。

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. 第一次開啟進階HTML編輯器時，會顯示警告訊息。 完成時，按一下&#x200B;**[!UICONTROL OK]**&#x200B;進行檢閱。

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >此警告會在您首次開啟進階HTML編輯器時顯示，並在每月重設。

1. 進階HTML編輯器隨即顯示。

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. 將所需的變更新增至您的電子郵件內容。

   >[!WARNING]
   >
   >請務必輸入正確的HTML和CSS程式碼，因為沒有語法驗證程式，且Adobe支援無法協助進行HTML編輯。

1. 基於相容性原因，進階HTML檢視中無法使用內容模擬和儲存。 切換回案頭檢視以預覽您的內容並儲存變更。

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >當您切換檢視時，您的編輯會保留。
