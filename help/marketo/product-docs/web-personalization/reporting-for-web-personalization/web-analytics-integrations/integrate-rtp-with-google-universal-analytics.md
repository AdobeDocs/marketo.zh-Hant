---
unique-page-id: 4720125
description: 將RTP與Google Universal Analytics整合 — Marketo檔案 — 產品檔案
title: 將RTP與Google Universal Analytics整合
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# 將RTP與Google Universal Analytics整合 {#integrate-rtp-with-google-universal-analytics}

## 介紹 {#intro}

善用Google Universal Analytics (GUA)與Marketo Real-Time Personalization (RTP)的影像和個人化資料，以更好地測量和分析您的線上行銷工作。

本文說明如何設定Marketo即時個人化(RTP)平台，並將其與Google Universal Analytics (GUA)帳戶整合。 RTP資料可附加至您的GUA帳戶，讓您檢視並檢視瀏覽您網站的組織、產業、電影和RTP區段的效能。

**Google Universal Analytics**

Google Universal Analytics搭配RTP的資料，可讓您更瞭解B2B使用者如何與您的線上內容互動，並有助於衡量個人化行銷活動並取得更好的結果。 [深入瞭解Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**僅適用於Google標籤管理員使用者**
>
>無需執行編碼或特殊設定。 請務必完成下列檢查清單：
>
>* RTP維度是在Google Universal Analytics中建立
>* [Google Tag Manager已正確安裝RTP標籤](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* 已在RTP的帳戶設定中啟用Google Universal Analytics整合
>* [Google Universal Analytics標籤已在Google Tag Manager中正確設定](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag Manager標籤已正確安裝您的網站](https://developers.google.com/tag-manager/quickstart)

## 在GUA中設定自訂Dimension {#set-up-custom-dimensions-in-gua}

1. 在Google Analytics中，

   1. 前往 **管理員**
   1. 選取 **帳戶。**
   1. 選取 **屬性。**
   1. 選取 **自訂定義** 和 **自訂Dimension**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 新增自訂維度。 按一下 **+新增自訂Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 新增下列專案 **自訂Dimension：**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>自訂Dimension名稱</strong></p></td> 
   <td><p><strong>範圍</strong></p></td> 
   <td><p><strong>作用中</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP組織</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓ (N)</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP產業</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP — 類別</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP群組</strong></p></td> 
   <td><p>工作階段</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**自訂Dimension名稱** 必須與上表中的定義完全相同（否則GUA中的自訂RTP儀表板和報告將無法正確顯示）

1. 新增 **名稱**. 選取範圍為 **工作階段**. 按一下 **建立**。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

您的自訂Dimension清單應如下所示。

![](assets/image2014-11-29-11-36-50-version-2.png)

在GUA中啟動自訂Dimension後，請前往RTP平台以在RTP中啟用這些維度。

## 在您的RTP帳戶中啟用GUA整合 {#activate-the-gua-integration-in-your-rtp-account}

1. 在RTP平台中，前往 **帳戶設定。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 下 **帳戶設定**，按一下 **網域**.
1. 下 **分析**，按一下 **Google Universal Analytics**.
1. 翻轉 **開啟** 相關自訂Dimension和事件，可將此資料從RTP附加至Google Universal Analytics。
1. 輸入 **索引編號** 與GUA中的索引編號對齊的維度的。
1. 按一下 **儲存**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>自訂Dimension的索引編號可在GUA中的「自訂Dimension」下找到。
>
>範例：RTP產業索引編號等於1，RTP組織索引編號等於2。

## 移除Google Analytics中的舊儀表板 {#remove-old-dashboards-in-google-analytics}

1. 在Google Analytics中。 前往 **報告。**
1. 按一下 **儀表板。**
1. 選取 **儀表板** （RTP B2B或RTP效能）
1. 按一下 **刪除儀表板**.

![](assets/image2014-11-29-11-3a42-3a55.png)
