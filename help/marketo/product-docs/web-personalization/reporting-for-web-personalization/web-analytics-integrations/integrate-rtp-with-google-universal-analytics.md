---
unique-page-id: 4720125
description: 將RTP與Google Universal Analytics整合 — Marketo檔案 — 產品檔案
title: 將RTP與Google Universal Analytics整合
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# 將RTP與Google Universal Analytics整合 {#integrate-rtp-with-google-universal-analytics}

## 簡介 {#intro}

運用Google Universal Analytics(GUA)和Marketo Real-Time Personalization的(RTP)首頁圖形和個人化資料，以更妥善地測量和分析您的線上行銷工作。

本文說明如何設定及整合Marketo即時個人化(RTP)平台與Google Universal Analytics(GUA)帳戶。 RTP資料可附加到您的GUA帳戶，以便您查看和查看訪問您網站的組織、行業、圖形學和RTP段的效能。

**Google Universal Analytics**

Google Universal Analytics與RTP的資料可讓您更清楚了解B2B使用者如何與您的線上內容互動，並協助您測量個人化促銷活動並獲得更好的結果。 [深入了解Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**僅適用於Google Tag Manager使用者**
>
>無需編碼或特殊配置。 請務必完成下列檢查清單：
>
>* RTP維度是在Google Universal Analytics中建立
>* [RTP標籤已正確安裝在Google標籤管理器中](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* Google Universal Analytics整合會在RTP的帳戶設定中啟用
>* [Google Universal Analytics標籤已在Google標籤管理器中正確設定](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag Manager標籤已正確安裝您的網站](https://developers.google.com/tag-manager/quickstart)


## 在GUA中設定自訂Dimension {#set-up-custom-dimensions-in-gua}

1. 在Google Analytics中，

   1. 前往 **管理**
   1. 選取 **帳戶。**
   1. 選取 **屬性。**
   1. 選擇 **自訂定義** 和 **自訂Dimension**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 新增自訂維度。 按一下 **+新自訂Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 新增下列項目 **自訂Dimension:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>自訂Dimension名稱</strong></p></td> 
   <td><p><strong>範圍</strong></p></td> 
   <td><p><strong>作用中</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP — 組織</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP類別</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP組</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**自訂Dimension名稱** 必須與上表中的定義完全相同（否則GUA中的自訂RTP控制面板和報表將無法正確顯示）

1. 新增 **名稱**. 選擇範圍為 **工作階段**. 按一下 **建立**。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

您的自訂Dimension清單應如下所示。

![](assets/image2014-11-29-11-36-50-version-2.png)

在GUA中啟動自訂Dimension後，請前往RTP平台，在RTP中啟用這些維度。

## 在您的RTP帳戶中啟用GUA整合 {#activate-the-gua-integration-in-your-rtp-account}

1. 在RTP平台中，前往 **帳戶設定。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在 **帳戶設定**，按一下 **網域**.
1. 在 **Analytics**，按一下 **Google Universal Analytics**.
1. 轉彎 **開啟** 相關的自訂Dimension和事件，將此資料從RTP附加至Google Universal Analytics。
1. 輸入 **索引號** 與GUA中的索引號對齊的維。
1. 按一下 **儲存**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>可在GUA的CustomDimension下找到CustomDimension的Index Number。
>
>範例：RTP-Industry索引號等於1,RTP-Organization索引號等於2。

## 移除Google Analytics中的舊控制面板 {#remove-old-dashboards-in-google-analytics}

1. 在Google Analytics。 前往 **報告。**
1. 按一下 **控制面板。**
1. 選取 **控制面板** （RTP B2B或RTP效能）
1. 按一下 **刪除控制面板**.

![](assets/image2014-11-29-11-3a42-3a55.png)
