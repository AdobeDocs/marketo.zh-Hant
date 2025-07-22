---
unique-page-id: 14352592
description: 如何插入動態欄位 — Marketo檔案 — 產品檔案
title: 如何插入動態欄位
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 如何插入動態欄位 {#how-to-insert-dynamic-fields}

我們允許您使用`{{first_name}}`或`{{company}}`等預先定義的屬性，個人化您的電子郵件範本。 這些欄位可讓您以電子郵件傳送多個連絡人，並自動完成這些欄位，而不需為每個連絡人分別輸入這些欄位。

>[!TIP]
>
>「first_name」和「company」欄位是唯一會同時尋找[!DNL Sales Connect]和[!DNL Salesforce]的欄位。 也就是說，如果連絡人不存在於[網頁應用程式](https://toutapp.com/login)中，我們會檢視[!DNL Salesforce]，看看是否可找到具有相符電子郵件地址的連絡人/潛在客戶記錄。 然後使用該記錄中的資訊來填入欄位。

## 將動態欄位插入範本 {#insert-a-dynamic-field-into-a-template}

1. 在&#x200B;**[!UICONTROL Templates & Campaigns]**&#x200B;中，找到您要編輯的範本，然後按一下&#x200B;**[!UICONTROL Edit Template]**。

1. 按一下「**[!UICONTROL Tout Dynamic Fields]**」。

   >[!NOTE]
   >
   >以電子郵件傳送存在於[!DNL Sales Connect]中的連絡人時，您可以使用基本動態欄位。 這些會直接從連絡人提取。

如果您要傳送電子郵件給存在於[!DNL Salesforce]中的連絡人，您可以利用[!DNL Salesforce]動態欄位。 這些全都以「sfdc」開頭。 只要您連線至[!DNL Salesforce]，這些欄位就會直接呼叫[!DNL Salesforce]中的潛在客戶/連絡人，以填入範本中的資訊。

## 在主旨列插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只要手動複製並貼到電子郵件的主旨欄位中，請務必確保具有正確的格式。
