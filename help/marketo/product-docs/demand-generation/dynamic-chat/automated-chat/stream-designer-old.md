---
description: 串流設計工具 — Marketo檔案 — 產品檔案
title: 流程設計工具
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 3788898496c50ebc3a5a8bf6adbd79a270024be7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%

---

# 流程設計工具 {#stream-designer}

有 _許多_ 可能的資料流組合。 本文包含行銷人員詢問網站訪客是否有任何產品問題的範例。 如果是，訪客可以排程約會。 如果沒有，訪客可以選擇加入郵寄清單以備將來通訊。 此外還提供免費PDF。 最終目標是排程約會或收集訪客的電子郵件。

>[!PREREQUISITES]
>
>您必須先使用檔案卡，才能使用 [設定它](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"} 在您的Adobe帳戶中。

## 串流設計工具卡片 {#stream-designer-cards}

串流設計工具包含多個卡片，您可以新增卡片來塑造聊天對話。

<table>
 <tr>
  <td style="width:25%"><strong>訊息</strong></td>
  <td>當您想發表不需回應的陳述式時使用(例如：「嗨！ 所有商品今天皆有25%優惠（優惠碼SAVE25"）。
</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>問題</strong></td>
  <td>當您想要詢問多重選擇問題時，請使用該選項，您可以提供其中可用的回應（例如：您感興趣的車輛型別為何？） 回應= SUV、Compact、Truck等)。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>文件</strong></td>
  <td>可讓您將PDF檔案內嵌在對話方塊中，並追蹤訪客的檔案參與活動（已檢視多少頁面、是否已下載檔案，及/或任何使用的搜尋詞）。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>資訊擷取</strong></td>
  <td>當您想要收集資訊（例如姓名、電子郵件地址、職稱等）時使用。 選擇要將訪客的回應歸因到哪個欄位後，您可以選擇讓訪客輸入回應，或從您決定的挑選清單中選取選項（秘訣：後者可協助改善資料庫清潔度）。 您也可以選擇以他們的回應覆寫您目前為其列出的任何資料，或者，如果您已經擁有問題的值，則完全略過問題。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>會議預訂</strong></td>
  <td>為訪客提供可用日期的行事曆以排程會議。 透過循環配置資源、特定代理程式或使用自訂規則，選擇行事曆可用性。 按一下 <b>新增屬性</b> 如果您想要擷取代理程式的名稱或電子郵件地址，並將其指派給聊天訪客的個人記錄以供日後查詢(提示：建立 <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">自訂欄位</a> 將代理程式的資訊對應至，以免覆寫標準Marketo Engage欄位)。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>目標</strong></td>
  <td>這是訪客唯一不會看到的卡片。 您可以決定在特定聊天中達成目標的時間（例如：如果收集訪客的電子郵件是您的目標，請在資料流中的資訊擷取之後立即放置目標卡片）。</td>
 </tr>
 <tr>
  <td style="width:25%"><strong>動作*</strong></td>
  <td>類似於表單中的隱藏欄位，您可以使用動作卡填入任何潛在客戶或公司屬性(具有 <a href="/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md#string">字串資料型別</a>)擷取隱含值。 您可以在交談的任何時間點新增動作卡，並使用自動填入個別值的值或原生權杖更新個別屬性。
  <p><i>*動作卡需要Dynamic Chat Prime。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。</i></td>
 </tr>
 <tr>
  <td style="width:25%"><strong>即時聊天</strong></td>
  <td>當您希望訪客與即時代理程式聊天時，請使用即時聊天卡。
  <li>即時聊天卡必須是分支中的最後一張卡。</li>
  <li>訪客在資料流中到達這張卡片後，就會立即路由到代理商，因此建議在此卡片前面加上問答卡，詢問訪客是否想與即時代理商聊天。</li></td>
 </tr>
</table>

## 串流設計工具圖示 {#stream-designer-icons}

在串流設計工具的右上角，您會看到幾個圖示。 以下是他們的工作。

<table>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-1.png"></td>
  <td>放大，建立更大的卡片</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-2.png"></td>
  <td>縮小，建立較小的卡片</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-3.png"></td>
  <td>開啟一個視窗，供您測試您的聊天（按相同按鈕關閉）</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-4.png"></td>
  <td>可讓您搜尋資料流中的卡片型別或內容</td>
 </tr>
 <tr>
  <td style="width:10%"><img src="assets/stream-designer-5.png"></td>
  <td>排列串流中的所有卡片</td>
 </tr>
</table>

## 建立資料流 {#create-a-stream}

您可以建立對話方塊的串流或 [對話式Forms](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"}. 在此範例中，我們將為對話方塊建立一個對話方塊。

1. 在您完成以下任務後： [已建立您的對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}，按一下 **[!UICONTROL 串流設計工具]** 標籤。

   ![](assets/stream-designer-6.png)

1. 拖放 [!UICONTROL 問題] 卡片。

   ![](assets/stream-designer-7.png)

1. 在 [!UICONTROL 聊天機器人回應]，說出您想要問的問題。

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >您可以使用代號為已知的聊天訪客個人化體驗(例如：Hello `{{lead.leadFirstName:""}}`)。 只要按一下右側的花括弧圖示，即可進行選取。 如果您希望匿名訪客看到一般專案（例如：Hello），請在引號之間新增預設值 `{{lead.leadFirstName:"there"}}`)。

   >[!NOTE]
   >
   >Poke預設為開啟，這會在聊天圖示旁邊顯示開頭的問題，訪客不需要按一下它即可檢視。 Poke只適用於交談中的第一張卡片。

1. 輸入您的使用者回應，然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**[!UICONTROL 編輯儲存的值]** 如果想在資料庫中儲存的值與聊天機器人針對問題卡片中的對應屬性向訪客顯示的值不同（例如：訪客看到「搜尋引擎最佳化」，而您將該值儲存為「SEO」），此為選用步驟。

1. 若為「是」，我們想要排程約會，因此在該選項下方將拖曳到「約會排程器」卡上。

   ![](assets/stream-designer-10.png)

1. 在右側的欄中，按一下 **[!UICONTROL 儲存]**.

   ![](assets/stream-designer-11.png)

1. 由於這是目標，請拖曳 [!UICONTROL 目標] 卡片在約會排程器下方。

   ![](assets/stream-designer-12.png)

1. 為您的目標命名（或選擇現有目標），然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/stream-designer-13.png)

1. 若為「否」，我們想要檢視他們是否會加入郵寄清單，所以在該選項下方將拖曳至其他選項 [!UICONTROL 問題] 卡片。

   ![](assets/stream-designer-14.png)

1. 輸入您的回應，並為訪客新增回應選擇。 按一下 **[!UICONTROL 儲存]** 完成時。

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >您可以按一下「 」，新增更多回應 **[!UICONTROL 新增回應]**.

1. 在「是」回應下方，拖曳至「資訊擷取」卡片上方，以便收集訪客的電子郵件。

   ![](assets/stream-designer-16.png)

1. 按一下 **[!UICONTROL 型別]** 下拉式清單並選取 **[!UICONTROL 電子郵件]**.

   ![](assets/stream-designer-17.png)

1. 輸入聊天機器人訊息和預留位置。 確定屬性已對應到Marketo Engage中的適當欄位，然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td style="width:30%"><strong>類型</strong></td>
     <td>您要擷取的資訊型別：電話、文字、電子郵件。</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>聊天機器人訊息</strong></td>
     <td>訪客看到的訊息，提示他們提供資訊。</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>預留位置</strong></td>
     <td>範例文字可協助訪客檢視要輸入的內容。</td>
    </tr>
    <tr>
     <td style="width:30%"><strong>將回應對應到屬性</strong></td>
     <td>可讓您將訪客的回應同步至您Marketo Engage訂閱中其「人員」記錄中的對應欄位。</td>
    </tr>
   </table>

1. 由於收集其電子郵件是目標，因此請拖曳 [!UICONTROL 目標] 資訊擷取下方的卡片。

   ![](assets/stream-designer-19.png)

1. 為您的目標命名（或選擇現有目標），然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/stream-designer-20.png)

1. 如果對方說「否」，請記得新增回應。 一個選項是拖曳下方的訊息卡，並說「仍要感謝您」。 但在此範例中，我們會改為提供他們自由PDF檔案。

   ![](assets/stream-designer-21.png)

1. 在此範例中，我們將建立新檔案。 為其命名，輸入您已託管之PDF的URL，然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/stream-designer-22.png)

1. 選取 **[!UICONTROL 預覽]** 切換即可預覽您的對話方塊。

   ![](assets/stream-designer-23.png)

1. 當您準備好要啟動對話方塊時，請按一下 **[!UICONTROL 發佈]**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>按一下之前 [!UICONTROL 發佈]，請記得確定您已執行 [已輸入您的目標URL](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [建立對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [對象條件](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/audience-criteria.md){target="_blank"}
>* [Adobe PDF內嵌API](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-pdf-embed-api.md){target="_blank"}
