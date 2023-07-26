---
unique-page-id: 42762825
description: 在Salesforce Lightning中使用大量動作 — Marketo檔案 — 產品檔案
title: 在Salesforce Lightning中使用大量動作
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 在Salesforce Lightning中使用大量動作 {#using-bulk-actions-in-salesforce-lightning}

瞭解如何執行大量動作，例如將銷售機會新增至行銷活動、傳送大量電子郵件，或將銷售機會從Salesforce推送至Sales Connect。

>[!PREREQUISITES]
>
>更新至最新版的Sales Connect套件，並在您的銷售機會/聯絡人檢視中安裝大量動作按鈕。 [按一下這裡以取得指示](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>在依照下列步驟操作之前，請確定您已登入您的Marketo Sales Connect帳戶。

## 大量電子郵件 {#bulk-email}

1. 在Salesforce中，按一下 **銷售機會** 索引標籤，然後選擇所需銷售機會的清單。

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >如果您已經位於要使用的清單中，您必須從下拉式清單中選擇它，以確保MSC大量動作按鈕顯示，以再次執行它。 這是無法變更的Salesforce行為。

1. 按一下箭頭下拉式清單（在畫面的最右側）並選取 **使用MSC傳送電子郵件**.

   ![](assets/two-6.png)

1. 將會出現MSC電子郵件。 它包含下列功能：

   a. 「收件者」欄位會顯示「所有收款」 — 這對應於您在「潛在客戶清單檢視表」中所選擇的潛在客戶清單\
   b.此清單會顯示在名為「大量撰寫」的左側面板上 — 您可以在此處新增/移除收件者\
   c.您可以選擇範本或建立您自己的電子郵件\
   d.您可以立即傳送電子郵件，或排程在稍後傳送

   ![](assets/three-5.png)

## 新增至行銷活動 {#add-to-campaign}

1. 在Salesforce中，按一下 **銷售機會** 索引標籤，然後選擇所需銷售機會的清單。

   ![](assets/four-4.png)

1. 按一下箭頭下拉式清單（在畫面的最右側）並選取 **新增至MSC Campaign**.

   ![](assets/five-4.png)

1. 將會出現「將人員新增至您的行銷活動」快顯視窗。 按一下 **下一個** 並透過一般促銷活動流程觸發MSC促銷活動。

   ![](assets/six-1.png)

## 推送至Marketo Sales Connect {#push-to-marketo-sales-connect}

1. 在Salesforce中，按一下 **銷售機會** 索引標籤，然後選擇所需銷售機會的清單。

   ![](assets/seven-2.png)

1. 按一下箭頭下拉式清單（在畫面的最右側）並選取 **推送至MSC**.

   ![](assets/eight-2.png)

1. 名為「Salesforce Bridge」的新索引標籤將會開啟。 按一下 **繼續前往群組→** 按鈕。

   ![](assets/nine-2.png)

1. 系統會將您傳送至您的MSC帳戶，您會在其中看到以日期/時間戳記建立的群組。 同步完成後，您將會收到通知，群組將包含從Salesforce同步的銷售機會。

   ![](assets/ten-1.png)

>[!NOTE]
>
>您也可以依照相同的步驟，在「連絡人清單檢視」中使用大量動作。

>[!MORELIKETHIS]
>
>* [透過群組電子郵件傳送電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [使用「選取並傳送」來撰寫大量電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
