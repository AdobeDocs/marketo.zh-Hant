---
unique-page-id: 2953243
description: 通知類型 — Marketo檔案 — 產品檔案
title: 通知類型
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 2%

---

# 通知類型 {#notification-types}

有數種通知類型。

## 促銷活動失敗  {#campaign-failure}

促銷活動失敗會通知您智慧促銷活動中的錯誤。

## CRM同步 {#crm-sync}

CRM同步通知會提醒您CRM同步發現嚴重問題，例如權限不正確或同步中斷。

**Microsoft Dynamics**

動態通知每24小時傳送一次，並包含該時段內無法同步的銷售機會。 失敗的典型原因是重複銷售線索（如上）或欄位長度不匹配錯誤。

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

如果您使用Salesforce，同步錯誤通知看起來就像下面的通知。 典型錯誤包括過期的憑證和超出API限制。

![](assets/salesforcesyncerror.png)

參與

當串流中的線索耗盡時，我們會傳送通知。  通知包括已耗盡的銷售線索數和其他一些資訊。

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

如果您嘗試在未接受服務條款的情況下將銷售機會傳送至Facebook，或在移除Marketo應用程式後嘗試將銷售機會傳送至Facebook。

空閒觸發程式促銷活動清除

停用已觸發且不再取得任何活動的智慧型促銷活動。 深入了解  [自動觸發促銷活動清除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

LinkedIn

當Marketo在三次嘗試後無法建立新對象、登入或推送電子郵件至LinkedIn時。

![](assets/linkedin.png)

網站服務

達到每日配額時，系統會通知您。 配額在每晚午夜、中央時間重置。

>[!NOTE]
>
>您可能會收到的部分錯誤碼概述於 [開發人員檔案](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
