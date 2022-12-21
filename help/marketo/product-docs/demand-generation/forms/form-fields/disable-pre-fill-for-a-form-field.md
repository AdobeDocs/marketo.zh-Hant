---
unique-page-id: 2359675
description: 停用表單欄位的預填 — Marketo檔案 — 產品檔案
title: 停用表單欄位的預填
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 停用表單欄位的預填 {#disable-pre-fill-for-a-form-field}

已知網頁訪客(Cookie)時，Marketo表單會依預設以其資訊預先填入欄位。 如果你想關掉它，這是怎麼做的。

>[!NOTE]
>
>**表單預填** 預設為啟用。 登陸頁面層級預填設定和管理層級預填設定高於表單層級設定：
>
>表單>登陸頁面>管理

## 如何停用預填 {#how-to-disable-pre-fill}

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-7.png)

1. 選取您的表單並按一下 **編輯表單**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >將表單嵌入到您自己的頁面時，表單預填無法運作。 它只適用於Marketo登陸頁面。

1. 選取其中一個欄位並設定 **表單預填** to **已停用**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >您也可以在登陸頁面層級或管理層級停用表單預填。

1. 按一下 **完成**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. 按一下 **核准並關閉**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## 敏感欄位 {#sensitive-fields}

當您 [將欄位標示為敏感欄位](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md)，防止其值預先填入表單中，您會在「預填」選項中看到這個資訊。

![](assets/disable-pre-fill.png)