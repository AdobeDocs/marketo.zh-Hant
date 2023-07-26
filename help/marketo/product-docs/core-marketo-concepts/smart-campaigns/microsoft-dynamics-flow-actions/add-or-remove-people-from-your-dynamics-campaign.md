---
description: 在Dynamics Campaign中新增或移除人員 — Marketo檔案 — 產品檔案
title: 新增或移除Dynamics行銷活動中的人員
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 新增或移除Dynamics行銷活動中的人員 {#add-or-remove-people-from-your-dynamics-campaign}

## 新增至Dynamics Campaign {#add-to-dynamics-campaign}

此流程步驟可用於Marketo Smart Campaigns，在Microsoft行銷活動中新增人員作為銷售機會或聯絡人。 如果Dynamics中尚未存在潛在客戶，則會自動將其同步並新增至促銷活動。

>[!NOTE]
>
>此流程動作僅適用於觸發行銷活動。

在您的智慧行銷活動中，尋找並選取您要將人員新增到其中的Dynamics行銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>如果您在行銷活動清單中看不到Dynamics行銷活動：
>
>* 確認Campaign同步功能正常運作
>* 此行銷活動在Microsoft Dynamics中無效

系統會自動建立行銷活動專屬的靜態行銷清單，每個清單都代表銷售機會和聯絡人，以便將個人新增至。 此為一次性動作，後續同步至行銷活動時，只會使用相同的行銷清單。 靜態行銷清單名稱所採用的命名標準為 `Mkto-leads-<uniqueID>` 潛在客戶和 `Mkto-contacts-<uniqueID>` 連絡人的資訊。

將這些Marketo產生的行銷清單與其他行銷活動建立關聯，可能會導致混淆行為。 例如：新增至一個促銷活動也會導致新增至第二個促銷活動。 同樣地，也不建議在Dynamics中將Marketo產生的行銷清單與Campaign解除關聯。

## 從Dynamics Campaign移除 {#remove-from-dynamics-campaign}

此流程步驟可用於Marketo Smart Campaigns，從Microsoft行銷活動中移除人員。 這只會從促銷活動中移除先前透過「新增至Microsoft促銷活動」的流程動作新增至促銷活動的潛在客戶。

>[!NOTE]
>
>此流程動作僅適用於觸發行銷活動。

在您的智慧行銷活動中，尋找並選取您要移除人員的Dynamics行銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>如果行銷活動清單中未顯示Dynamics行銷活動：
>
>* 確認Campaign同步功能正常運作
>* 此行銷活動在Microsoft Dynamics中無效
