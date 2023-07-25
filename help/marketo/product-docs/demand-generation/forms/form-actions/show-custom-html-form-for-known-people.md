---
unique-page-id: 2359644
description: 顯示已知人員的自訂HTML表單 — Marketo檔案 — 產品檔案
title: 顯示已知人員的自訂HTML表單
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# 顯示已知人員的自訂HTML表單 {#show-custom-html-form-for-known-people}

如果訪客已確認（過去提供電子郵件地址的已知人員），為何還要麻煩使用表單？ 只要給他們下載按鈕即可。 方法如下。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-5.png)

1. 下 **行銷活動**，選取您的表單並按一下 **編輯表單**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 下 **表單設定**，按一下 **設定**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 設定條件 **已知訪客，節目**：至 **自訂HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 按一下 ![—](assets/image2014-9-25-14-3a1-3a26.png) 若要編輯 **自訂HTML** 會向已知人員顯示。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 有一些預設內容，但您可以隨意變更。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用Token：

   | Token | 說明 |
   |---|---|
   | `{{lead.FirstName}}` | 這會顯示個人的名字。 |
   | `{{lead.LastName}}` | 這會顯示人員的姓氏。 |
   | `{{form.Button:default=Download}}` | 這會顯示表單按鈕。 取代之後的區域 `=` 以變更按鈕文字。 |
   | `{{form.NotYou:default=Not you?}}` | 若此人是其他人，此畫面會顯示連結。 取代之後的區域 `=` 以變更連結文字。 |

   >[!CAUTION]
   >
   >只能使用上述四個代號。 此處無法使用任何其他權杖。

1. 按一下 **完成**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 按一下 **核准並關閉**.

   >[!NOTE]
   >
   >此表單必須經過核准才能用於登陸頁面。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >記住 [核准登入頁面草稿](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) 由表單變更所建立。

   蛋糕！ 檢視人員返回相同表單時會看到什麼內容：

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >您可以將表單後續追蹤頁面設定為檔案的URL，將按鈕的點選導向資產。
