---
unique-page-id: 5472678
description: 匯入非拉丁字元清單 — Marketo檔案 — 產品檔案
title: 匯入非拉丁字元清單
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 匯入非拉丁字元清單 {#import-a-non-latin-characters-list}

嘗試匯入非英文的檔案？ 當您使用Excel開啟清單時，它看起來會很完美。

![](assets/image2015-2-10-9-3a34-3a57.png)

但將其匯入Marketo時，您可能會發現未正確擷取非英文字元。

![](assets/image2015-2-10-9-3a35-3a49.png)

這是因為檔案未正確儲存，使得Marketo無法辨識所有非拉丁字元。 好消息是，您可以遵循一些簡單步驟來進行修正。

1. 從Excel的&#x200B;**[!UICONTROL Save As]功能表選取**...**[!UICONTROL File]**。

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. 選擇&#x200B;**[!UICONTROL UTF-16 Unicode Text (.txt)]**&#x200B;作為&#x200B;**[!UICONTROL Format]**&#x200B;選項。 這會以Marketo顯示檔案的方式進行編碼。

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo也支援UTF-8、Shift-JIS或EUC-JP。

1. Excel會將新檔案儲存為副檔名為.txt的文字檔。 但它也會將檔案中的所有逗號轉換為定位字元。 我們需要將它改回。

   >[!TIP]
   >
   >如果您使用Windows，可以使用&#x200B;**[!DNL Notepad]**&#x200B;開啟文字檔；如果您使用Mac，可以使用&#x200B;**[!DNL TextEdit]**。

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. 從檔案中選取索引標籤並複製。

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. 從&#x200B;**[!UICONTROL Find and Replace]功能表選取**...**[!UICONTROL Edit]**。

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Windows使用者的同等動作為： **[!UICONTROL Edit]> [!UICONTROL Replace]...**

1. 將您在步驟4中複製的標籤貼到第一個（要取代的）方塊中，並在第二個（取代為）方塊中輸入逗號。 然後按一下&#x200B;**[!UICONTROL All]**。

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. 好了，所有逗號都恢復了，我們準備好了。

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. 將新檔案匯入Marketo，這次應該會正確顯示資訊。

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >匯入的任何日期/時間欄位都會視為中央時間。 如果您的日期/時間欄位位於不同的時區，可以使用Excel公式將其轉換為中部時間（美洲/芝加哥）。

我們知道這很奇怪，但它很管用。 匯入愉快！
