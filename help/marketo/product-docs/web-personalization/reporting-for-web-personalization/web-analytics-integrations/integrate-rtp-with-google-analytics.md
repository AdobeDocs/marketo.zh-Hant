---
unique-page-id: 2949158
description: 將RTP與Google Analytics整合 — Marketo檔案 — 產品檔案
title: 將RTP與Google Analytics整合
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 將RTP與Google Analytics整合 {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics現在是作業標準，Google中的所有屬性皆已升級至Universal Analytics。
>
>本文說明如何使用舊版Google Standard Analytics，但建議您切換至Universal Analytics。
>
>如果您尚未使用 [analytics.js追蹤程式碼](https://developers.google.com/analytics/devguides/collection/analyticsjs/), Google強烈建議您重新標籤網站以使用。 下列項目已遭Google淘汰：
>
>* ga.js
>* urchin.js
>* WAP/伺服器端片段
>* YT / MO
>* 自訂變數
>* 使用者定義的變數
>
>了解如何整合 [使用Universal Analytics進行網頁個人化](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## 簡介 {#introduction}

使用從Marketo即時個人化(RTP)直接資料流量，從新的角度分析網路分析至Google Analytics(GA)帳戶。 根據組織、產業和RTP促銷活動，以GA衡量您的網路造訪。 檢視量度，例如GA中的產業類型或RTP區段，以及它們如何根據不同的流量來源（社交、付費、自然）執行和產生銷售機會，分析促銷活動的點進率，以及測量個人化促銷活動對您網站的影響。 利用此功能，即可從您的RTP帳戶中獲得最大的好處

**RTPAudience Analytics**

透過整合，您的GA帳戶中會有新維度。 RTP會透過下列功能自動增強控制面板：

1. 組織與產業
1. RTP中的自訂區段
1. Account-Based Marketing清單

專注於您的關鍵B2B潛在客戶。 依目標產業和區段分析管道。

## 管道報表 {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

RTP B2B控制面板可協助您了解根據垂直市場和RTP細分的訪客劃分。 您可以根據金融業和不同的行銷活動（付費、自然、社交）來查看訪客績效。 控制面板也提供RTP區段執行方式的概觀，並向下演習以顯示造訪您網站的最上層組織。

## 行為流程 {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

「行為流量」報表（請參閱影像）可視覺化訪客從一個頁面或事件到下一個頁面的路徑。 影像範例顯示金融部門所有訪客的路徑。 此報告可協助您探索讓訪客持續參與您網站的內容。

## RTP效能 {#rtp-performance}

測量您的RTP促銷活動，並將其與您整體網站平均值產生關聯。 了解這些行銷活動如何影響您的網站量度，並使用此資料將個人化工作聚焦於正確的目標。 產生自訂報表，以更清楚了解個人化促銷活動的執行方式。

![](assets/image2014-11-28-16-3a47-3a0.png)

## 使用Google Analytics設定RTP {#setting-up-rtp-with-google-analytics}

1. 將電子郵件rtp.ga2@gmail.com新增為Read &amp; Analyze使用者至您的GA帳戶。 如需詳細資訊，請參閱 [此處](https://support.google.com/analytics/answer/2884495?hl=en).

1. 在您的RTP帳戶中。 前往 **帳戶設定**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. 在 **帳戶設定**, **網域** 和 **Analytics**.

1. 按一下 **Google Analytics**.

1. 開啟相關 **自訂變數** 和 **事件** 將此資料從RTP附加至Google Analytics。

1. 輸入 **插槽** 傳送自訂變數資料的數字（預設為1,2）。

![](assets/image2014-11-28-17-3a0-3a17.png)

1. 按一下 **儲存**.

>[!NOTE]
>
>若要將區段資料傳送至GA，請在 [編輯區段頁面](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) 在RTP平台中，選取核取方塊 **傳送區段比對的Google Analytics至事件**.

## 使用RTP資料設定Google Analytics報表 {#setting-up-google-analytics-reports-with-rtp-data}

在Google Analytics中，您可以使用控制面板、GA分段和報告來檢視您的RTP資料：

* [控制面板](https://support.google.com/analytics/answer/1068216?hl=en) 提供網站效能的概觀。
* GA區段的用途是在GA介面中篩選訪客，並檢視每個區段的流量。 了解如何建立區段 [此處](https://support.google.com/analytics/answer/3124493?hl=en).
* 建立 [自訂報告](https://support.google.com/analytics/answer/1033013?hl=en) 檢視和/或設定排程電子郵件。 請參閱「自訂>新增自訂報表」下方的。
