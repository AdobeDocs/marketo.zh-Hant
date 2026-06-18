---
unique-page-id: 7515133
description: 瞭解Salesforce和Marketo中合併銷售機會、聯絡人和人員的運作方式。 瞭解分數、欄位值和活動記錄的合併規則。
title: SFDC同步 — 合併銷售機會/聯絡人/人員
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 25bbf4409df3db38b849d936e2a90b48f859d089
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 2%

---

# SFDC 同步：合併商機/聯絡人/人員 {#sfdc-sync-merging-a-lead-contact-person}

有時最好只列出規則。 開始吧：

* 當您在&#x200B;**[!DNL Salesforce]**&#x200B;中合併兩個銷售機會時，一般的同步會告知Marketo，而銷售機會會自動合併為Marketo中的人員。
* 在&#x200B;**Marketo**&#x200B;中合併兩個人實際上會叫用與在[!DNL Salesforce]中合併潛在客戶相同的程式。 仍可自動運作。
* 將&#x200B;**銷售機會（人員）合併至連絡人**&#x200B;的工作方式相同。 最後兩邊只有一個接觸點。
* 合併時，會加總預設分數。

>[!NOTE]
>
>合併每個分數為10的3個銷售機會（人員），會產生1個銷售機會（人員）的結果，分數為30。

* 衝突的欄位值是從「成功記錄」中取得。 （記錄=產生的潛在客戶或連絡人）
* 如果「失敗記錄」（正在消失的記錄）有一個值，且成功記錄沒有（或為空），我們會保留失敗記錄。 換句話說，「有值總比沒有值好。」
* 所有活動記錄專案都會合併。

>[!NOTE]
>
>API合併中的布林值欄位行為在2026年3月版本中變更。 現在，系統會正確將False值視為該欄位有值。 評估衝突欄位時，只有null值會視為「空白」。 檢視[此社群貼文](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219){target="_blank"}更多詳細資料。

>[!MORELIKETHIS]
>
>深入瞭解[在Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)中合併人員的詳細資訊。
