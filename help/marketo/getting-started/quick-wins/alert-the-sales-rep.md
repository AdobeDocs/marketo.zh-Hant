---
unique-page-id: 2359424
description: 提醒銷售代表 — Marketo檔案 — 產品檔案
title: 警示銷售代表
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 警示銷售代表 {#alert-the-sales-rep}

## 任務：當某人填寫您網站上的表單時提醒銷售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

若要自動傳送警示電子郵件給銷售代表，您只需要警示電子郵件和電子郵件行銷活動即可。 以下是其操作方式。

>[!PREREQUISITES]
>
>[含有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步驟1：建立警報電子郵件 {#step-create-an-alert-email}

1. 移至&#x200B;**[!UICONTROL Marketing Activities]**&#x200B;區域。

   ![](assets/alert-the-sales-rep-1.png)

1. 選取您在&#x200B;**登陸頁面（含表單**&#x200B;快速入門）中建立的[我的程式](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}，然後在&#x200B;**[!UICONTROL New]**&#x200B;底下按一下&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/alert-the-sales-rep-2.png)

1. 按一下「**[!UICONTROL Email]**」。

   ![](assets/alert-the-sales-rep-3.png)

1. **將電子郵件命名為「我的電子郵件警示」**，選取範本並按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/alert-the-sales-rep-4.png)

1. 輸入您想要銷售團隊檢視的&#x200B;**寄件者名稱**、**寄件者電子郵件**、**[!UICONTROL Reply-to]**&#x200B;和&#x200B;**[!UICONTROL Subject]**。

   ![](assets/alert-the-sales-rep-5.png)

1. 按兩下以編輯電子郵件文字。

   ![](assets/alert-the-sales-rep-6.png)

1. 輸入電子郵件內容。

   ![](assets/alert-the-sales-rep-7.png)

1. 將游標放在您要插入人員聯絡資訊的位置，然後按一下&#x200B;**插入Token**&#x200B;圖示。

   ![](assets/alert-the-sales-rep-8.png)

1. 尋找並選取`{{SP_Send_Alert_Info}}` **[!UICONTROL Token]**&#x200B;並按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}}是警示電子郵件的特殊權杖。 請參閱[使用傳送警示資訊Token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"}瞭解更多資訊。

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/alert-the-sales-rep-10.png)

1. 按一下&#x200B;**[!UICONTROL Email Actions]**&#x200B;下拉式清單，然後選取&#x200B;**[!UICONTROL Approve and Close]**。

   ![](assets/alert-the-sales-rep-11.png)

## 步驟2：建立警報觸發程式行銷活動 {#step-create-an-alert-trigger-campaign}

1. 選取先前建立的&#x200B;**我的程式**，然後在&#x200B;**[!UICONTROL New]**&#x200B;下按一下&#x200B;**[!UICONTROL New Smart Campaign]**。

   ![](assets/alert-the-sales-rep-12.png)

1. **將行銷活動命名為**&#x200B;我的警示行銷活動，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/alert-the-sales-rep-13.png)

1. 在「**[!UICONTROL Smart List]**」標籤下方，尋找&#x200B;**[!UICONTROL Fills Out Form]**&#x200B;觸發器並將其拖曳至畫布。

   ![](assets/alert-the-sales-rep-14.png)

1. 選取我們先前建立的表單。

   ![](assets/alert-the-sales-rep-15.png)

1. 在「**[!UICONTROL Flow]**」標籤下方，尋找&#x200B;**[!UICONTROL Send Alert]**&#x200B;流量動作並將其拖曳至畫布。

   ![](assets/alert-the-sales-rep-16.png)

1. 選取先前建立的&#x200B;**[!UICONTROL My Alert Email]**&#x200B;並保留&#x200B;**[!UICONTROL Send To]**&#x200B;為&#x200B;**[!UICONTROL Sales Owner]**。

   ![](assets/alert-the-sales-rep-17.png)

1. 在&#x200B;**[!UICONTROL To Other Emails]**&#x200B;欄位中輸入您的電子郵件地址。

   ![](assets/alert-the-sales-rep-18.png)

1. 前往&#x200B;**[!UICONTROL Schedule]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL Activate]**&#x200B;按鈕。

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >將&#x200B;**[!UICONTROL Qualification Rules]**&#x200B;設為&#x200B;**[!UICONTROL every time]** （透過編輯Smart Campaign），以允許同一人多次觸發警報。

1. 按一下確認畫面上的&#x200B;**[!UICONTROL Activate]**。

   ![](assets/alert-the-sales-rep-20.png)

## 步驟3：測試！ {#step-test-it-out}

1. 選取您的登入頁面並按一下&#x200B;**[!UICONTROL View Approved Page]**。

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >別忘了核准登陸頁面；這些頁面要等到核准後才會上線。

1. 填寫表單並按一下&#x200B;**[!UICONTROL Submit]**。

   ![](assets/alert-the-sales-22.png)

1. 您應該很快就會收到電子郵件。 在您確認一切都正常運作後，請從「傳送警報」流程中移除您的電子郵件地址（請參閱上述步驟2.7）。

   >[!NOTE]
   >
   >按一下Marketo中的&#x200B;**[!UICONTROL Person Info]**&#x200B;索引標籤以檢視連絡人資訊。

## 任務完成！ {#mission-complete}

<br> 

[◄任務7：個人化電子郵件](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[任務9：更新個人資料►](/help/marketo/getting-started/quick-wins/update-person-data.md)
