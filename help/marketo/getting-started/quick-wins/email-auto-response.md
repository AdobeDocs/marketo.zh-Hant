---
unique-page-id: 2359416
description: 電子郵件自動回應 — Marketo檔案 — 產品檔案
title: 電子郵件自動回應
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 2%

---

# 電子郵件自動回應 {#email-auto-response}

## 任務：有人填寫表單時，請傳送感謝電子郵件給您 {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [含有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步驟1：建立電子郵件 {#step-create-an-email}

1. 移至[!UICONTROL Marketing Activities]區域。

   ![](assets/email-auto-response-1.png)

1. 在左側功能表中選取您的程式，按一下&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/email-auto-response-2.png)

1. 選擇「**[!UICONTROL Email]**」。

   ![](assets/email-auto-response-3.png)

1. 將您的電子郵件命名為「自動回覆電子郵件」，選擇一個範本，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/email-auto-response-4.png)

   電子郵件編輯器將在新視窗或標籤中開啟。 如果封鎖快顯視窗，請按一下資產摘要頁面上的&#x200B;**[!UICONTROL Edit Draft]**&#x200B;以存取電子郵件。

1. 輸入主旨列，然後按兩下電子郵件的可編輯區域。

   ![](assets/email-auto-response-5.png)

   _RTF編輯器將會在電子郵件編輯器的上方開啟。_

1. 反白顯示現有的電子郵件內容。

   ![](assets/email-auto-response-6.png)

1. 輸入您的電子郵件內容並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/email-auto-response-7.png)

1. 按一下&#x200B;**[!UICONTROL Email Actions]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL Approve and Close]**。

   ![](assets/email-auto-response-8.png)

## 步驟2：建立Smart Campaign {#step-create-a-smart-campaign}

1. 選取您的程式，按一下&#x200B;**[!UICONTROL New]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL New Smart Campaign]**。

   ![](assets/email-auto-response-9.png)

1. **將您的智慧行銷活動命名為「自動回應行銷活動」**，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/email-auto-response-10.png)

1. 前往 **[!UICONTROL Smart List]** 標籤。

   ![](assets/email-auto-response-11.png)

   我們將設定此行銷活動，每當有人填寫您在&#x200B;[**登入頁面中建立的表單及表單**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}&#x200B;時執行。

1. 尋找&#x200B;**[!UICONTROL Fills Out Form]**&#x200B;觸發器並將其拖曳至畫布。

   ![](assets/email-auto-response-12.png)

1. 在下拉式清單中選取&#x200B;**[!UICONTROL My Form]**。 然後按一下「**[!UICONTROL Flow]**」標籤。

   ![](assets/email-auto-response-13.png)

1. 將&#x200B;**[!UICONTROL Send Email]**&#x200B;流量動作拖曳至左側畫布。

   ![](assets/email-auto-response-14.png)

1. 選取您的&#x200B;**自動回覆電子郵件**。 然後按一下「**[!UICONTROL Schedule]**」標籤。

   ![](assets/email-auto-response-15.png)

1. 按一下「**[!UICONTROL Edit]**」。

   ![](assets/email-auto-response-16.png)

1. 選取&#x200B;**[!UICONTROL every time]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/email-auto-response-17.png)

1. 按一下「**[!UICONTROL Activate]**」。

   ![](assets/email-auto-response-18.png)

1. 按一下確認畫面上的&#x200B;**[!UICONTROL Activate]**。

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>一旦啟用，此行銷活動就會在每次有人填寫指定表單時執行。 行銷活動將持續執行直到其停用。

## 步驟3：填寫表單 {#step-fill-out-the-form}

1. 選取&#x200B;**我的頁面** （這是在[登陸頁面中以表單](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}快速成功建立的）並按一下&#x200B;**[!UICONTROL Preview]**。

   ![](assets/email-auto-response-20.png)

   _您的「免費試用」登陸頁面將在新標籤中開啟。_

1. 填寫您的名字、姓氏和電子郵件地址，然後按一下&#x200B;**[!UICONTROL Submit]**。

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>請務必使用您實際的電子郵件地址，以便取得電子郵件。

## 任務完成 {#mission-complete}

在幾分鐘內，您應該就會在收件匣中看到自動回應電子郵件。

[◄個任務3：簡單評分](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[任務5：匯入人員清單►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
