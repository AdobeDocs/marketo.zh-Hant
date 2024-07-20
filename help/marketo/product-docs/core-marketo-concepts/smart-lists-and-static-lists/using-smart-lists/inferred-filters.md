---
unique-page-id: 2953188
description: 推斷的篩選器 — Marketo檔案 — 產品檔案
title: 推斷的篩選器
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# 推斷的篩選器 {#inferred-filters}

當有人造訪您的網站時，[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}會對其進行Cookie並將其放入系統中。 我們會在特殊資料庫中查詢他們的IP，並推斷各種資訊。

>[!NOTE]
>
>為確保推斷的欄位值保持最新狀態，我們會定期更新用於IP位址查詢的資料庫。 資料庫更新可能會引入新的推斷欄位值，您可能需要將這些值新增到智慧列示篩選器定義中。
>
>資料庫更新可以在[Marketo Engage的產品版本](/help/marketo/release-notes/release-schedule.md){target="_blank"}期間進行。 當更新發生時，[Marketo Engage發行說明](/help/marketo/release-notes/current.md){target="_blank"}將包含推斷欄位值之任何變更的說明。

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

當您在智慧清單中使用這些篩選器時，結果會產生具有此推斷資訊的人員。

>[!TIP]
>
>在網頁活動報表中使用這些篩選器。 使用銷售代表的區域，並將他們訂閱給過去24小時內有網站訪客的自訂每日報表。 他們一定會喜歡！
>
>* 造訪的網頁 — 過去24小時
>* 推斷的狀態是[選取其區域]

這些匿名訪客在按一下電子郵件連結或填寫表單時，會自動轉換為人員。 但是，它們會保留所有推斷的資訊。

>[!NOTE]
>
>深入瞭解[匿名活動和潛在客戶](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}。
