---
unique-page-id: 2949158
description: 將RTP與Google Analytics整合 — Marketo檔案 — 產品檔案
title: 將RTP與Google Analytics整合
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# 將RTP與Google Analytics整合 {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics現在是作業標準，而且Google中的所有屬性都已升級為Universal Analytics。
>
>本文會說明如何使用舊版Google Standard Analytics，但建議您改用Universal Analytics。
>
>如果您尚未使用[analytics.js追蹤程式碼](https://developers.google.com/analytics/devguides/collection/analyticsjs/)，Google強烈建議您重新標籤網站以使用。 Google已棄用下列專案：
>
>* ga.js
>* urchin.js
>* WAP/伺服器端代碼片段
>* YT / MO
>* 自訂變數
>* 使用者定義的變數
>
>瞭解如何將[Web Personalization與Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)整合

## 簡介 {#introduction}

使用從Marketo Real-Time Personalization (RTP)到Google Analytics(GA)帳戶的直接資料流，從新角度分析您的網站分析。 根據組織、產業和RTP行銷活動，在GA中測量您的網站造訪。 檢視量度，例如GA中的產業型別或RTP區段，以及這些量度如何根據不同的流量來源（社交、付費、有機）執行和產生銷售機會、分析行銷活動的點進率，以及衡量個人化行銷活動對您網站的影響。 利用此功能從您的RTP帳戶中獲得最大利益

**RTPAudience Analytics**

透過整合，您在GA帳戶中擁有新維度。 RTP會透過以下功能自動增強您的儀表板：

1. 組織和產業
1. RTP中的自訂區段
1. Account-Based Marketing清單

專注於您的關鍵B2B潛在客戶。 依目標產業和區段分析管道。

## 管道報表 {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

RTP B2B儀表板可協助您根據垂直和RTP細分瞭解訪客的劃分情形。 您可以根據金融業和不同的行銷活動（付費、自然、社交）檢視訪客成效。 控制面板也提供RTP區段執行方式的高層級概觀，並向下鑽研以顯示造訪您網站的排名最前的組織。

## 行為流量 {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

行為流量報表（請參閱影像）可視覺化訪客從一個頁面或事件移動至下一個頁面的路徑。 此影像範例顯示金融領域所有訪客的路徑。 此報表可協助您探索哪些內容可讓訪客持續參與您的網站。

## RTP效能 {#rtp-performance}

衡量您的RTP行銷活動，並將其與整體網站平均值建立關聯。 瞭解這些行銷活動如何影響您的網站量度，並使用此資料將您的個人化工作聚焦於正確的目標。 產生自訂報表，以便更清楚瞭解個人化行銷活動的執行情形。

![](assets/image2014-11-28-16-3a47-3a0.png)

## 使用Google Analytics設定RTP {#setting-up-rtp-with-google-analytics}

1. 將電子郵件rtp.ga2@gmail.com作為讀取和分析使用者新增到您的GA帳戶。 如需詳細資訊，請參閱[這裡](https://support.google.com/analytics/answer/2884495?hl=en)。

1. 在您的RTP帳戶中。 移至&#x200B;**帳戶設定**。

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. 在&#x200B;**帳戶設定**、**網域**&#x200B;和&#x200B;**Analytics**&#x200B;之下。

1. 按一下&#x200B;**Google Analytics**。

1. 開啟相關的&#x200B;**自訂變數**&#x200B;和&#x200B;**事件**，將此資料從RTP附加至Google Analytics。

1. 輸入&#x200B;**插槽**&#x200B;編號以傳送自訂變數資料（預設為1,2）。

![](assets/image2014-11-28-17-3a0-3a17.png)

1. 按一下&#x200B;**保存**。

>[!NOTE]
>
>若要將區段資料傳送至GA，請在RTP平台中的[編輯區段頁面](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)下選取核取方塊&#x200B;**傳送事件至區段比對上的Google Analytics**。

## 設定包含RTP資料的Google Analytics報表 {#setting-up-google-analytics-reports-with-rtp-data}

在Google Analytics中，您可以使用控制面板、GA細分和報表來檢視RTP資料：

* [儀表板](https://support.google.com/analytics/answer/1068216?hl=en)提供網站效能的概觀。
* GA區段旨在篩選GA介面中的訪客，並檢視每個區段的流量。 在[這裡](https://support.google.com/analytics/answer/3124493?hl=en)瞭解如何建立區段。
* 建立[自訂報告](https://support.google.com/analytics/answer/1033013?hl=en)以檢視和/或設定排程電子郵件。 請參閱「自訂>新增自訂報表」中的。
