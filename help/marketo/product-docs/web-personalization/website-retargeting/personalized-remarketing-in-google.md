---
unique-page-id: 4720810
description: Google中的個人化再行銷 — Marketo檔案 — 產品檔案
title: Google中的個人化再行銷
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Google中的個人化再行銷 {#personalized-remarketing-in-google}

個人化再行銷可讓您利用RTP資料和Google Analytics的強大功能，並透過Google顯示網路觸及範圍，重新與使用者互動。

>[!PREREQUISITES]
>
>* 完成[使用網頁Personalization資料重新目標定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)設定
>* 檢閱[使用Google Analytics說明](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645)的再行銷檔案。

## 在Google中建立再行銷對象 {#creating-a-remarketing-audience-in-google}

1. 登入您的Google Analytics。 按一下&#x200B;**管理員**、**帳戶**、**屬性**。 按一下&#x200B;**對象定義**&#x200B;和&#x200B;**對象**。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 按一下&#x200B;**+新對象**。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **連結設定**：連結至您的Google Adwords帳戶。 **定義對象**：按一下&#x200B;**新建**。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. 在「對象產生器」中，按一下「自訂Dimension」、「自訂變數」、「事件」底下的&#x200B;**序列**&#x200B;和&#x200B;**尋找RTP資料**。

>[!TIP]
>
>如何在Analytics中尋找RTP資料來建立您的對象？
>
>在Google Analytics中：
>
>* 自訂變數：組織、產業
>* 事件類別：區段、Insightera-CTA、RTP — 再行銷
>* 事件標籤：區段名稱、行銷活動名稱、分段的對象名稱
>
>在Google Universal Analytics中：
>
>* 自訂Dimension：組織、產業、類別(Fortune 500,1000、Global 2000)、群組（企業、中小企業）、ABM清單（指定帳戶清單）
>* 事件類別：RTP-Segment、RTP-Campaign、RTP-Remarketing
>* 事件標籤：區段名稱、行銷活動名稱、分段的對象名稱

**來自RTP分段對象資料的再行銷對象範例**

1. 按一下&#x200B;**序列。**
1. 選取&#x200B;**事件標籤。**
1. 輸入&#x200B;**分段對象名稱** （如同RTP中所示）。
1. 按一下&#x200B;**套用**。

![](assets/image2015-2-10-14-3a51-3a43.png)

**來自RTP產業資料的對象範例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 按一下&#x200B;**序列**。
1. 選取&#x200B;**RTP — 產業**。
1. 輸入&#x200B;**產業名稱** (例如 金融服務、教育……)。
1. 按一下&#x200B;**套用**。
1. 輸入&#x200B;**對象名稱**。 按一下&#x200B;**保存**。

![](assets/image2015-1-15-18-3a29-3a16.png)

## 在Google Adwords中建立再行銷廣告行銷活動 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. 登入&#x200B;**Google Adwords**。 按一下&#x200B;**行銷活動**，選取&#x200B;**僅顯示網路**。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 輸入&#x200B;**促銷活動名稱**，選取&#x200B;**輸入再行銷。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 輸入&#x200B;**廣告群組名稱，**&#x200B;輸入&#x200B;**增強型CPC**，選取&#x200B;**再行銷清單**。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 按一下「儲存」並繼續。
1. 新增影像或文字廣告，然後開始您的再行銷活動。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [使用網頁Personalization資料重新進行目標定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* 在Facebook中[個人化的再行銷](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
