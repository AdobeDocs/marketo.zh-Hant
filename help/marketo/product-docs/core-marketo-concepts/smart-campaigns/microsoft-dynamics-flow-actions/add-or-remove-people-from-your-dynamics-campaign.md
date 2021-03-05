---
description: 從Dynamics Campaign —— 行銷人員檔案——產品檔案新增或移除人員
title: 從動態促銷活動新增或移除人員
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# 從動態促銷活動中新增或移除人員{#add-or-remove-people-from-your-dynamics-campaign}

## 新增至Dynamics促銷活動{#add-to-dynamics-campaign}

此流程步驟可用於Marketo Smart促銷活動，以新增人員作為Microsoft促銷活動中的潛在客戶或連絡人。 如果銷售機會尚未在Dynamics中存在，則會自動同步該銷售機會並新增至促銷活動。

>[!NOTE]
>
>此流量動作僅適用於「觸發促銷活動」。

在智慧型促銷活動中，尋找並選取您要新增人員的動態促銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>如果您在促銷活動清單中看不到動態促銷活動：
>
>* 確定促銷活動同步功能正常
>* 促銷活動在Microsoft Dynamics中未作用中


系統會自動建立促銷活動專用的靜態行銷清單，每個清單分別用於銷售機會和連絡人，以新增人員至。 這是一次性動作，後續同步至促銷活動的一次，會使用相同的行銷清單。 靜態行銷清單名稱採用的命名標準為銷售機會`Mkto-leads-<uniqueID>`和聯繫人`Mkto-contacts-<uniqueID>`。

將這些行銷人員產生的行銷清單與其他行銷活動產生關聯，可能會導致行為混亂。 例如：新增至一個促銷活動也會導致新增至第二個促銷活動。 同樣地，也不建議將行銷人員產生的行銷清單與Dynamics中的行銷活動分離。

## 從Dynamics促銷活動移除{#remove-from-dynamics-campaign}

此流程步驟可用於Marketo Smart促銷活動，以移除Microsoft促銷活動中的人員。 這只會移除先前透過「新增至Microsoft促銷活動」的流程動作新增至促銷活動的促銷活動中那些潛在客戶。

>[!NOTE]
>
>此流量動作僅適用於「觸發促銷活動」。

在智慧型促銷活動中，尋找並選取您要移除其他人的動態促銷活動。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>如果您在促銷活動清單中未看到動態促銷活動：
>
>* 確定促銷活動同步功能正常
>* 促銷活動在Microsoft Dynamics中未作用中

