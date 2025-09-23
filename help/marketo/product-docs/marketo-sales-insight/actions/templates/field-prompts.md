---
description: 欄位提示 — Marketo檔案 — 產品檔案
title: 欄位提示
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 3%

---

# 欄位提示 {#field-prompts}

欄位提示可讓您將文字字串新增至需要移除或取代才能傳送電子郵件的電子郵件。 這是提醒使用者新增其他個人化的絕佳方式。

若要新增欄位提示，請輸入所要的文字。 請在開頭加上驚歎號，並在結尾加上大括弧（請參閱下文）。

**範例：**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>在傳送電子郵件之前，使用者需要先以自己的個人化內容取代此文字。

![](assets/field-prompts-1.png)

>[!NOTE]
>
>在促銷活動中使用提示時，最好將其與手動電子郵件步驟搭配使用。 這些步驟將指派提醒任務給使用者傳送電子郵件，讓他們有機會將提示替換為自訂文字。 Sales Campaigns中的自動電子郵件步驟將嘗試自動傳送，不允許使用者取代提示。 未取代的提示會導致電子郵件無法傳送。
