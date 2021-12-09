---
description: 建立資料流 — Marketo檔案 — 產品檔案
title: 建立資料流
hide: true
hidefromtoc: true
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# 建立資料流 {#create-a-stream}

有 _many_ 您可以建立的資料流組合。 以下範例為行銷人員詢問網站訪客是否有任何產品問題。 如果是，訪客可以排程約會。 若否，訪客可選擇加入郵件清單以供未來通信之用。 目標是排程約會或收集訪客的電子郵件。

1. 在 [建立對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue)，按一下 **串流設計工具** 標籤。

   ![](assets/create-a-stream-1.png)

1. 拖放「問題」卡片。

   ![](assets/create-a-stream-2.png)

1. 在「查特博特回應」下，回答您想問的問題。

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Poke預設設為開啟，這會在聊天圖示旁顯示開頭問題，訪客不必按一下它即可檢視。

1. 輸入您的使用者回應，然後按一下 **儲存**.

   ![](assets/create-a-stream-4.png)

1. 對於「是」，我們要計畫約會，因此在下面，該選項將拖動到「約會計畫程式」卡上。

   ![](assets/create-a-stream-5.png)

1. 在右側的欄中，按一下 **儲存**.

   ![](assets/create-a-stream-6.png)

1. 因為這是目標，請將「目標」卡拖曳至「約會排程器」下方。

   ![](assets/create-a-stream-7.png)

1. 為目標命名（或選擇現有目標），然後按一下 **儲存**.

   ![](assets/create-a-stream-8.png)

1. 若為「否」，我們想查看他們是否會加入郵寄清單，因此在選項下方，拖曳至另一張「問題」卡。

   ![](assets/create-a-stream-9.png)

1. 輸入您的回應，並為訪客新增回應選擇。 按一下 **儲存** 時才能使用。

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >您可以按一下 **新增回應**.

1. 在「是」回應下方，拖曳至「資訊擷取」卡片上，以便收集訪客的電子郵件。

   ![](assets/create-a-stream-11.png)

1. 按一下 **類型** 下拉式清單並選取 **電子郵件**.

   ![](assets/create-a-stream-12.png)

1. 輸入聊天機器人訊息和預留位置。 確認屬性已對應至Marketo中的適當欄位，然後按一下 **儲存**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>類型</strong></td>
     <td>要捕獲的資訊類型：電話，簡訊，電子郵件。</td>
    </tr>
    <tr>
     <td><strong>Chatbot訊息</strong></td>
     <td>訪客看到的訊息會提示他們提供資訊。</td>
    </tr>
    <tr>
     <td><strong>預留位置</strong></td>
     <td>可協助訪客查看要輸入的內容的範例文字。</td>
    </tr>
    <tr>
     <td><strong>將回應對應至屬性</strong></td>
     <td>可讓您將訪客的回應同步至其Marketo訂閱之人員記錄中的對應欄位。</td>
    </tr>
   </table>

1. 由於收集其電子郵件是目標，請將「目標」卡拖曳至「資訊擷取」下方。

   ![](assets/create-a-stream-14.png)

1. 為目標命名（或選擇現有目標），然後按一下 **儲存**.

   ![](assets/create-a-stream-15.png)

1. 如果他們說「否」，請記得新增回應。 拖曳訊息卡至該選項下方。

   ![](assets/create-a-stream-16.png)

1. 輸入您的訊息，然後按一下 **儲存**.

   ![](assets/create-a-stream-17.png)

1. 要激活對話框時，按一下 **發佈**.

   ![](assets/create-a-stream-18.png)

>[!NOTE]
>
>按一下「發佈」之前，請記得確定您已 [輸入目標URL](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>[對話方塊](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
