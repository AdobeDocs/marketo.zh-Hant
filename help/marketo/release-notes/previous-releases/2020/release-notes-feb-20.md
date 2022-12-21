---
unique-page-id: 37355826
description: 發行說明 — 2020年2月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年2月
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 發行說明：』20年2月 {#release-notes-feb}

』20年2月發行包含下列功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號表示的特徵( ![（星號）](assets/yellow-star.png))是付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每季發行_** 下列功能已於 **2020年2月21日**.

## 核心Marketo Engage {#core-marketo-engage}

* **Microsoft Dynamics「在Microsoft中變更擁有者」流量動作**:保持對Microsoft Dynamics CRM資料的控制，並能直接從Marketo Engage變更銷售機會/連絡擁有者。 這是我們原生CRM整合功能的增強功能。
* **使用者管理API**:透過外部身分和組織管理系統，自動管理使用者和角色。 這是對API呼叫功能的增強。
* **自訂物件結構API**:在Marketo Engage中，自動管理和布建跨例項的自訂物件結構，讓資料模型在銷售和行銷工具中保持一致。 透過此API，您可以在沙箱或英才中心中定義和測試自訂物件，並視需要布建至所有例項。 這是對API呼叫功能的增強。 請連絡您的Marketo Engage代表，以了解如何存取此增強功能。
* **登陸頁面重新導向規則API**:自動管理登錄頁面重新導向規則。 這是對API呼叫功能的增強。
* **表單描述符快取**:我們正在通過將表單快取為資源，減少嵌入表單的載入時間，並增強整體應用程式的穩定性。 請注意，對內嵌表單進行核准最多需要四分鐘時間，才能在網路上反映。 這是對登錄頁面與Forms功能的增強。

<br> 

**_整季推出_**

下列功能屬於非季度週期，將在未來數月內發行。

## Bizible {#bizible}

![（星號）](assets/yellow-star.png)

* **帳戶型細分**:在「帳戶」層級分析歸因，並能根據「帳戶」屬性為Discover展示板建立區段和篩選器。 使用這些區段來深入鑽研您的帳戶型行銷績效。
* **儲存篩選器**:儲存每位使用者專屬的控制面板特定篩選，以快速且一致地分析控制面板。
* **匯出至PDF**:將Bizible Dashboard匯出為PDF，以在組織間分享寶貴的深入分析。

## Sales Connect {#sales-connect}

* **撰寫視窗更新**:我們已簡化透過Sales Connect選取範本和傳送電子郵件的程式。 使用我們網頁用戶端中的「撰寫」視窗，Salesforce可供銷售者一站式使用，以儲存範本類別、排程電子郵件、大量傳送電子郵件，以及透過檢視和點擊追蹤傳送電子郵件。
* **命令中心更新**:我們正在重建Sales Connect指揮中心，以便讓銷售者了解從Sales Connect啟動的所有電子郵件、呼叫和任務。 他們還可以從指揮中心查看電子郵件參與和傳遞等資訊。

<br> 

## 公告 {#announcements}

* **Marketo Engage成功中心**:我們將於2020年2月推出Marketo成功中心。 Success Center是產品內的說明中心，可讓您直接從Marketo Engage執行個體搜尋產品檔案和社群、啟動操作指南、存取採用內容(例如Marketo大學和同儕最佳實務影片)等。 **附註**:此功能將在澳新銀行測試版推出，並將於本季末在北美地區推出。

## 淘汰 {#deprecations}

* **資產API「_method」參數**:2020年9月後，資產API端點將不再接受「_method」在POST內文中傳遞查詢參數，以略過URI長度限制。 為了適應需要此參數的請求，資產API的URI限制將從6KiB增加到65KiB，以便可以提交長請求URI。
* **不再支援Internet Explorer**:自2020年7月31日的發行版本開始，Internet Explorer將不再支援Marketo Engage使用者介面。

**_產品發行網路研討會_** [加入我們](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 3月3日上午11:00 PT /下午2:00 ET，由我們的產品團隊主持的線上網路研討會，深入了解此版本包含的功能。
