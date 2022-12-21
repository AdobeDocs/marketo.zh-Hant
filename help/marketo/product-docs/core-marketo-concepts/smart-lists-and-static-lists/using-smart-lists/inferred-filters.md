---
unique-page-id: 2953188
description: 推斷篩選器 — Marketo檔案 — 產品檔案
title: 推斷的篩選器
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
source-git-commit: c045e9008bf0e9d145ac67866a1e0d7cb6e26069
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 推斷的篩選器 {#inferred-filters}

當有人瀏覽您的網站時， [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 將它們加入系統。 我們在一個特殊的資料庫中查找他們的IP，並推斷出各種好的資訊。

>[!NOTE]
>
>為確保推斷的欄位值保持最新，我們會定期更新用於IP地址查閱的資料庫。 資料庫更新可引入新的推斷欄位值，您可能需要將這些值添加到智慧清單篩選器定義中。
>
>資料庫更新可能發生在 [Marketo Engage產品發行](/help/marketo/release-notes/release-schedule.md){target=&quot;_blank&quot;}。 更新發生時， [Marketo Engage發行說明](/help/marketo/release-notes/current.md){target=&quot;_blank&quot;}將包含對推斷欄位值所做任何變更的說明。

![](assets/image2015-4-27-13-3a25-3a46.png)

![](assets/image2015-4-27-16-3a58-3a53.png)

![](assets/image2015-4-27-16-3a59-3a35.png)

![](assets/image2015-4-27-17-3a0-3a12.png)

![](assets/image2015-4-27-13-3a36-3a9.png)

![](assets/image2015-4-27-13-3a30-3a48.png)

當您在智慧清單中使用其中任何一個篩選器時，結果會產生具有這個推斷資訊的使用者。

>[!TIP]
>
>在網頁活動報表中使用這些篩選器。 使用銷售代表的地區，並在過去24小時內向網站訪客訂購自定義的每日報告。 他們會喜歡的！
>
>* 已瀏覽網頁 — 最近24小時
>* 推斷狀態為 [選擇其領土]


這些匿名訪客在點按電子郵件連結或填寫表單時，會自動轉換成人員。 然而，它們保留了所有推斷的資訊。

>[!NOTE]
>
>深入了解 [匿名活動和銷售機會](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md).
