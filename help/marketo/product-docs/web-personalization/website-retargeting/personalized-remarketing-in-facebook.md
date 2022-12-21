---
unique-page-id: 4720917
description: facebook中的個人化再行銷 — Marketo檔案 — 產品檔案
title: facebook中的個人化再行銷
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# facebook中的個人化再行銷 {#personalized-remarketing-in-facebook}

個人化再行銷可讓您使用RTP資料和Facebook再行銷的強大功能，與使用者重新互動。

>[!PREREQUISITES]
>
>* 完成 [使用Web個人化資料重新鎖定目標](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) 設定
>* 檢閱 [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [自訂對象的facebook檔案](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) 和再行銷。


## 在Facebook中建立對象 {#creating-an-audience-in-facebook}

1. 在Facebook，前往 [對象標籤](https://www.facebook.com/ads/audience_manager) 廣告管理員。

1. 按一下 **工具** 選取 **對象**.

   ![](assets/one-1.png)

1. 按一下 **建立自訂對象**.

   ![](assets/two-1.png)

1. 選擇 **網站流量**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. 在「網站流量」清單中，選取 **自訂組合**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. 在「包含」清單中，選取 **事件**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. 在「事件」清單中，選取 **RTP再行銷** 並選取參數。

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. 在此範例中，選取要包含的產業 **教育**. 輸入 **教育**，編輯 **最後** 180天。 輸入對象名稱： **教育產業**. 按一下 **建立對象**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. 您現在已使用Facebook中的RTP資料建立新的自訂對象。

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## facebook中的RTP資料點 {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>事件名稱</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>RTP再行銷</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>參數</th> 
        <th>值</th> 
       </tr> 
       <tr> 
        <td>ABM清單</td> 
        <td>（帳戶型清單名稱）</td> 
       </tr> 
       <tr> 
        <td colspan="1">類別</td> 
        <td colspan="1"><p>財富500強</p><p>財富1000強</p><p>2000年全球</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">群組</td> 
        <td colspan="1"><p>企業</p><p>中小型企業</p></td> 
       </tr> 
       <tr> 
        <td>產業</td> 
        <td><p>防禦</p><p>教育</p><p>金融服務</p><p>政府</p><p>醫療保健、製藥、生物技術</p><p>軟體和網際網路</p><p>等（根據RTP行業選項）</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">區段的受眾</td> 
        <td colspan="1">（在RTP中建立的分段對象名稱）</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 使用廣告定位您的對象 {#target-your-audience-with-an-ad}

如需其他詳細資訊，請參閱 [Facebook檔案](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. 前往「廣告管理員」，按一下 **建立廣告**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. 選擇 **將人員發送到您的網站** 作為促銷活動的目標。

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. 輸入您的網站URL。

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. 建立您的廣告集。 從您建立的對象清單中選取自訂對象，例如教育產業。

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. 選取所有其他廣告集選項、設定預算並定義廣告創意素材。

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. 您現在都可以在Facebook中設定個人化再行銷活動。

>[!MORELIKETHIS]
>
>* [使用Web個人化資料重新鎖定目標](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Google中的個人化再行銷](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

