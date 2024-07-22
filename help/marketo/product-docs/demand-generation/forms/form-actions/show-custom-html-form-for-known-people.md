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

如果訪客已編碼（過去提供電子郵件地址的已知人員），為何還要麻煩使用表格？ 只要給他們下載按鈕即可。 方法如下。

1. 移至&#x200B;**行銷活動**。

   ![](assets/login-marketing-activities-5.png)

1. 在&#x200B;**行銷活動**&#x200B;下，選取您的表單並按一下&#x200B;**編輯表單**。

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 在&#x200B;**表單設定**&#x200B;下，按一下&#x200B;**設定**。

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 設定&#x200B;**已知訪客，顯示**：為&#x200B;**自訂HTML**。

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 按一下![—](assets/image2014-9-25-14-3a1-3a26.png)以編輯將顯示給已知人員的&#x200B;**自訂HTML**。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 雖然有部分預設內容，但您可以隨時變更內容。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用Token：

   | Token | 說明 |
   |---|---|
   | `{{lead.FirstName}}` | 這會顯示使用者的名字。 |
   | `{{lead.LastName}}` | 這會顯示人員的姓氏。 |
   | `{{form.Button:default=Download}}` | 這會顯示表單按鈕。 取代`=`之後的區域以變更按鈕文字。 |
   | `{{form.NotYou:default=Not you?}}` | 若此人是其他人，此畫面會顯示連結。 取代`=`之後的區域以變更連結文字。 |

   >[!CAUTION]
   >
   >上述四個代號只能使用。 此處無法使用任何其他權杖。

1. 按一下&#x200B;**完成**。

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 按一下&#x200B;**核准並關閉**。

   >[!NOTE]
   >
   >此表單必須經過核准才能用於登入頁面。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >記得要[核准表單變更所建立的登入頁面草稿](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md)。

   小菜一碟！ 檢視某人返回相同表單時會看到什麼內容：

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >您可以將表單後續追蹤頁面設定為檔案的URL，將按鈕的點選導向資產。
