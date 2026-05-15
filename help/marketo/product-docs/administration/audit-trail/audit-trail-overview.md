---
unique-page-id: 11377945
description: 稽核軌跡概觀，以及它如何在Marketo執行個體中擷取六個月變更和登入活動的歷史記錄。
title: 稽核軌跡概觀
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
TQID: https://experienceleague.adobe.com/4MTpv09ZFWkX6tirnq7ZIABSkfoz07qljcUUORwYNn8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 2%

---

# 稽核軌跡概觀 {#audit-trail-overview}

稽核軌跡可讓您取得Marketo執行個體中所做的變更的完整歷史記錄（六個月）。

>[!NOTE]
>
>稽核軌跡資料歷程記錄開始於2016年9月14日。

![](assets/audit-trail-overview-1.png)

## 什麼是稽核軌跡 {#what-is-audit-trail}

稽核軌跡可以即時擷取Marketo訂閱中發生之動作和事件的完整清單。 功能包括自助式存取六個月的資料歷史記錄，以協助回答下列問題：

「此資產或設定有什麼改變，上次更新的是誰？」

「使用者X最近做了什麼？」

「誰正在登入我們的帳戶？」

## 我們稽核的專案 {#what-we-audit}

Marketo稽核下列專案的[建立、編輯和刪除](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md)動作：

* Design Studio資產
* 所有Marketo計畫
* 智慧行銷活動
* 清單（智慧/靜態）
* 使用者（管理員）
* 角色和許可權（管理員）
* Workspace與資料分割（管理員）
* 使用者登入記錄

>[!NOTE]
>
>Marketo目前正在&#x200B;_非_&#x200B;稽核在Web Personalization、預測性內容或銷售Insight中所做的變更。

## 稽核軌跡元件 {#audit-trail-components}

稽核軌跡包含三個元件。

**1) [資產稽核軌跡](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

請參閱對特定資產完成的活動。

**2) [管理員稽核軌跡](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

監視以使用者為基礎的詳細資訊。

**3) [使用者登入歷程記錄](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

檢視哪些人一直在登入您的訂閱以及何時登入（也包括失敗的登入嘗試）。

>[!TIP]
>
>因為您可以使用「稽核軌跡」稽核太多了，[篩選](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)可以節省大量時間。

## 匯出資料 {#exporting-data}

您只能檢視執行個體中30天的資料。 若要取得（最多）六個月的值，請使用匯出選項。

![](assets/two.png)

>[!NOTE]
>
>**定義**
>
>**未知：**&#x200B;在[!DNL Webhook]中，您可能會看到使用者的名稱和電子郵件列為「未知」。 當您變更CRM中的挑選清單值時，就會發生此狀況。 這些值會顯示在Marketo表單和登入頁面中。 在CRM端執行此更新將會自動草稿您的登入頁面參考表單。 在[!DNL Webhook]中，Marketo擷取登入頁面為草稿，但使用者的名稱和電子郵件將顯示為「未知」，因為Marketo無法從CRM端擷取使用者資訊。

>[!MORELIKETHIS]
>
>[啟用稽核軌跡](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
