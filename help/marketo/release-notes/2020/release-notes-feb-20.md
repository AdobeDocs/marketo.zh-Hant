---
unique-page-id: 37355826
description: 發行說明- 2002年2月——行銷檔案——產品檔案
title: 發行說明- 2002年2月
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---


# 發行說明：Feb &#39;20 {#release-notes-feb}

2002年2月發行包含下列功能。 檢查您的Marketo版本，以取得功能。

>[!AVAILABILITY]
>
>以星號(![(star)](assets/star-yellow.svg))表示的功能是付費附加元件。 請連絡您的Marketo Engage代表以瞭解更多資訊。

**_季_** 度發行2020年2月21日發 **行下列功能**。

## 核心Marketo Engage{#core-marketo-engage}

* **Microsoft Dynamics 「Change Owner in Microsoft 」流動操作**:透過直接從Marketo Engage變更潛在客戶／連絡人擁有者的能力，維持對Microsoft Dynamics CRM資料的控制。這是對我們原生CRM整合功能的增強。
* **使用者管理API**:透過外部身分識別和組織管理系統，自動化使用者和角色管理。這是對我們API呼叫功能的增強。
* **自訂物件結構API**:在Marketo Engage中自動管理和布建跨例項的自訂物件結構描述，讓銷售和行銷工具的資料模型保持一致。使用此API，您可以在沙盒或卓越中心中定義和測試自訂物件，並視需要布建至多個例項。 這是對我們API呼叫功能的增強。 請連絡您的Marketo Engage代表，瞭解如何存取此增強功能。
* **著陸頁面重新導向規則API**:自動管理著陸頁面重新導向規則。這是對我們API呼叫功能的增強。
* **表單描述符快取**:我們透過將表單快取為資源，來縮短內嵌表單的載入時間並增強整體應用程式穩定性。請注意，對內嵌表單進行核准最多需要四分鐘，才能在Web上反映。 這是對著陸頁面與Forms功能的增強。

<br> 

**_整季發行_**

以下功能是非季度週期，將於未來數月內發佈。

## Bizible {#bizible}

![（星號）](assets/star-yellow.svg)

* **帳戶型劃分**:分析「帳戶」層級的歸因，並能夠根據「帳戶」屬性為Discover展示板建立區段和篩選器。使用這些區段深入探討您以帳戶為基礎的行銷績效。
* **儲存篩選**:儲存每位使用者專屬的控制面板特定篩選，以快速且一致地分析控制面板。
* **匯出為PDF**:將可見儀表板匯出為PDF，以分享貴組織的寶貴見解。

## 銷售連接{#sales-connect}

* **合成窗口更新**:我們已簡化透過Sales Connect選取範本和傳送電子郵件的程式。使用我們網頁用戶端和Salesforce中的「合成」視窗做為銷售者的一站式商店，可儲存範本類別、排程電子郵件、大量傳送電子郵件，以及透過檢視和點選追蹤傳送電子郵件。
* **命令中心更新**:我們正在重建Sales Connect指揮中心，讓銷售者深入瞭解他們從Sales Connect啟動的所有電子郵件、呼叫和任務。他們還可以從指揮中心查看電子郵件參與和傳遞能力等資訊。

<br> 

## 公告{#announcements}

* **Marketo Engage成功中心**:我們將於2020年2月推出行銷成功中心。成功中心是產品內協助中心，可讓您直接從您的Marketo Engage實例搜尋產品檔案和社群、啟動操作指南、存取採用內容（例如Marketo University和同儕最佳實務影片）等。 **注意**:這項功能將在澳新銀行推出為beta版，並將於本季度晚些時候推出至北美地區。

## 淘汰{#deprecations}

* **資產API &quot;_method&quot;參數**:在2020年9月之後，資產API端點將不再接受&quot;_method&quot;來傳遞POST內文中的查詢參數，以略過URI長度限制。為了容納需要此參數的請求，資產API的URI限制將從6KiB增加到65KiB，因此可提交長請求URI。
* **取代Internet Explorer支援**:從2020年7月31日發行的7月版本開始，Internet Explorer將不再支援Marketo Engage使用者介面。

**_產品發_** [行網路](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 研討會於3月3日上午11:00AM PT / 2:00PM ET加入我們，參加由我們的產品團隊主持的即時網路研討會，並進一步瞭解此版本所包含的功能。
