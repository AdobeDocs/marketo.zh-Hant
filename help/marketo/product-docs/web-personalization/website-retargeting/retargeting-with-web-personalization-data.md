---
unique-page-id: 4720796
description: 使用Web個人化資料重新鎖定目標 — Marketo檔案 — 產品檔案
title: 使用Web個人化資料重新鎖定目標
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 使用Web個人化資料重新鎖定目標 {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>網站重新鎖定目標現在位於「網頁個人化」方塊下。 如果您只購買「重新鎖定目標」，您會看到此圖磚，並透過 **僅限** 已啟用重新定位功能。 這可讓您存取帳戶設定、「重新鎖定目標」頁面、區段及其他追蹤頁面。

再行銷會根據潛在客戶的身分和行為，以顯示廣告來鎖定過去造訪過您網站的潛在客戶。 個人化重新鎖定目標會根據產業、具名帳戶和已知人員資料，以相關廣告鎖定特定對象。

網頁個人化目前會將資料附加至下列再行銷平台：

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web個人化會將下列資料傳送至再行銷平台，以建立對象並執行再行銷廣告促銷活動：

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">網頁個人化資料</th> 
  </tr> 
  <tr> 
   <th><p>產業</p></th> 
  </tr> 
  <tr> 
   <th><p>組（企業、中小型企業）</p></th> 
  </tr> 
  <tr> 
   <th><p>類別(財富500/1000,2000年全球)</p></th> 
  </tr> 
  <tr> 
   <th><p>ABM清單（具名帳戶清單）</p></th> 
  </tr> 
  <tr> 
   <th><p>區段對象（根據區段）</p></th> 
  </tr> 
  <tr> 
   <th><p>已點按Web促銷活動</p></th> 
  </tr> 
 </tbody> 
</table>

## 再行銷設定 {#remarketing-configuration}

1. 前往 **重新定位**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >「重新定位設定」是依網域或子網域而定。 如果您想要將資料從這些網域傳送至重新定位平台，請啟動其他網域。

1. 啟用Google Analytics的設定，或依網域啟用Google Universal Analytics。

   >[!NOTE]
   >
   >您必須在網站上實作Google重新定位標籤。
   >
   >如果您已設定與Web個人化和Google Analytics的整合，則不需要編輯此部件，因為它與帳戶設定下的相同配置。

   ![](assets/two.png)

1. 啟動Facebook的設定。 按一下並展開Facebook折疊式功能表，按一下 **開啟** 將個別事件和資料傳送至FacebookAudience Manager。 按一下 **儲存**.

   >[!NOTE]
   >
   >你需要 [Facebook自訂對象像素](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)已安裝您的網站，以便使用此功能。

   ![](assets/three.png)

## 建立分段的受眾 {#creating-segmented-audience}

區段對象可讓您選取現有的區段作為對象，以用於重新定位促銷活動。 例如，選取已知人員區段。

>[!TIP]
>
>不需要針對產業或其他已在網域設定中傳送的資料建立分段對象。 最好根據已知人員資料，對區段使用分段對象。

1. 按一下 **建立分段的受眾**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. 輸入對象名稱、選取管道，然後從現有區段清單中選取區段。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 按一下 **儲存**.

   您現在已完成Web個人化中的重新鎖定目標設定、登入您的重新鎖定目標平台，以及根據此資料建立您的對象，並設定您的重新鎖定目標廣告促銷活動。
