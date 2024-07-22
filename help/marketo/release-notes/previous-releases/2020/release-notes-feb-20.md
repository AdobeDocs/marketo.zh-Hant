---
unique-page-id: 37355826
description: 發行說明–2020年2月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年2月
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 發行說明： 2020年2月 {#release-notes-feb}

2020年2月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![（星號）](assets/yellow-star.png))表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**&#x200B;下列功能已於&#x200B;**2020年2月21日發行**。

## 核心Marketo Engage {#core-marketo-engage}

* **Microsoft Dynamics「在Microsoft中變更擁有者」流程動作**：保持對Microsoft Dynamics CRM資料的控制權，並直接從Marketo Engage變更銷售機會/連絡擁有者。 這是原生CRM整合功能的增強功能。
* **使用者管理API**：透過外部身分識別與組織管理系統，自動管理使用者與角色。 這是我們API呼叫功能的增強功能。
* **自訂物件結構描述API**：在Marketo Engage中自動跨執行個體管理和布建自訂物件結構描述，以保持銷售和行銷工具中的資料模型一致。 透過此API，您可以在沙箱或卓越中心中定義及測試自訂物件，並視需要布建至任意數量的執行個體。 這是我們API呼叫功能的增強功能。 請聯絡您的Marketo Engage代表以瞭解如何存取此增強功能。
* **登陸頁面重新導向規則API**：自動管理登陸頁面重新導向規則。 這是我們API呼叫功能的增強功能。
* **表單描述元快取**：我們將透過快取表單作為資源來減少內嵌表單的載入時間，並提升整體應用程式穩定性。 請注意，對內嵌式表單的核准，最多可能需要四分鐘才能反映在網路上。 這是登陸頁面和Forms功能的增強功能。

<br> 

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## Bizible {#bizible}

![（星形）](assets/yellow-star.png)

* **以帳戶為基礎的分段**：分析帳戶層級的歸因，並有能力根據帳戶屬性建立區段和篩選器以探索看板。 使用這些區段來深入瞭解以帳戶為基礎的行銷績效。
* **儲存篩選器**：儲存每個使用者專屬的儀表板特定篩選器，以快速且一致地分析您的儀表板。
* **匯出至PDF**：將Bizible儀表板匯出為PDF，以在整個組織內共用有價值的深入分析。

## Sales Connect {#sales-connect}

* **撰寫視窗更新**：我們已簡化透過Sales Connect選取範本及傳送電子郵件的程式。 在我們的網頁使用者端和Salesforce中使用撰寫視窗，作為賣家的一站式商店，能夠儲存範本類別、排程電子郵件、大量傳送電子郵件，以及傳送包含檢視和點選追蹤的電子郵件。
* **指揮中心更新**：我們正在重建Sales Connect指揮中心，以便讓賣家深入瞭解其所有電子郵件、通話和從Sales Connect啟動的工作。 他們也可以從指揮中心檢視電子郵件參與度和傳遞能力等資訊。

<br> 

## 公告 {#announcements}

* **Marketo Engage成功中心**：我們將在2020年2月啟動Marketo成功中心。 Success Center是產品內的說明中心，可讓您搜尋產品檔案和社群、啟動操作指南、存取採用內容(例如Marketo University和同儕最佳實務影片)等，直接從您的Marketo Engage執行個體進行。 **注意**：此功能將會以測試版的形式在澳新銀行推出，並預計於本季末在北美地區推出。

## 淘汰 {#deprecations}

* **資產API「_method」引數**： 2020年9月後，資產API端點將不再接受於POST主體中使用「_method」傳遞查詢引數，以略過URI長度限制。 為因應需要此引數的請求，資產API的URI限制將從6KiB增加到65KiB，以便提交較長的請求URI。
* **Internet Explorer支援淘汰**：從2020年7月31日推出的七月版開始，Internet Explorer將不再支援Marketo Engage使用者介面。

**_產品發行網路研討會_** [於3月3日上午11:00點/下午2:00點（東部時間）加入我們](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html)，參加我們產品團隊舉辦的即時網路研討會，並深入瞭解此發行版本包含的功能。
