---
unique-page-id: 2359644
description: 顯示已知人員的自訂HTML表單——行銷人員檔案——產品檔案
title: 顯示已知人員的自訂HTML表單
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# 顯示已知人員的自訂HTML表單 {#show-custom-html-form-for-known-people}

如果訪客是Cookie（過去提供電子郵件地址的已知人員），那麼為什麼要費心處理表格？ 只要給他們下載按鈕。 這是方法。

1. 前往「行 **銷****活動」**。

   ![](assets/login-marketing-activities-5.png)

1. 在「 **行銷** 活 **動」**&#x200B;下 **，選取您的表單，然後按一** 下「編 **輯表單**」。

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 在「表 **單設** 定 **」下，按一**&#x200B;下「設定 ****」。

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 若已知訪 **客** , **請設定顯示**:至自 **訂****HTML**。

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 按一 ![下-](assets/image2014-9-25-14-3a1-3a26.png) 以編輯將顯 **示給已知人** 員的自訂 **** HTML。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 有些預設內容，但您可以隨意修改。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用的Token:

   | Token | 說明 |
   |---|---|
   | `{{lead.FirstName}}` | 這會顯示該人員的名字。 |
   | `{{lead.LastName}}` | 這將顯示該人的姓。 |
   | `{{form.Button:default=Download}}` | 這將顯示表單按鈕。 取代按鈕文 `=` 字後的區域。 |
   | `{{form.NotYou:default=Not you?}}` | 這會顯示連結，以防該人為其他人。 取代後方的區 `=` 域以變更連結文字。 |

   >[!CAUTION]
   >
   >只能使用上述4個Token。 任何其他Token在此處都無法運作。

1. 按一 **下完成**。

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 按一 **下「核准並關閉**」。

   >[!NOTE]
   >
   >表單必須經過核准才能用於登陸頁面。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >請記得 [核准表單變更所建立](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) 的著陸頁面草稿。

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >您可以將按鈕的點按指向資產，方法是將表單後續頁面設定至檔案的URL。

小菜一碟！ 查看如果回到相同的表格，人們會看到什麼：