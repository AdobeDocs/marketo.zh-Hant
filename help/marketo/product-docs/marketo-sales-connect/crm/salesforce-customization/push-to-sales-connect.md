---
unique-page-id: 14352477
description: 推送至銷售連線——行銷人員檔案——產品檔案
title: 推送至Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# 推送至Sales Connect {#push-to-sales-connect}

我們的「推送至成品」按鈕會在Salesforce中列出您的潛在客戶／聯絡人，並將它們推入Sales Connect的群組。 然後，您就可以快速傳送附有Tout追蹤的可自訂群組電子郵件。

## 需求 {#requirements}

* Sales Connect [Salesforce套件](http://docs.marketo.com/x/C4PS) ，安裝者 `Salesforce Admin`

* `Push to Sales Connect`按鈕，列出查看依據 `Salesforce Admin`

* 使用Sales Connect建立的Salesforce連線，適用於進行推播的使用者

## 如何 {#how-to}

1. 按一下Salesforce **中的** 「銷售機會／連絡人」標籤。
1. 切換至「執行」按鈕旁的「推送至銷售連線」清單檢視。
1. 按一 **下開始**。
1. 選擇要推送到成品的所有銷售線索／聯繫人。
1. 選擇 **推送至MSE**。
1. 將出現一個新窗口，驗證您要推送的銷售線索／聯繫人數。 選擇 **繼續到組**。 Sales Connect `will not push over` Salesforce或Sales Connect中標示 `Email Opt Out` 的任何 `Unsubscribed` 連絡人。

   >[!NOTE]
   >
   >Sales Connect將添加名為&quot;SFDC-..&quot;的組 至Web應用程式上的「關 [系」頁面](http://toutapp.com/login)。

1. 選擇「 **以電子郵件傳送整個群組** 」以傳送此群組電子郵件。

