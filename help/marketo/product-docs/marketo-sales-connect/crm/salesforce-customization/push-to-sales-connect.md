---
unique-page-id: 14352477
description: 推送至銷售連線 — Marketo檔案 — 產品檔案
title: 推送至Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# 推送至Sales Connect {#push-to-sales-connect}

我們的「按到輸出」按鈕將在Salesforce中取得您的銷售機會/聯繫人的清單，並將他們推入Sales Connect中的組。 然後，您就可以快速傳送可自訂的群組電子郵件，並附上「輸出」追蹤。

## 需求 {#requirements}

* 由Salesforce管理員安裝的Sales Connect Salesforce包

* 按到Sales Connect按鈕，安裝該按鈕，以便由Salesforce管理員進行清單視圖

* 使用Sales Connect建立的Salesforce連接，用於進行推播的用戶

## 作法 {#how-to}

1. 按一下 **銷售機會/聯繫人** 標籤。
1. 切換到「執行」按鈕旁要「推送至銷售連接」的「清單視圖」。
1. 按一下 **開始**.
1. 選擇要推送到輸出的所有銷售機會/聯繫人。
1. 選擇 **推送至MSE**.
1. 將出現一個新窗口，驗證您要推送的銷售機會/聯繫人的數量。 選擇 **繼續到組**. Sales Connect不會推送任何在Salesforce中標示為「電子郵件選擇退出」或在Sales Connect中取消訂閱的聯絡人。

   >[!NOTE]
   >
   >Sales Connect將添加名為「SFDC-..」的組 到 [網頁應用程式](https://toutapp.com/login).

1. 選擇 **電子郵件整個群組** 發送此組電子郵件。
