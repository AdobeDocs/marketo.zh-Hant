---
description: 流設計器 — Marketo文檔 — 產品文檔
title: 流設計器
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: adf3a9f156ec5ed823a0647affb87f6c0686d35f
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# 流設計器 {#stream-designer}

有 _許多_ 可以建立的流組合。 本文包含一個示例，在該示例中，商家詢問站點訪問者是否有任何產品問題。 如果是，訪問者可以安排預約。 如果否，則允許訪問者加入郵件清單以供將來通信。 目標是安排約會或收集訪問者的電子郵件。

## 流設計卡 {#stream-designer-cards}

流設計器包含多個可添加以塑造聊天對話形狀的卡。

<table>
 <tr>
  <td><strong>訊息</strong></td>
  <td>在您想要生成無需響應的語句時使用(例如：「嗨！ 所有項目今天都減少了25%，代碼為SAVE25")。
</td>
 </tr>
 <tr>
  <td><strong>問題</strong></td>
  <td>當您想問多選題時使用，您將提供其可用回答(例如：你對哪種車感興趣？ 響應= SUV、緊湊型、卡車等)。</td>
 </tr>
 <tr>
  <td><strong>資訊捕獲</strong></td>
  <td>在要收集資訊時使用。 要選擇的三個欄位是「電子郵件地址」、「電話號碼」和「文本」（允許訪問者自行寫郵件）。</td>
 </tr>
 <tr>
  <td><strong>約會計畫程式</strong></td>
  <td>為訪問者提供可用日期日曆，以安排後續活動。 日曆可用性反映 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">下一個聯機代理</a>。</td>
 </tr>
 <tr>
  <td><strong>目標</strong></td>
  <td>這是訪客看不到的唯一一張牌。 您需要確定在特定聊天中的哪個點實現目標(例如：如果收集訪問者的電子郵件是您的目標，請將目標卡立即放在流中「資訊捕獲」之後)。</td>
 </tr>
</table>

## 建立流 {#create-a-stream}

1. 等你 [已建立對話框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}，按一下 **流設計器** 頁籤。

   ![](assets/create-a-stream-1.png)

1. 拖放問題卡。

   ![](assets/create-a-stream-2.png)

1. 在查博回應下，你想問什麼。

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >預設情況下，Poke設定為on ，即在聊天表徵圖旁顯示開題，而訪問者不必按一下它即可查看。

1. 輸入用戶響應，然後按一下 **保存**。

   ![](assets/create-a-stream-4.png)

1. 對於「是」，我們要安排約會，因此在該選項下方拖動到約會計畫程式卡上。

   ![](assets/create-a-stream-5.png)

1. 在右側的列中，按一下 **保存**。

   ![](assets/create-a-stream-6.png)

1. 因為這是目標，請將目標卡拖到約會計畫程式下面。

   ![](assets/create-a-stream-7.png)

1. 命名目標（或選擇現有目標），然後按一下 **保存**。

   ![](assets/create-a-stream-8.png)

1. 對於「否」，我們希望查看他們是否會加入郵件清單，因此，在該選項下面，將其拖動到另一問號卡上。

   ![](assets/create-a-stream-9.png)

1. 輸入您的響應，並為訪問者添加響應選項。 按一下 **保存** 完成。

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >您可以通過按一下 **添加響應**。

1. 在「Yes（是）」響應下，拖動「Info Capture（資訊捕獲）」卡，以便收集訪問者的電子郵件。

   ![](assets/create-a-stream-11.png)

1. 按一下 **類型** 下拉並選擇 **電子郵件**。

   ![](assets/create-a-stream-12.png)

1. 輸入聊天器消息和佔位符。 確保屬性映射到Marketo的相應欄位，然後按一下 **保存**。

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>類型</strong></td>
     <td>要捕獲的資訊類型：電話，簡訊，電子郵件。</td>
    </tr>
    <tr>
     <td><strong>查特博特消息</strong></td>
     <td>訪問者看到的消息提示他們提供資訊。</td>
    </tr>
    <tr>
     <td><strong>佔位符</strong></td>
     <td>幫助訪問者查看要輸入的內容的示例文本。</td>
    </tr>
    <tr>
     <td><strong>將響應映射到屬性</strong></td>
     <td>允許您將訪問者的響應同步到您的Marketo訂閱中其人員記錄中的相應欄位。</td>
    </tr>
   </table>

1. 由於收集其電子郵件是一個目標，請將目標卡拖到「資訊捕獲」下。

   ![](assets/create-a-stream-14.png)

1. 命名目標（或選擇現有目標），然後按一下 **保存**。

   ![](assets/create-a-stream-15.png)

1. 如果他們說「否」，請記住添加一個響應。 將留言卡拖到該選項下面。

   ![](assets/create-a-stream-16.png)

1. 輸入您的消息，然後按一下 **保存**。

   ![](assets/create-a-stream-17.png)

1. 選擇 **預覽** 切換以預覽對話框。

   ![](assets/create-a-stream-18.png)

1. 準備好激活對話框後，按一下 **發佈**。

   ![](assets/create-a-stream-19.png)

>[!NOTE]
>
>在按一下「發佈」之前，請記住確保 [已輸入目標URL](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target=&quot;_blank&quot;}。

>[!MORELIKETHIS]
>
>* [建立對話框](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;
>* [受眾標準](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;
>* [報告](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;

