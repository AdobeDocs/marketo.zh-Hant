---
unique-page-id: 2359416
description: 電子郵件自動回覆 - Marketo 文件 - 產品文件
title: 電子郵件自動回覆
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 100%

---

# 電子郵件自動回覆 {#email-auto-response}

## 任務：當有人填寫表單時傳送一封感謝電子郵件 {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [完成設定與新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [附有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步驟 1：建立電子郵件 {#step-create-an-email}

1. 前往「[!UICONTROL Marketing Activities]」區域。

   ![](assets/email-auto-response-1.png)

1. 在左側選單中選取您的方案，按一下「**[!UICONTROL New]**」下拉式選單，然後選取「**[!UICONTROL New Local Asset]**」。

   ![](assets/email-auto-response-2.png)

1. 選取「**[!UICONTROL Email]**」。

   ![](assets/email-auto-response-3.png)

1. 將您的電子郵件命名為「自動回覆電子郵件」，選擇一個範本，然後按一下「**[!UICONTROL Create]**」。

   ![](assets/email-auto-response-4.png)

   電子郵件編輯器會於新的視窗或索引標籤中開啟。若快顯視窗被封鎖，請按一下資產摘要頁面上的「**[!UICONTROL Edit Draft]**」來存取電子郵件。

1. 輸入主旨行的內容，然後按兩下電子郵件的可編輯區域。

   ![](assets/email-auto-response-5.png)

   _RTF 文字編輯器會於電子郵件編輯器頂部開啟。_

1. 醒目標示現有的電子郵件內容。

   ![](assets/email-auto-response-6.png)

1. 輸入您的電子郵件內容，然後按一下「**[!UICONTROL Save]**」。

   ![](assets/email-auto-response-7.png)

1. 按一下「**[!UICONTROL Email Actions]**」下拉式選單，選取「**[!UICONTROL Approve and Close]**」。

   ![](assets/email-auto-response-8.png)

## 步驟 2：建立智慧行銷活動 {#step-create-a-smart-campaign}

1. 選取您的方案，按一下「**[!UICONTROL New]**」下拉式選單，然後選取「**[!UICONTROL New Smart Campaign]**」。

   ![](assets/email-auto-response-9.png)

1. 將您的智慧行銷活動&#x200B;**命名**&#x200B;為「自動回覆行銷活動」，然後按一下「**[!UICONTROL Create]**」。

   ![](assets/email-auto-response-10.png)

1. 前往「**[!UICONTROL Smart List]**」索引標籤。

   ![](assets/email-auto-response-11.png)

   我們現在設定為每當有人填寫您在&#x200B;[**附有表單的登陸頁面**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}&#x200B;中建立的表單時，便會執行此行銷活動。

1. 找到「**[!UICONTROL Fills Out Form]**」觸發程序，將其拖曳至版面。

   ![](assets/email-auto-response-12.png)

1. 選取下拉式選單中的「**[!UICONTROL My Form]**」。然後按一下「**[!UICONTROL Flow]**」索引標籤。

   ![](assets/email-auto-response-13.png)

1. 將「**[!UICONTROL Send Email]**」流程動作拖曳至左側版面。

   ![](assets/email-auto-response-14.png)

1. 選取您的&#x200B;**自動回覆電子郵件**。然後按一下「**[!UICONTROL Schedule]**」索引標籤。

   ![](assets/email-auto-response-15.png)

1. 按一下「**[!UICONTROL Edit]**」。

   ![](assets/email-auto-response-16.png)

1. 選取「**[!UICONTROL every time]**」然後按一下「**[!UICONTROL Save]**」。

   ![](assets/email-auto-response-17.png)

1. 按一下「**[!UICONTROL Activate]**」。

   ![](assets/email-auto-response-18.png)

1. 在確認畫面上按一下「**[!UICONTROL Activate]**」。

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>啟動後，每當有人填寫指定表單時，此行銷活動就會執行。行銷活動會持續執行，直到停用為止。

## 步驟 3：填寫表單 {#step-fill-out-the-form}

1. 選取「**我的頁面**」(在[附有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}快速成果中所建立)，然後按一下「**[!UICONTROL Preview]**」。

   ![](assets/email-auto-response-20.png)

   _您的「免費試用」登陸頁面會在新的索引標籤中開啟。_

1. 在表單中填寫您的名字、姓氏和電子郵件地址，然後按一下「**[!UICONTROL Submit]**」。

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>請確保使用真實的電子郵件地址，方能收到電子郵件。

## 任務完成 {#mission-complete}

幾分鐘內，您便會在收件匣中看到自動回覆電子郵件。

[◄ 任務 3：簡單評分](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[任務 5：匯入人員清單 ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
