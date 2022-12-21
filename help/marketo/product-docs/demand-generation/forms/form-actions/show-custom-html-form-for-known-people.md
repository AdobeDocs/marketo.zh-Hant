---
unique-page-id: 2359644
description: 顯示已知人員的自訂HTML表單 — Marketo檔案 — 產品檔案
title: 顯示已知人員的自定義HTML表單
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# 顯示已知人員的自定義HTML表單 {#show-custom-html-form-for-known-people}

如果訪客是Cookie（過去曾提供電子郵件地址的已知人員），那麼為何還要麻煩使用表單？ 給他們下載按鈕。 這是方法。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-5.png)

1. 在 **行銷活動**，選取您的表單並按一下 **編輯表單**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 在 **表單設定**，按一下 **設定**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 若 **已知訪客，節目**:to **自訂HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 按一下 ![—](assets/image2014-9-25-14-3a1-3a26.png) 編輯 **自訂HTML** 會向已知人展示。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 有一些預設內容，但可以隨時更改。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用的Token:

   | 代號 | 說明 |
   |---|---|
   | `{{lead.FirstName}}` | 這會顯示人員的名字。 |
   | `{{lead.LastName}}` | 這會顯示該人員的姓氏。 |
   | `{{form.Button:default=Download}}` | 這會顯示表單按鈕。 替換 `=` 來更改按鈕文本。 |
   | `{{form.NotYou:default=Not you?}}` | 這會顯示連結，以防該人是其他人。 替換 `=` 來更改連結文本。 |

   >[!CAUTION]
   >
   >只能使用上述四個代號。 此處無法使用任何其他Token。

1. 按一下 **完成**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 按一下 **核准並關閉**.

   >[!NOTE]
   >
   >表單必須經過核准，才能用於登錄頁面。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >記住 [核准登錄頁面草稿](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) 由表單建立時變更。

   蛋糕！ 查看若使用者回到相同表單時會看到什麼內容：

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >您可以將表單後續頁面設定為檔案的URL，將按鈕的點按導向至資產。
