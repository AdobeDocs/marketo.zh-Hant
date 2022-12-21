---
description: 從您的Dynamics Campaign新增或移除人員 — Marketo檔案 — 產品檔案
title: 從Dynamics促銷活動中新增或移除人員
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 從Dynamics促銷活動中新增或移除人員 {#add-or-remove-people-from-your-dynamics-campaign}

## 新增至Dynamics Campaign {#add-to-dynamics-campaign}

此流程步驟可用於Marketo智慧型促銷活動，以在Microsoft促銷活動中將人員新增為銷售機會或聯絡人。 如果Dynamics中尚未存在銷售機會，則會自動同步該銷售機會，並新增至促銷活動。

>[!NOTE]
>
>此流量動作僅適用於觸發促銷活動。

在您的智慧型行銷活動中，尋找並選取您要新增人員的Dynamics行銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>如果您在促銷活動清單中看不到動態促銷活動：
>
>* 確認促銷活動同步功能正常
>* 促銷活動在Microsoft Dynamics中未作用


系統會自動建立促銷活動專用的靜態行銷清單，每個清單分別用於銷售機會和聯絡人，以新增人員。 這是一次性動作，且會使用相同的行銷清單，以供後續同步至促銷活動。 靜態行銷清單名稱採用的命名標準為 `Mkto-leads-<uniqueID>` 對於銷售機會和 `Mkto-contacts-<uniqueID>` 聯繫人。

將這些Marketo產生的行銷清單與其他行銷活動關聯，可能會導致混淆行為。 例如：新增至一個促銷活動也會導致新增至第二個促銷活動。 同樣地，也不建議將Marketo產生的行銷清單與Dynamics中的促銷活動分離。

## 從Dynamics Campaign中移除 {#remove-from-dynamics-campaign}

此流程步驟可用於Marketo智慧型促銷活動，以從Microsoft促銷活動中移除訪客。 這只會移除促銷活動中先前已透過「新增至Microsoft促銷活動」的流程動作新增至促銷活動的那些銷售機會。

>[!NOTE]
>
>此流量動作僅適用於觸發促銷活動。

在您的智慧型促銷活動中，尋找並選取您要移除其他人員的動態促銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>如果您在促銷活動清單中未看到動態促銷活動：
>
>* 確認促銷活動同步功能正常
>* 促銷活動在Microsoft Dynamics中未作用

