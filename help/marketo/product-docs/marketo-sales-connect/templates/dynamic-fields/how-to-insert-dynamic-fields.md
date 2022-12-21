---
unique-page-id: 14352592
description: 如何插入動態欄位 — Marketo檔案 — 產品檔案
title: 如何插入動態欄位
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 如何插入動態欄位 {#how-to-insert-dynamic-fields}

我們可讓您使用預先定義的屬性(例如 `{{first_name}}` 或 `{{company}}`. 這些欄位可讓您傳送電子郵件給多個聯絡人，並自動完成這些欄位，而不必為每個聯絡人個別輸入。

>[!TIP]
>
>&quot;first_name&quot;和&quot;company&quot;欄位是唯一同時查看Sales Connect和Salesforce的欄位。 這表示如果連絡人不存在於 [網頁應用程式](https://toutapp.com/login)，我們會在Salesforce中查看是否能找到具有相符電子郵件地址的聯絡/銷售機會記錄。 然後，我們會使用該記錄的資訊來填入欄位。

## 將動態欄位插入範本 {#insert-a-dynamic-field-into-a-template}

1. 在 **範本與行銷活動**，找到您要編輯的範本並按一下 **編輯範本**.

1. 按一下 **輸出動態欄位**.

   >[!NOTE]
   >
   >用電子郵件發送Sales Connect中存在的聯繫人時，可以使用基本的動態欄位。 這些會直接從聯絡人處拉出。

如果您正在向Salesforce中存在的聯繫人發送電子郵件，則可以利用Salesforce動態欄位。 這些都以「sfdc」開頭。 只要您與Salesforce有連線，這些欄位就會直接呼叫Salesforce中的銷售機會/連絡人，以填入範本中的資訊。

## 在主旨行中插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只需手動複製並貼到電子郵件的主旨欄位，並請務必注意，以確保格式正確。
