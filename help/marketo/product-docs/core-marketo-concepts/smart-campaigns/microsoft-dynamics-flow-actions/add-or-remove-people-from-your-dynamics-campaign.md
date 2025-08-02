---
description: 新增或移除您 [!DNL Dynamics] 行銷活動中的人員 — Marketo檔案 — 產品檔案
title: 從您的 [!DNL Dynamics] 行銷活動新增或移除人員
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# 從您的[!DNL Dynamics]行銷活動新增或移除人員 {#add-or-remove-people-from-your-dynamics-campaign}

## 新增至Dynamics Campaign {#add-to-dynamics-campaign}

此流程步驟可用於Marketo Engage Smart Campaigns，在Microsoft行銷活動中新增人員作為銷售機會或聯絡人。 如果Dynamics中尚未存在潛在客戶，則會自動將其同步並新增至促銷活動。

>[!NOTE]
>
>此流程動作僅適用於觸發行銷活動。

在您的Smart Campaign中，尋找並選取要新增人員的Dynamics行銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>如果您在行銷活動清單中看不到Dynamics行銷活動：
>
>* 確認Campaign同步功能正常運作
>* 行銷活動在[!DNL Microsoft Dynamics]中未啟用

系統會自動建立促銷活動專屬的靜態行銷清單，每個清單都代表銷售機會和聯絡人，以便將個人新增至。 此為一次性動作，後續同步至行銷活動時，只會使用相同的行銷清單。 靜態行銷清單名稱採用的命名標準為潛在客戶為`Mkto-leads-<uniqueID>`，聯絡人為`Mkto-contacts-<uniqueID>`。

將這些Marketo產生的行銷清單與其他行銷活動建立關聯，可能會導致混淆行為。 例如：新增至一個促銷活動也會導致新增至第二個促銷活動。 同樣地，也不建議在[!DNL Dynamics]中將Marketo產生的行銷清單與行銷活動解除關聯。

## 從Dynamics Campaign移除 {#remove-from-dynamics-campaign}

此流程步驟可用於Marketo Smart Campaigns，從Microsoft行銷活動中移除人員。 這只會從促銷活動中移除先前透過「新增至Microsoft促銷活動」的流程動作新增至促銷活動的潛在客戶。

>[!NOTE]
>
>此流程動作僅適用於觸發行銷活動。

在Smart Campaign中，尋找並選取您要移除人員的Dynamics行銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>如果您在行銷活動清單中未看見[!DNL Dynamics]行銷活動：
>
>* 確認Campaign同步功能正常運作
>* 行銷活動在[!DNL Microsoft Dynamics]中未啟用
