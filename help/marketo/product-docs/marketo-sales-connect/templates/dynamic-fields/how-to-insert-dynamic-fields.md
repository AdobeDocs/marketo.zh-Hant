---
unique-page-id: 14352592
description: 如何插入動態欄位 — Marketo檔案 — 產品檔案
title: 如何插入動態欄位
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 如何插入動態欄位 {#how-to-insert-dynamic-fields}

我們允許您使用預先定義的屬性(例如 `{{first_name}}` 或 `{{company}}`. 這些欄位可讓您以電子郵件傳送多個連絡人，並自動完成這些欄位，而不需為每個連絡人分別輸入這些欄位。

>[!TIP]
>
>「first_name」和「company」欄位是唯一會同時檢視Sales Connect和Salesforce的欄位。 這表示如果連絡人不存在於 [網頁應用程式](https://toutapp.com/login)，我們會檢視Salesforce以確認是否能找到具有相符電子郵件地址的聯絡人/潛在客戶記錄。 然後使用該記錄中的資訊來填入欄位。

## 將動態欄位插入範本 {#insert-a-dynamic-field-into-a-template}

1. 在 **範本與行銷活動**，找到您要編輯的範本並按一下 **編輯範本**.

1. 按一下 **Tout動態欄位**.

   >[!NOTE]
   >
   >當傳送電子郵件給Sales Connect中的連絡人時，您可以使用基本的動態欄位。 這些會直接從連絡人提取。

如果您要傳送電子郵件給Salesforce中的聯絡人，則可以利用Salesforce動態欄位。 這些全都以「sfdc」開頭。 只要您有Salesforce的連線，這些欄位就會直接呼叫Salesforce中的銷售機會/聯絡人，在範本中填入資訊。

## 在主旨列插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只要手動複製並貼到電子郵件的主旨欄位中，請務必確保具有正確的格式。
