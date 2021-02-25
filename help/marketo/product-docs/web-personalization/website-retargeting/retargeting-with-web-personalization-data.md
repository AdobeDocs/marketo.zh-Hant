---
unique-page-id: 4720796
description: 使用網頁個人化資料重新鎖定目標——行銷檔案——產品檔案
title: 使用網頁個人化資料重新鎖定目標
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---


# 使用Web個人化資料重新定位{#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>「網站重新定位」現在位於「網頁個人化」方塊下。 如果您只購買「重新定位」功能，您會看到此圖格，並存取僅&#x200B;****&#x200B;啟用「重新定位」功能的「網頁個人化」產品。 這可讓您存取帳戶設定、重新定位頁面、區段和其他追蹤頁面。

再行銷的目標客戶是過去曾瀏覽過您網站的潛在客戶，他們會根據他們的身分和所做的事，以展示廣告為目標。 個人化的重新定位會根據產業、指名帳戶和已知人員資料，以相關廣告鎖定特定受眾。

Web個人化目前會將資料附加至下列再行銷平台：

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web個人化會傳送下列資料至再行銷平台，以建立受眾並執行再行銷廣告促銷活動：

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">網頁個人化資料</th> 
  </tr> 
  <tr> 
   <th><p>產業</p></th> 
  </tr> 
  <tr> 
   <th><p>群組（企業、中小型企業）</p></th> 
  </tr> 
  <tr> 
   <th><p>類別（財富500/1000，全球2000年）</p></th> 
  </tr> 
  <tr> 
   <th><p>ABM清單（命名帳戶清單）</p></th> 
  </tr> 
  <tr> 
   <th><p>細分受眾（根據細分）</p></th> 
  </tr> 
  <tr> 
   <th><p>點按的Web促銷活動</p></th> 
  </tr> 
 </tbody> 
</table>

## 重新行銷設定{#remarketing-configuration}

1. 前往&#x200B;**重新定位**。

   ![](assets/one.png)

   >[!NOTE]
   >
   >「重新定位設定」是依網域或子網域而定。 如果您想要將資料從這些網域傳送至重新定位平台，請啟動其他網域。

1. 針對每個網域啟用Google Analytics或Google Universal Analytics的設定。

   >[!NOTE]
   >
   >您必須在您的網站上實作「Google重新定位標籤」。
   >
   >如果您已設定「與Web個人化」和「Google Analytics整合」，則不需要編輯此部分，因為它與「帳戶設定」下的設定相同。

   ![](assets/two.png)

1. 啟動Facebook的設定。 按一下並展開Facebookaccordion，按一下&#x200B;**On**，將個別的事件和資料傳送至Facebook Audience Manager。 按一下&#x200B;**保存**。

   >[!NOTE]
   >
   >您必須安裝[Facebook自訂對象像素](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)，才能使用此功能。

   ![](assets/three.png)

## 建立區段對象{#creating-segmented-audience}

「區隔對象」可讓您選取現有的「區隔」作為對象，以用於重新定位促銷活動。 例如，選取「已知人員」區段。

>[!TIP]
>
>您不需要針對已在網域設定中傳送的產業或其他資料建立分段對象。 最好根據已知人員資料，針對區段使用區段對象。

1. 按一下「建立區段對象&#x200B;**」。**

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. 輸入對象名稱，選取渠道，並從現有區段清單中選取區段。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 按一下&#x200B;**保存**。

   您現在已完成「網頁個人化」中的「重新定位設定」、登入您的重新定位平台，並根據此資料建立您的受眾，以及設定您的重新定位廣告促銷活動。
