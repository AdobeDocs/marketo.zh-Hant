---
unique-page-id: 4720810
description: Google中的個人化再行銷 — Marketo檔案 — 產品檔案
title: Google中的個人化再行銷
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Google中的個人化再行銷 {#personalized-remarketing-in-google}

個人化再行銷可讓您透過Google顯示網路，利用RTP資料和Google Analytics的強大功能，與使用者重新互動。

>[!PREREQUISITES]
>
>* 完成 [使用Web個人化資料重新鎖定目標](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) 配置
>* 檢閱 [使用Google Analytics說明進行再行銷](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) 檔案。


## 在Google中建立再行銷對象 {#creating-a-remarketing-audience-in-google}

1. 登入您的Google Analytics。 按一下 **管理**, **帳戶**, **屬性**. 按一下 **對象定義** 和 **對象**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. 按一下 **+新受眾**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **連結設定**:連結至您的Google Adwords帳戶。 **定義對象**:按一下 **新建**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. 在Audience Builder中，按一下 **序列** 和 **查找RTP資料** 在「自訂Dimension」、「自訂變數」、「事件」下。

>[!TIP]
>
>如何在Analytics中尋找RTP資料以建立您的對象？
>
>在Google Analytics中：
>
>* 自訂變數：組織、行業
>* 事件類別：區段， Insightera-CTA, RTP — 再行銷
>* 事件標籤：區段名稱、促銷活動名稱、分段對象名稱
>
>在Google Universal Analytics中：
>
>* 自訂Dimension:組織、行業、類別（財富500,1000，全球2000年）、組（企業、中小型企業）、ABM清單（指定客戶清單）
>* 事件類別：RTP — 區段、RTP — 促銷活動RTP — 再行銷
>* 事件標籤：區段名稱、促銷活動名稱、分段對象名稱


**從RTP分段的受眾資料再行銷受眾的範例**

1. 按一下 **序列。**
1. 選擇 **事件標籤。**
1. 輸入 **分段對象的名稱** （如RTP中所示）。
1. 按一下 **套用**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**來自RTP產業資料的受眾範例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 按一下 **序列**.
1. 選擇 **RTP-Industry**.
1. 輸入 **產業名稱** (例如 金融服務、教育……)。
1. 按一下 **套用**.
1. 輸入 **對象名稱**. 按一下 **儲存**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## 在Google Adwords中建立再行銷廣告促銷活動 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. 登入 **Google Adwords**. 按一下 **行銷活動**，選取 **僅顯示網路**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 輸入 **促銷活動名稱**，選擇 **輸入再行銷。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 輸入 **廣告群組名稱、** 輸入 **增強的CPC**，選擇 **再行銷清單**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 按一下「儲存並繼續」。
1. 新增影像或文字廣告，然後開始再行銷活動。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [使用Web個人化資料重新鎖定目標](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [facebook中的個人化再行銷](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

