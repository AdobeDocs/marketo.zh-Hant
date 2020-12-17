---
unique-page-id: 2953243
description: 通知類型——行銷檔案——產品檔案
title: 通知類型
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# 通知類型{#notification-types}

有幾種通知類型。

## 促銷活動失敗{#campaign-failure}

促銷活動失敗會通知您智慧型促銷活動中的錯誤。

## CRM同步{#crm-sync}

CRM同步通知會提醒您CRM同步發現的重大問題，例如權限不正確或同步中斷。

**Microsoft Dynamics**

動態通知每24小時傳送一次，並包含該時段內無法同步的銷售機會。 失敗的典型原因是重複銷售線索（如上所示）或欄位長度不符錯誤。

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

如果您使用Salesforce，同步錯誤通知的外觀會類似下方。 典型錯誤包括過期的憑證和超出的API限制。

![](assets/salesforcesyncerror.png)

參與

當潛在客源在串流中耗盡時，我們會傳送通知。  通知包括已經筋疲力盡的銷售線索數和其他資訊。

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

如果您嘗試在未接受服務條款的情況下將潛在客戶傳送至Facebook，或是在移除Marketo應用程式後嘗試將潛在客戶傳送至Facebook。

閒置觸發器促銷活動清除

停用已觸發的智慧型促銷活動，而不會再收到任何活動。 進一步瞭解[自動觸發促銷活動清除](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)。

LinkedIn

當Marketo嘗試三次後無法建立新對象、登入或推送電子郵件至LinkedIn時。

![](assets/linkedin.png)

網站服務

當您達到每日配額時，將會通知您。 配額會在午夜（中央時間）每晚重設。

>[!NOTE]
>
>我們的[開發人員檔案](http://developers.marketo.com/rest-api/error-codes/#response_level_error_codes)中概述了您可能收到的部分錯誤碼。

