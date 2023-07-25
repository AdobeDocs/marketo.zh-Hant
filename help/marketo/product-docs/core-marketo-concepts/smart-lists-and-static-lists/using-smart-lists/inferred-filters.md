---
unique-page-id: 2953188
description: 推斷的篩選器 — Marketo檔案 — 產品檔案
title: 推斷的篩選器
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 推斷的篩選器 {#inferred-filters}

有人造訪您的網站時， [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 對資料進行Cookie處理，然後將其放入系統中。 我們會在特殊的資料庫中查詢他們的IP，並推斷出各種良好的資訊。

>[!NOTE]
>
>為確保推斷的欄位值保持最新狀態，我們會定期更新用於IP位址查詢的資料庫。 資料庫更新可能會引入新的推斷欄位值，您可能需要將這些值新增到智慧清單篩選定義中。
>
>資料庫更新可能發生在 [Marketo Engage產品發行](/help/marketo/release-notes/release-schedule.md){target="_blank"}. When an update does occur, the [Marketo Engage release notes](/help/marketo/release-notes/current.md){target="_blank"} 將包含推斷欄位值之任何變更的說明。

![](assets/image2015-4-27-13-3a25-3a46.png)

![](assets/image2015-4-27-16-3a58-3a53.png)

![](assets/image2015-4-27-16-3a59-3a35.png)

![](assets/image2015-4-27-17-3a0-3a12.png)

![](assets/image2015-4-27-13-3a36-3a9.png)

![](assets/image2015-4-27-13-3a30-3a48.png)

當您在智慧清單中使用任何這些篩選器時，結果會產生具有此推斷資訊的人員。

>[!TIP]
>
>在網頁活動報表中使用這些篩選器。 使用銷售代表的區域，並將其訂閱給網站訪客在過去24小時內的自訂每日報表。 他們一定會喜歡！
>
>* 造訪的網頁 — 過去24小時
>* 推斷的狀態為 [選取其地區]

這些匿名訪客在點按電子郵件連結或填寫表單時，會自動轉換為人員。 但是會保留所有推斷的資訊。

>[!NOTE]
>
>進一步瞭解 [匿名活動和潛在客戶](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md).
