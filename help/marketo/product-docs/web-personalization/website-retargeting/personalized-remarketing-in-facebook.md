---
unique-page-id: 4720917
description: Facebook的個人化再行銷——行銷檔案——產品檔案
title: Facebook中的個人化再行銷
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Facebook中的個人化再行銷{#personalized-remarketing-in-facebook}

個人化再行銷可讓您使用RTP資料和Facebook再行銷的強大功能，與使用者重新互動。

>[!PREREQUISITES]
>
>* 完成[使用Web個人化資料重新定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)設定
>* 檢視「自訂對象」和「再行銷」的[](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)[Facebook檔案。](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)


## 在Facebook中建立對象{#creating-an-audience-in-facebook}

1. 在Facebook中，前往「廣告管理員」中的「對象」標籤[。](https://www.facebook.com/ads/audience_manager)

1. 按一下「工具」**並選取「對象」**。****

   ![](assets/one-1.png)

1. 按一下「建立自訂對象」。****

   ![](assets/two-1.png)

1. 選擇&#x200B;**網站流量**。

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. 在「網站流量」清單中，選取「自訂組合」**。**

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. 在「包括」清單中，選擇&#x200B;**Event**。

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. 在「事件」清單中，選擇&#x200B;**RTP Remarketing**&#x200B;並選擇參數。

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. 在此範例中，選取「產業」以包含&#x200B;**Education**。 輸入&#x200B;**教育**，並編輯&#x200B;**在最近**&#x200B;中為180天。 輸入對象名稱：**教育產業**。 按一下「建立對象」。****

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. 您現在已在Facebook中使用RTP資料建立新的自訂對象。

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## Facebook中的RTP資料點{#rtp-data-points-in-facebook}

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
        <td>（帳戶型清單的名稱）</td> 
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
        <td><p>防衛</p><p>教育</p><p>金融服務</p><p>政府機關</p><p>醫療保健、製藥、生物技術</p><p>軟體與網際網路</p><p>等等……（根據RTP行業選項）</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">細分受眾</td> 
        <td colspan="1">（在RTP中建立的分段對象名稱）</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 使用廣告{#target-your-audience-with-an-ad}鎖定您的對象

如需詳細資訊，請參閱[Facebook的檔案](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience)。

1. 前往「廣告管理員」，按一下「建立廣告」。****

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. 選擇&#x200B;**將訪客傳送至您的網站**&#x200B;作為促銷活動的目標。

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. 輸入您的網站URL。

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. 建立您的廣告集。 從您建立的「對象」清單中選取自訂對象，例如教育產業。

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. 選擇所有其他廣告集選項、設定預算並定義廣告創意。

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. 您現在都已在Facebook中設定個人化的再行銷活動。

>[!MORELIKETHIS]
>
>* [使用網頁個人化資料重新鎖定目標](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Google的個性化再營銷](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

