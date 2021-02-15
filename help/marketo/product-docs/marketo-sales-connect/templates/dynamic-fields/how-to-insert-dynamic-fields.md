---
unique-page-id: 14352592
description: 如何插入動態欄位——行銷檔案——產品檔案
title: 如何插入動態欄位
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# 如何插入動態欄位{#how-to-insert-dynamic-fields}

我們允許您使用預先定義的屬性（例如`{{first_name}}`或`{{company}}`）個人化您的電子郵件範本。 這些欄位可讓您以電子郵件傳送多個連絡人，並自動完成這些欄位，而不需為每個連絡人個別輸入。

>[!TIP]
>
>&quot;first_name&quot;和&quot;company&quot;欄位是Sales Connect和Salesforce中唯一可尋找的欄位。 這表示，如果[Web應用程式](https://toutapp.com/login)中不存在連絡人，我們會在Salesforce中尋找連絡人／銷售機會記錄，以找出相符的電子郵件地址。 然後，我們會使用該記錄中的資訊填入欄位。

## 將動態欄位插入範本{#insert-a-dynamic-field-into-a-template}

1. 在&#x200B;**範本與促銷活動**&#x200B;中，尋找您要編輯的範本，然後按一下&#x200B;**編輯範本**。

1. 按一下「**輸出動態欄位**」。

   >[!NOTE]
   >
   >在以電子郵件寄送Sales Connect中存在的聯繫人時，您可以使用基本的動態欄位。 這些會直接從聯繫人那裡拉出。

如果您正在以電子郵件寄送存在於Salesforce中的聯絡人，您可以利用Salesforce動態欄位。 這些都以「sfdc」開頭。 只要您與Salesforce有連線，這些欄位就會直接呼叫Salesforce中的潛在客戶／連絡人，以在範本中填入資訊。

## 在主旨行{#insert-dynamic-fields-in-a-subject-line}中插入動態欄位

只需手動將它們複製並貼至電子郵件的主旨欄位，並小心確保您有正確的格式。
