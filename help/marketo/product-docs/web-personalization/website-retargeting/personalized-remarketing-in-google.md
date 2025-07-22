---
unique-page-id: 4720810
description: Google中的個人化再行銷 — Marketo檔案 — 產品檔案
title: Google中的個人化再行銷
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# Google中的個人化再行銷 {#personalized-remarketing-in-google}

個人化再行銷可讓您利用RTP資料和Google Analytics的強大功能，並透過Google顯示網路觸及範圍，重新與使用者互動。

>[!PREREQUISITES]
>
>* 使用[資料 [!DNL Web Personalization] 設定完成](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)重新目標定位
>* 檢閱Google Analytics說明的[再行銷](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645)檔案。

## 在Google中建立再行銷對象 {#creating-a-remarketing-audience-in-google}

1. 登入您的Google Analytics。 按一下&#x200B;**[!UICONTROL Admin]**，**[!UICONTROL Account]**，**[!UICONTROL Property]**。 按一下&#x200B;**[!UICONTROL Audience Definitions]**&#x200B;和&#x200B;**[!UICONTROL Audiences]**。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 按一下「**[!UICONTROL +New Audience]**」。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL Link Configuration]**：連結至您的[!DNL Google Adwords]帳戶。 **[!UICONTROL Define Audience]**：按一下&#x200B;**[!UICONTROL Create New]**。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. 在對象產生器中，按一下&#x200B;**[!UICONTROL Sequences]**、**[!UICONTROL Find the RTP Data]**、[!UICONTROL Custom Dimensions]下的[!UICONTROL UICONTROL [ !] Custom Variables]和[!UICONTROL Events]。

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
>* 自訂維度：組織、產業、類別(Fortune 500,1000、Global 2000)、群組（企業、中小企業）、ABM清單（具名帳戶清單）
>* 事件類別：RTP-Segment、RTP-Campaign、RTP-Remarketing
>* 事件標籤：區段名稱、行銷活動名稱、分段的對象名稱

**來自RTP分段對象資料的再行銷對象範例**

1. 按一下&#x200B;**[!UICONTROL Sequences].**
1. 選取&#x200B;**[!UICONTROL Event Label].**
1. 輸入&#x200B;**[!UICONTROL Name of Segmented Audience]** （如它在RTP中所示）。
1. 按一下「**[!UICONTROL Apply]**」。

![](assets/image2015-2-10-14-3a51-3a43.png)

**來自RTP產業資料的對象範例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 按一下「**[!UICONTROL Sequences]**」。
1. 選擇「**[!UICONTROL RTP-Industry]**」。
1. 輸入&#x200B;**產業名稱** （例如[!UICONTROL Financial Services]，[!UICONTROL Education]...）。
1. 按一下「**[!UICONTROL Apply]**」。
1. 輸入&#x200B;**[!UICONTROL Audience Name]**。 按一下「**[!UICONTROL Save]**」。

![](assets/image2015-1-15-18-3a29-3a16.png)

## 在[!DNL Google Adwords]中建立再行銷廣告行銷活動 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. 登入&#x200B;**[!DNL Google Adwords]**。 按一下&#x200B;**[!UICONTROL Campaigns]**，選取&#x200B;**[!UICONTROL Display Network only]**。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 輸入&#x200B;**[!UICONTROL Campaign Name]**，選取&#x200B;**[!UICONTROL Type Remarketing].**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 輸入&#x200B;**[!UICONTROL Ad Group Name]，**&#x200B;輸入&#x200B;**[!UICONTROL Enhanced CPC]**，選取&#x200B;**[!UICONTROL Remarketing List]**。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 按一下&#x200B;**[!UICONTROL Save]**&#x200B;並繼續。
1. 新增影像或文字廣告，然後開始您的再行銷活動。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [使用 [!DNL Web Personalization] 資料重新鎖定目標](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [個人化再行銷於 [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
