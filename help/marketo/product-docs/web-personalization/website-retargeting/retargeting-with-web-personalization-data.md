---
unique-page-id: 4720796
description: 使用網頁個人化資料重新進行目標定位 — Marketo檔案 — 產品檔案
title: 使用網頁個人化資料重新進行目標定位
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 使用網頁個人化資料重新進行目標定位 {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>網站重新目標定位現在歸類於「網頁個人化」圖磚之下。 如果您只購買重新目標定位，您會看到此動態磚，並透過存取Web Personalization產品 **僅限** 已啟用重新定位功能。 這可讓您存取帳戶設定、「重新目標定位」頁面、區段以及其他追蹤頁面。

再行銷會根據潛在客戶的身份和行為，將目標鎖定於過去造訪過您網站的潛在客戶，並投放顯示廣告。 個人化重新鎖定目標會根據產業、具名帳戶和已知個人資料，利用相關廣告鎖定特定對象。

Web Personalization目前會將資料附加至下列再行銷平台：

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web Personalization會將下列資料傳送至再行銷平台，以建立對象並執行再行銷廣告行銷活動：

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">網頁個人化資料</th> 
  </tr> 
  <tr> 
   <th><p>產業</p></th> 
  </tr> 
  <tr> 
   <th><p>群組（企業、中小企業）</p></th> 
  </tr> 
  <tr> 
   <th><p>類別(Fortune 500/1000、Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>ABM清單（具名帳戶清單）</p></th> 
  </tr> 
  <tr> 
   <th><p>區段對象（根據區段）</p></th> 
  </tr> 
  <tr> 
   <th><p>網頁促銷活動已點按</p></th> 
  </tr> 
 </tbody> 
</table>

## 再行銷設定 {#remarketing-configuration}

1. 前往 **重新目標定位**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >「重新定位設定」是依網域或子網域而定。 如果您想要將資料從其他網域傳送至重新定位平台，請啟用這些網域。

1. 為每個網域啟用Google Analytics或Google Universal Analytics的設定。

   >[!NOTE]
   >
   >您必須在網站上實施Google重新目標定位標籤。
   >
   >如果您已設定與「網頁個人化」和Google Analytics的整合，則不需要編輯此零件，因為它與「帳戶設定」下的設定相同。

   ![](assets/two.png)

1. 啟動Facebook的設定。 按一下並展開Facebook摺疊式功能表，按一下 **開啟** 將個別事件和資料傳送至FacebookAudience Manager。 按一下 **儲存**.

   >[!NOTE]
   >
   >您必須擁有 [facebook自訂對象畫素](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)已安裝您的網站，此功能可正常運作。

   ![](assets/three.png)

## 建立區段對象 {#creating-segmented-audience}

區段對象可讓您選取現有區段作為對象，以用於重新定位行銷活動。 例如，選取您的「已知人員」區段。

>[!TIP]
>
>不需要為產業或其他已在網域設定中透過傳送的資料建立分段對象。 建議您最好根據已知人員資料對區段使用分段對象。

1. 按一下 **建立區段對象**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. 輸入對象名稱，選取管道，然後從現有區段清單中選取區段。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 按一下 **儲存**.

   您現在已完成Web Personalization中的重新目標定位設定、登入您的重新目標定位平台，並根據此資料建立您的對象，以及設定您的重新目標定位廣告行銷活動。
