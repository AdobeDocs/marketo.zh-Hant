---
unique-page-id: 42762794
description: 在 [!DNL Salesforce] Classic - Marketo檔案 — 產品檔案中使用大量動作
title: 在 [!DNL Salesforce] 傳統版中使用大量動作
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# 在[!DNL Salesforce] Classic中使用大量動作 {#using-bulk-actions-in-salesforce-classic}

瞭解如何執行大量動作，例如將銷售機會新增至行銷活動、傳送大量電子郵件，或將銷售機會從[!DNL Salesforce]推播至[!DNL Sales Connect]。

>[!PREREQUISITES]
>
>更新至[!DNL Sales Connect]封裝的最新版本，並在您的銷售機會/聯絡人檢視中安裝大量動作按鈕。 [按一下這裡以取得指示](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)。

>[!NOTE]
>
>在依照列出的步驟操作之前，請確定您已登入您的Marketo Sales Connect帳戶。

## 大量電子郵件 {#bulk-email}

1. 在[!DNL Salesforce]中，按一下&#x200B;**[!UICONTROL Leads]**&#x200B;標籤，然後按&#x200B;**[!UICONTROL Go]**&#x200B;按鈕。

   ![](assets/one-5.png)

1. 選擇所需的銷售機會，然後按一下&#x200B;**[!UICONTROL Email with MSC (Classic)]**&#x200B;按鈕。

   ![](assets/two-5.png)

1. 將會出現MSC電子郵件。 它包含下列功能：

   a. &quot;[!UICONTROL To]&quot;欄位顯示&quot;[!UICONTROL All Recipients]&quot; — 這對應於您在「銷售機會清單檢視」中選擇的銷售機會清單\
   b.此清單會顯示在名為&quot;[!UICONTROL Bulk Compose]&quot;的左側面板上 — 您可以在此處新增/移除收件者\
   c.您可以選擇範本或建立您自己的電子郵件\
   d.您可以預覽將填入電子郵件中的動態欄位\
   e.您可以立即傳送電子郵件，或排程在稍後傳送

   ![](assets/three-4.png)

## 新增至行銷活動 {#add-to-campaign}

1. 在[!DNL Salesforce]中，按一下&#x200B;**[!UICONTROL Leads]**&#x200B;標籤，然後按&#x200B;**[!UICONTROL Go]**&#x200B;按鈕。

   ![](assets/four-3.png)

1. 選擇所需的銷售機會，然後按一下&#x200B;**[!UICONTROL Add to MSC Campaign (Classic)]**&#x200B;按鈕。

   ![](assets/five-3.png)

1. 「[!UICONTROL Add People to Your Campaign]」快顯視窗將會出現。 按一下&#x200B;**[!UICONTROL Next]**&#x200B;並透過一般促銷活動流程來觸發MSC促銷活動。

   ![](assets/six.png)

## 推送至Marketo Sales Connect {#push-to-marketo-sales-connect}

1. 在[!DNL Salesforce]中，按一下&#x200B;**[!UICONTROL Leads]**&#x200B;標籤，然後按&#x200B;**[!UICONTROL Go]**&#x200B;按鈕。

   ![](assets/seven-1.png)

1. 選擇所需的銷售機會，然後按一下&#x200B;**[!UICONTROL Push to MSC (Classic)]**&#x200B;按鈕。

   ![](assets/eight-1.png)

1. 將開啟名為「[!UICONTROL Salesforce Bridge]」的新索引標籤。 按一下&#x200B;**[!UICONTROL Proceed to Group →]**&#x200B;按鈕。

   ![](assets/nine-1.png)

1. 系統會將您傳送至您的MSC帳戶，您會在其中看到以日期/時間戳記建立的群組。 同步完成後，您將會收到通知，群組將會包含從[!DNL Salesforce]同步的潛在客戶。

   ![](assets/ten.png)

>[!NOTE]
>
>您也可以依照相同的步驟，在「連絡人清單檢視」中使用大量動作。

>[!MORELIKETHIS]
>
>* [透過群組電子郵件傳送電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [使用Select和Send撰寫大量電子郵件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
