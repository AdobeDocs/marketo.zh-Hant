---
unique-page-id: 7515133
description: SFDC同步——合併銷售線索／聯繫人／人員——行銷人員——產品文檔
title: SFDC同步——合併銷售線索／聯繫人／人員
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# SFDC同步：合併銷售線索／聯繫人／人員{#sfdc-sync-merging-a-lead-contact-person}

有時最好只列出規則。 接下來：

* 當您在&#x200B;**Salesforce**&#x200B;中合併兩個銷售機會時，一般同步會告訴Marketo，而銷售機會會自動合併為Marketo中的人員。
* 在&#x200B;**Marketo**&#x200B;中合併兩個人實際上會叫用與在Salesforce中合併他們作為銷售線索相同的程式。 它仍會自動運作。
* 將&#x200B;**銷售線索（人員）合併到聯繫人**&#x200B;的運作方式相同。 最後雙方都有單一接觸。
* 合併時，預設分數會相加。

>[!NOTE]
>
>合併3個潛在客源（人），每10分，將產生1個潛在客源（人）,30分的結果。

* 從「成功記錄」擷取衝突的欄位值。 （記錄=產生的線索或聯繫人）
* 如果「失敗記錄」（即將消失的記錄）有價值，而獲勝記錄沒有價值，我們將保持失敗記錄。 換句話說，&quot;有些價值比沒有價值好。&quot;
* 將合併所有活動日誌項目。

>[!NOTE]
>
>深入瞭解[在Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)中合併人員的更多資訊。
