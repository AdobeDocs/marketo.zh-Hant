---
unique-page-id: 4719400
description: 在區域網路促銷活動中建立新功能——行銷檔案——產品檔案
title: 在區域網頁促銷活動中建立新功能
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---


# 在區域Web促銷活動中建立新促銷活動{#create-a-new-in-zone-web-campaign}

網頁促銷活動是與特定區段相關的自訂反應，可以是您網站上的[對話方塊](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)、區域內取代、[介面工具集功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)或電子郵件警報。 「在區域內」網頁促銷活動會以內容或圖形橫幅取代您網站中根據區域ID的元素。

## 建立區域內Web促銷活動{#create-an-in-zone-web-campaign}

1. 前往&#x200B;**Web促銷活動**。

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. 選擇&#x200B;**建立新Web促銷活動。**

   ![](assets/create-new-web-campaign-hand.png)

1. 選擇&#x200B;**在區域中**&#x200B;促銷活動類型。 自訂並新增&#x200B;**Zone id。** 將促銷活動設 **** 為Sticky，並在編輯器中新增您的創意。新增要預覽的頁面URL，然後按一下&#x200B;**預覽**，查看促銷活動在您網站上的反應。

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**什麼是區域ID?**
   >
   >區域ID是您要在Onsite上找到「在區域內」網頁促銷活動的位置。 若要尋找「區域ID」，只要前往您的網站，選取您要以Web促銷活動取代的區域，然後按一下滑鼠右鍵即可。 在Chrome中，選項是「Inspect元素」，在其他瀏覽器中可能不同。
   >
   >然後，您會想要尋找與網站此區段關聯的「id」，因為您正在檢查該元素，所以會反白顯示此區段。 例如，如果在Chrome中按一下滑鼠右鍵，反白顯示的文字會顯示`<div id="featured-slider">`，則「featured-slider」是您應在「zone id」區段中輸入的內容。 通常使用&quot;div id&quot;，但也可使用任何ID，例如h1 id、p id等。

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">名稱</th> 
   <th colspan="1" rowspan="1">說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> 區域ID </strong></td> 
   <td colspan="1" rowspan="1"><p>輸入促銷活動所取代之網站元素之HTML程式碼中找到的ID名稱。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 黏著 </strong></p></td> 
   <td colspan="1" rowspan="1">依預設，「在區域內」促銷活動會選取「自黏」核取方塊，並在網站訪客作業期間將「在區域內」促銷活動保留在其「區域內」ID位置。 建議一律將「In Zone」（入區）設為「Sticky」（自黏）。</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 淡出</strong> </p></td> 
   <td colspan="1" rowspan="1">選取「使用效果」核取方塊和「淡出」會對網站上的「區域ID」區域產生淡出效果。 如果「在區域」是圖形橫幅，則頁面會先載入，然後促銷活動會以淡出效果啟動。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>滑動</strong></td> 
   <td colspan="1">選取「使用效果」核取方塊和「滑動」選項可讓滑動效果對網站的「區域識別碼」區域有效。 如果「在區域」是圖形橫幅，則頁面會先載入，然後以從左至右的滑動效果啟動促銷活動。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Rich Text Editor  </strong></td> 
   <td colspan="1">富格文本編輯器允許文本格式設定、連結和影像插入。 <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">閱讀更多資訊</a> 。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 在網站上預覽   </strong></td> 
   <td colspan="1">在促銷活動啟動之前先預覽。<br> 
    <ul> 
     <li> URL —— 輸入執行促銷活動的範例URL，以檢視促銷活動的顯示效果預覽範例。</li> 
     <li>裝置——預覽促銷活動依裝置的顯示方式：桌上型電腦、行動縱向、行動橫向、平板電腦縱向、縱向橫向。</li> 
     <li> 預覽——按一下「預覽」以開啟範例URL的新視窗，以瞭解促銷活動的反應。<strong></strong></li> 
     <li> 共用——使用「共用」按鈕，將電子郵件傳送給具有連結的同事，以查看代理促銷活動。</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>使用我們內建的[範本](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)或[儲存現有促銷活動](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)做為範本，以加速並簡化促銷活動建立程式。

>[!NOTE]
>
>**想要A/B測試您的Web促銷活動嗎？** 您可以測試一或多個網頁促銷 [活動，以取得最佳結果](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md)。透過「自動調整」功能，平台會自動辨識效能較佳的促銷活動、繼續轉換率最高的促銷活動並暫停其他促銷活動。

## 編輯Web促銷活動{#edit-a-web-campaign}

從「Web促銷活動」頁面，按一下「促銷活動」上的「編輯」。********

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>若要更輕鬆找到您想要的促銷活動，請使用[篩選功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md)。

## 預覽Web促銷活動{#preview-a-web-campaign}

1. 在「Web促銷活動」頁面中，按一下您要檢視之Web促銷活動上的&#x200B;**預覽**。

   ![](assets/in-zone-web-campaign-preview.png)

## 複製Web促銷活動{#clone-a-web-campaign}

請參閱[複製Web促銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md)。

## 刪除Web促銷活動{#delete-a-web-campaign}

1. 在「Web促銷活動」頁面中，按一下您要刪除之促銷活動上的&#x200B;**Delete**。

   ![](assets/in-zone-web-campaign-delete.png)

1. 會出現確認訊息，確認您是否要刪除促銷活動。

>[!MORELIKETHIS]
>
>* [建立新的Widget Web促銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [建立新對話方塊Web促銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)

