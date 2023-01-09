---
description: 串流設計工具 — Marketo檔案 — 產品檔案
title: 流程設計工具
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: 24075208786077797f4917a2907b6dcfec7ed7bf
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 2%

---

# 流程設計工具 {#stream-designer}

有 _many_ 可能的流組合。 本文包含行銷人員詢問網站訪客是否有任何產品問題的範例。 如果是，訪客可以排程約會。 若否，訪客可選擇加入郵件清單以供未來通信之用。 酒店還提供免費PDF。 最終目標是排程約會或收集訪客的電子郵件。

>[!PREREQUISITES]
>
>您必須先 [設定](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target=&quot;_blank&quot;})。

## 串流設計工具卡 {#stream-designer-cards}

流設計器包含多張可添加的卡，以形成聊天對話。

<table>
 <tr>
  <td><strong>訊息</strong></td>
  <td>當您想要做陳述而不需要回應時使用(例如：「嗨！ 使用代碼SAVE25」時，所有項目今天可節省25%。
</td>
 </tr>
 <tr>
  <td><strong>問題</strong></td>
  <td>當您想要詢問多選題時使用，您會提供可用的回應(例如：你對哪種車感興趣？ 回應= SUV、小型車、卡車等)。</td>
 </tr>
 <tr>
  <td><strong>文件</strong></td>
  <td>可讓您在對話方塊中內嵌PDF檔案，並追蹤訪客的檔案參與活動（如果已下載檔案，已檢視多少頁面，和/或任何已使用的搜尋詞）。</td>
 </tr>
 <tr>
  <td><strong>資訊擷取</strong></td>
  <td>收集資訊時使用。 要選擇的三個欄位是「電子郵件地址」、「電話號碼」和「文字」（這可讓訪客自行撰寫訊息）。</td>
 </tr>
 <tr>
  <td><strong>約會排程器</strong></td>
  <td>為訪客提供可用日期的日曆，以排程後續作業。 日曆可用性反映 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">下一個代理排隊</a>.</td>
 </tr>
 <tr>
  <td><strong>目標</strong></td>
  <td>這是訪客唯一看不到的卡片。 您可以決定在哪個時間點在特定聊天內達成目標(例如：如果收集訪客的電子郵件是您的目標，請將「目標」卡片緊接在資料流中的「資訊擷取」之後)。</td>
 </tr>
</table>

## 流設計器表徵圖 {#stream-designer-icons}

在串流設計工具的右上角，您會看到幾個圖示。 他們做的是。

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>為偏好該檢視的使用者新增背景格線</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>放大，建立更大的卡片</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>縮小，建立較小的卡</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>開啟一個窗口，供您測試聊天（按相同按鈕關閉）</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>排列資料流中的所有卡片</td>
 </tr>
</table>

## 建立資料流 {#create-a-stream}

1. 等你 [建立對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}，按一下 **串流設計工具** 標籤。

   ![](assets/stream-designer-6.png)

1. 拖放「問題」卡片。

   ![](assets/stream-designer-7.png)

1. 在「查特博特回應」下，回答您想問的問題。

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >您可以使用代號來個人化已知聊天訪客的體驗(例如：Hello `{{lead.leadFirstName:""}}`)。 只需按一下右側的大括弧圖示並進行選取即可。 如果您希望匿名訪客看到通用內容，請在引號之間新增預設值(例如：Hello `{{lead.leadFirstName:"there"}}`)。

   >[!NOTE]
   >
   >Poke預設設為開啟，這會在聊天圖示旁顯示開頭問題，訪客不必按一下它即可檢視。 Poke僅在對話的第一張卡上可用。

1. 輸入您的使用者回應，然後按一下 **儲存**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**編輯儲存的值** 對於想要將不同值儲存在資料庫中的訪客，「問題」卡片中對應屬性的查詢機器人中，會顯示哪些值，這是可選步驟(例如：訪客看見「搜尋引擎最佳化」，您將該值儲存為「SEO」。)

1. 對於「是」，我們要計畫約會，因此在下面，該選項將拖動到「約會計畫程式」卡上。

   ![](assets/stream-designer-10.png)

1. 在右側的欄中，按一下 **儲存**.

   ![](assets/stream-designer-11.png)

1. 因為這是目標，請將「目標」卡拖曳至「約會排程器」下方。

   ![](assets/stream-designer-12.png)

1. 為目標命名（或選擇現有目標），然後按一下 **儲存**.

   ![](assets/stream-designer-13.png)

1. 若為「否」，我們想查看他們是否會加入郵寄清單，因此在選項下方，拖曳至另一張「問題」卡。

   ![](assets/stream-designer-14.png)

1. 輸入您的回應，並為訪客新增回應選擇。 按一下 **儲存** 時才能使用。

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >您可以按一下 **新增回應**.

1. 在「是」回應下方，拖曳至「資訊擷取」卡片上，以便收集訪客的電子郵件。

   ![](assets/stream-designer-16.png)

1. 按一下 **類型** 下拉式清單並選取 **電子郵件**.

   ![](assets/stream-designer-17.png)

1. 輸入聊天機器人訊息和預留位置。 確認屬性已對應至Marketo中的適當欄位，然後按一下 **儲存**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td><strong>類型</strong></td>
     <td>要捕獲的資訊類型：電話，簡訊，電子郵件。</td>
    </tr>
    <tr>
     <td><strong>聊天機器人訊息</strong></td>
     <td>訪客看到的訊息會提示他們提供資訊。</td>
    </tr>
    <tr>
     <td><strong>預留位置</strong></td>
     <td>可協助訪客查看要輸入的內容的範例文字。</td>
    </tr>
    <tr>
     <td><strong>將回應對應到屬性</strong></td>
     <td>可讓您將訪客的回應同步至其Marketo訂閱之人員記錄中的對應欄位。</td>
    </tr>
   </table>

1. 由於收集其電子郵件是目標，請將「目標」卡拖曳至「資訊擷取」下方。

   ![](assets/stream-designer-19.png)

1. 為目標命名（或選擇現有目標），然後按一下 **儲存**.

   ![](assets/stream-designer-20.png)

1. 如果他們說「否」，請記得新增回應。 一個選項是拖曳訊息卡到下方，說「反正謝謝」。 但在此範例中，我們會改為提供免費的PDF檔案。

   ![](assets/stream-designer-21.png)

1. 在此示例中，我們將建立新文檔。 請為其命名，輸入您已托管的PDF的URL，然後按一下 **儲存**.

   ![](assets/stream-designer-22.png)

1. 選取 **預覽** 切換以預覽對話方塊。

   ![](assets/stream-designer-23.png)

1. 準備好啟動對話方塊時，按一下 **發佈**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>按一下「發佈」之前，請記得確定您已 [輸入目標URL](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target=&quot;_blank&quot;}。

>[!MORELIKETHIS]
>
>* [建立對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [對象條件](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;}
>* [報表](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}
>* [使用文檔卡](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target=&quot;_blank&quot;}

