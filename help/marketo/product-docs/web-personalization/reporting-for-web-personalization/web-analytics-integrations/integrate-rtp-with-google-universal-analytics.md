---
unique-page-id: 4720125
description: 將RTP與Google Universal Analytics整合——行銷檔案——產品檔案
title: 將RTP與Google Universal Analytics整合
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# 將RTP與Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}整合

## 介紹{#intro}

運用Google Universal Analytics(GUA)與Marketo Real-Time Personalization的(RTP)原始圖形和個人化資料，以更好地測量和分析您的線上行銷成果。

本貼文說明如何設定Marketo即時個人化(RTP)平台與Google Universal Analytics(GUA)帳戶整合。 RTP資料可附加至您的GUA帳戶，讓您檢視並檢視造訪您網站的組織、產業、圖片和RTP區段的效能。

**Google Universal Analytics**

Google Universal Analytics搭配RTP的資料，讓您更瞭解B2B使用者如何與您的線上內容互動，並協助測量並從您的個人化宣傳中獲得更佳的結果。 [閱讀更多有關Google Universal Analytics的資訊](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1)。

>[!NOTE]
>
>**僅限Google標籤管理員使用者**
>
>不需要進行編碼或特殊配置。 請確定您已完成下列檢查清單：
>
>* RTP維度是在Google Universal Analytics中建立
>* [RTP標籤已正確安裝在Google標籤管理器中](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* RTP的「帳戶設定」中啟用了Google Universal Analytics整合
>* [Google Universal Analytics標籤已在Google標籤管理器中正確設定](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [您的網站已正確安裝Google Tag Manager標籤](https://developers.google.com/tag-manager/quickstart)


## 在GUA {#set-up-custom-dimensions-in-gua}中設定自訂維度

1. 在Google Analytics中，

   1. 前往&#x200B;**Admin**
   1. 選擇&#x200B;**帳戶。**
   1. 選擇&#x200B;**屬性。**
   1. 選擇&#x200B;**自訂定義**&#x200B;和&#x200B;**自訂維度**。
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 新增自訂維度。 按一下「**+新建自訂維度**」

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 新增下列&#x200B;**自訂維度：**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>自訂維度名稱</strong></p></td> 
   <td><p><strong>範圍</strong></p></td> 
   <td><p><strong>作用中</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP組織</strong></p></td> 
   <td><p>會話</p></td> 
   <td><p align="center">ý</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Industry</strong></p></td> 
   <td><p>會話</p></td> 
   <td><p align="center">ý</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP類別</strong></p></td> 
   <td><p>會話</p></td> 
   <td><p align="center">ý</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP組</strong></p></td> 
   <td><p>會話</p></td> 
   <td><p align="center">ý</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**自訂維** 度名稱必須與上表中的定義完全相同（否則，GUA中的自訂RTP控制面板和報表無法正確顯示）

1. 添加&#x200B;**名稱**。 選擇範圍作為&#x200B;**會話**。 按一下&#x200B;**建立**。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

您的自訂維度清單應如下所示。

![](assets/image2014-11-29-11-36-50-version-2.png)

在激活GUA中的自定義維後，請轉至RTP平台以在RTP中啟用這些維。

## 在RTP帳戶{#activate-the-gua-integration-in-your-rtp-account}中激活GUA整合

1. 在RTP平台中，轉到&#x200B;**帳戶設定。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在「**帳戶設定**」下，按一下「**網域**」。
1. 在「**Analytics**」下方，按一下「Google Universal Analytics **」。**
1. 開啟&#x200B;****&#x200B;相關的自訂維度和事件，將此資料從RTP附加至Google Universal Analytics。
1. 在GUA中輸入與索引編號對齊的維的&#x200B;**索引編號**。
1. 按一下&#x200B;**保存**。

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>在GUA的「自訂維度」下，可找到自訂維度的索引編號。
>
>範例：RTP-Industry Index Number=1,RTP-Organization Index Number=2。

## 移除Google Analytics中的舊控制面板{#remove-old-dashboards-in-google-analytics}

1. 在Google Analytics中。 轉至&#x200B;**報告。**
1. 按一下&#x200B;**儀表板。**
1. 選擇&#x200B;**儀表板**（RTP B2B或RTP效能）
1. 按一下「刪除控制面板」。****

![](assets/image2014-11-29-11-3a42-3a55.png)
