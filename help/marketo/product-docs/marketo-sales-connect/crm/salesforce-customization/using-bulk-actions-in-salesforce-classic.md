---
unique-page-id: 42762794
description: 在Salesforce Classic中使用大量動作 — Marketo檔案 — 產品檔案
title: 在Salesforce Classic中使用大量動作
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 在Salesforce Classic中使用大量動作 {#using-bulk-actions-in-salesforce-classic}

了解如何執行大量動作，例如將銷售機會新增至行銷活動、傳送大量電子郵件或將銷售機會從Salesforce推送至Sales Connect。

>[!PREREQUISITES]
>
>更新為最新版本的Sales Connect包，並在銷售機會/聯繫人視圖中安裝批量操作按鈕。 [按一下這裡以取得指示](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>執行上述步驟之前，請確定您已登入Marketo Sales Connect帳戶。

## 大量電子郵件 {#bulk-email}

1. 在Salesforce中，按一下 **銷售機會** ，然後 **開始** 按鈕。

   ![](assets/one-5.png)

1. 選擇所需的銷售機會，然後按一下 **使用MSC(Classic)的電子郵件** 按鈕。

   ![](assets/two-5.png)

1. MSC電子郵件會彈出。 包含下列功能：

   a.&quot;To&quot;欄位顯示&quot;All receipts&quot; — 此欄位與您在「銷售線索清單視圖」中選擇的銷售線索清單相對應\
   b.左側面板上會顯示此清單，稱為「大量撰寫」 — 您可以在此處新增/移除收件者\
   c.您可以選擇範本或建立自己的電子郵件\
   d.您可以預覽要填入電子郵件的動態欄位\
   e.您可以立即傳送電子郵件，或排程稍後傳送

   ![](assets/three-4.png)

## 新增至Campaign {#add-to-campaign}

1. 在Salesforce中，按一下 **銷售機會** ，然後 **開始** 按鈕。

   ![](assets/four-3.png)

1. 選擇所需的銷售機會，然後按一下 **新增至MSC Campaign(Classic)** 按鈕。

   ![](assets/five-3.png)

1. 將會出現「將人員新增至您的促銷活動」快顯視窗。 按一下 **下一個** 並瀏覽一般促銷活動流程，以觸發MSC促銷活動。

   ![](assets/six.png)

## 推送至Marketo Sales Connect {#push-to-marketo-sales-connect}

1. 在Salesforce中，按一下 **銷售機會** ，然後 **開始** 按鈕。

   ![](assets/seven-1.png)

1. 選擇所需的銷售機會，然後按一下 **推送至MSC(Classic)** 按鈕。

   ![](assets/eight-1.png)

1. 將開啟一個名為「Salesforce Bridge」的新頁簽。 按一下 **繼續到組→** 按鈕。

   ![](assets/nine-1.png)

1. 您將被發送到MSC帳戶，在該帳戶中您將看到使用日期/時間戳建立的組。 同步完成後，您會收到通知，且群組將包含從Salesforce同步的銷售機會。

   ![](assets/ten.png)

>[!NOTE]
>
>您也可以依照相同步驟，在「聯繫人清單視圖」中使用批量操作。

>[!MORELIKETHIS]
>
>* [透過群組電子郵件傳送電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [使用選擇和發送合成大量電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

