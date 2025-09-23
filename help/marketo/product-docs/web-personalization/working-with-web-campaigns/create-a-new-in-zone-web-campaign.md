---
unique-page-id: 4719400
description: 在區域中建立新的網頁行銷活動 — Marketo檔案 — 產品檔案
title: 建立新的特定區塊動態顯示網頁行銷活動
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 4%

---

# 建立新的特定區塊動態顯示網頁行銷活動 {#create-a-new-in-zone-web-campaign}

網路行銷活動是與特定區段關聯的自訂反應，可以是您網站上的[對話方塊](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)、區域取代、[Widget功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)或電子郵件警示。 「地區」網路促銷活動會根據地區ID將您網站的元素替換為內容或圖形橫幅。

## 建立區域內網路行銷活動 {#create-an-in-zone-web-campaign}

1. 移至&#x200B;**[!UICONTROL Web Campaigns]**。

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. 選取&#x200B;**[!UICONTROL Create New Web Campaign].**

   ![](assets/create-new-web-campaign-hand.png)

1. 選取&#x200B;**[!UICONTROL In Zone]**&#x200B;行銷活動型別。 自訂並新增&#x200B;**[!UICONTROL Zone id]。**&#x200B;將行銷活動設為&#x200B;**[!UICONTROL Sticky]**&#x200B;並在編輯器中新增您的創意。 新增要預覽的頁面URL，然後按一下&#x200B;**[!UICONTROL Preview]**&#x200B;以檢視行銷活動在您的網站上會如何回應。

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**什麼是區域ID？**
   >
   >區域ID是您希望&quot;[!UICONTROL In Zone]&quot;網路促銷活動位於網站上的位置。 若要尋找&quot;[!UICONTROL Zone ID]&quot;，只要移至您的網站，選取您要取代為網頁行銷活動的區域，然後按一下右鍵。 在Chrome中，選項為「檢查元素」，但在其他瀏覽器中，選項可能會有所不同。
   >
   >接著，您會想要尋找與網站此區段相關聯的「id」，此區段會反白顯示，因為您正在檢查該元素。 例如，如果您在Chrome中按一下滑鼠右鍵，醒目提示的文字會顯示`<div id="featured-slider">`，則「featured-slider」是您應在「zone id」區段中輸入的文字。 通常會使用「div id」，但也可以使用任何ID，例如h1 id、p id等。

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
   <td colspan="1" rowspan="1"><p>輸入在促銷活動取代之網站元素的HTML程式碼中找到的識別碼名稱。</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong> 粘性 </strong></p></td>
   <td colspan="1" rowspan="1">依預設，「粘著」核取方塊會針對「所在區域」行銷活動選取，且「所在區域」行銷活動會在訪客在網站上的整個作業階段中保持在其區域ID位置。 建議永遠將「In Zone」設為「Sticky」。</td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>正在淡出</strong> </p></td>
   <td colspan="1" rowspan="1">選取「使用效果」核取方塊和「淡化」 ，可讓網站上的「區域ID」區域呈現淡出效果。 如果「位於區域」是圖形橫幅，則頁面會先載入，然後促銷活動會啟動，呈淡出效果。</td>
  </tr>
  <tr>
   <td colspan="1"><strong>滑動</strong></td>
   <td colspan="1">選取「使用效果」核取方塊及「滑動」選項，可讓網站上的「區域ID」區域產生滑動效果。 如果「位於區域」是圖形橫幅，則頁面會先載入，然後促銷活動以由左至右的滑動效果啟動。</td>
  </tr>
  <tr>
   <td colspan="1"><strong> RTF 編輯器  </strong></td>
   <td colspan="1">RTF編輯器允許文字格式、連結和影像插入。 <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">在此閱讀更多資訊</a> 。</td>
  </tr>
  <tr>
   <td colspan="1"><strong> 在網站上預覽   </strong></td>
   <td colspan="1">在啟動行銷活動之前進行預覽。<br>
    <ul>
     <li> URL — 輸入行銷活動執行所在的範例URL，以檢視行銷活動即時效果的預覽範例。</li>
     <li>裝置 — 透過裝置預覽行銷活動的顯示方式：案頭、行動裝置直向、行動裝置橫向、Tablet直向、直向。</li>
     <li> 預覽 — 按一下<strong>預覽</strong>開啟範例URL的新視窗，以檢視行銷活動的反應。</li>
     <li> 共用 — 使用「共用」按鈕傳送電子郵件給同事，內含檢視Proxy促銷活動的連結。</li>
    </ul></td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>使用我們的[內建範本](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)或[將您現有的行銷活動](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)儲存為範本，以便重複使用，藉此加速並簡化行銷活動的建立程式。

>[!NOTE]
>
>**要進行A/B測試您的Web行銷活動？**&#x200B;一或多個網頁行銷活動可以[A/B測試以取得最佳結果](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md)。 透過自動調整功能，平台會自動辨識表現較好的行銷活動，並繼續最高轉換的行銷活動，並暫停其他行銷活動。

## 編輯網站行銷活動 {#edit-a-web-campaign}

從&#x200B;**網頁行銷活動**&#x200B;頁面，按一下行銷活動上的&#x200B;**編輯**。

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>若要更輕鬆地尋找您想要的行銷活動，請使用[篩選功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md)。

## 預覽網站行銷活動 {#preview-a-web-campaign}

1. 從[!UICONTROL Web Campaigns]頁面，按一下您要檢視之網頁行銷活動的&#x200B;**[!UICONTROL Preview]**。

   ![](assets/in-zone-web-campaign-preview.png)

## 原地複製網頁行銷活動 {#clone-a-web-campaign}

請參閱[複製網站行銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md)。

## 刪除網頁行銷活動 {#delete-a-web-campaign}

1. 從網頁行銷活動頁面，按一下您要刪除行銷活動上的&#x200B;**[!UICONTROL Delete]**。

   ![](assets/in-zone-web-campaign-delete.png)

1. 系統會顯示確認訊息，確認您是否要刪除行銷活動。

>[!MORELIKETHIS]
>
>* [建立新的Widget Web行銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [建立新的對話方塊網頁行銷活動](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
