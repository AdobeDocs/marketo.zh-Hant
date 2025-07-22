---
unique-page-id: 2953243
description: 通知型別 — Marketo檔案 — 產品檔案
title: 通知型別
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 1%

---

# 通知型別 {#notification-types}

通知型別有幾種。

## 行銷活動失敗  {#campaign-failure}

行銷活動失敗會通知您智慧型行銷活動中的錯誤。

## CRM同步 {#crm-sync}

CRM同步通知會針對CRM同步處理發現的關鍵問題提醒您，例如許可權不正確或同步處理已關閉。

**[!DNL Microsoft Dynamics]**

每24小時傳送一次[!DNL Dynamics]則通知，其中包含無法在該時段內同步處理的銷售機會。 失敗的一般原因是重複的銷售機會（如上所述）或欄位長度不符錯誤。

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

如果您使用[!DNL Salesforce]，同步錯誤通知看起來會類似於下面的通知。 典型錯誤包括憑證過期和超出API限制。

![](assets/salesforcesyncerror.png)

## 參與度 {#engagement}

當人們在資料流中精疲力盡時，我們會傳送通知。 通知包括筋疲力盡的人數和某些其他資訊。

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

如果您嘗試在不接受服務條款的情況下將人們傳送到Facebook，或如果您在移除Marketo應用程式後嘗試將人們傳送到Facebook。

## 閒置觸發程式促銷活動清除 {#idle-trigger-campaign-cleanup}

停用已觸發不再取得任何活動的智慧型行銷活動。 深入瞭解[自動觸發行銷活動清理](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)。

## LinkedIn {#linkedin}

當Marketo無法建立新受眾、登入時，或是在三次嘗試後推送電子郵件至LinkedIn。

![](assets/linkedin.png)

## 網站服務 {#web-services}

當您達到每日配額時，您將會收到通知。 配額會在每個午夜的中央時間重設。

>[!NOTE]
>
>我們在[開發人員檔案](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/error-codes)中列出您可能會收到的部分錯誤碼。
