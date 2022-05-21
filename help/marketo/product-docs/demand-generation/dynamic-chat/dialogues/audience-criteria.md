---
description: Audience Criteria - Marketo Docs - Product Documentation
title: 對象條件
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
source-git-commit: a437f39ccc5b1937c34ce43e7aedad82b22cf532
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 1%

---

# 對象條件 {#audience-criteria}

Similar to Marketo Smart Lists, Audience Criteria attributes allow you to define your target audience. You can target known or unknown people using inferred, person, or company attributes (or a combination thereof).

****

__****

1. ****

   ![](assets/audience-criteria-1.png)

1. __ In the Select Values field, type in CA (you can also click the drop-down and select from the list).

   ![](assets/audience-criteria-2.png)

1. ****__

   ![](assets/audience-criteria-3.png)

   >[!NOTE]
   >
   >****

1. ****

   ![](assets/audience-criteria-4.png)

1. Type 50 and click elsewhere on the screen to save.

   ![](assets/audience-criteria-5.png)

And that&#39;s it!

****

There&#39;s an easy way to specifically target people who are not in your database yet. ****

1. ****

   ![](assets/audience-criteria-6.png)

1. ****

   ![](assets/audience-criteria-7.png)

1. ****__

   ![](assets/audience-criteria-8.png)

   >[!NOTE]
   >
   >[](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)We look up their IP in a special database and infer all kinds of good info.

1. __ In the Select Values field, type in NY (you can also click the drop-down and select from the list).

   ![](assets/audience-criteria-9.png)

## Add Groups {#add-groups}

You have the option of grouping attributes as well, in case you want to have all of certain attributes along with &quot;all or any&quot; of another. You can add multiple groups.

![](assets/audience-criteria-10.png)

![](assets/audience-criteria-11.png)

## 目標 {#target}

This is where you enter the URL(s) that you want a specific Dialogue to be shown on. You also have the option of adding exclusions.

Acceptable formats:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>Using an asterisk acts as a catch-all wilcard. `https://*.website.com``support.website.com``https://website.com/folder/*`

**** Exclusions follow the same format as inclusions.

![](assets/audience-criteria-12.png)

>[!MORELIKETHIS]
>
>* [](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md)
>* [](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md)
>* [](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md)

