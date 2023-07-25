---
unique-page-id: 2359424
description: 提醒銷售代表 — Marketo檔案 — 產品檔案
title: 警示銷售代表
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# 警示銷售代表 {#alert-the-sales-rep}

## 任務：當某人填寫您網站上的表單時提醒銷售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

若要自動傳送警示電子郵件給銷售代表，您只需要警示電子郵件和電子郵件行銷活動即可。 以下是其操作方式。

>[!PREREQUISITES]
>
>[含有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步驟1：建立警報電子郵件 {#step-create-an-alert-email}

1. 前往 **[!UICONTROL 行銷活動]** 區域。

   ![](assets/alert-the-sales-rep-1.png)

1. 選取 **我的程式** 您建立於 [含有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} 快速獲勝，然後在 **[!UICONTROL 新增]** 按一下 **[!UICONTROL 新增本機資產]**.

   ![](assets/alert-the-sales-rep-2.png)

1. 按一下 **[!UICONTROL 電子郵件]**.

   ![](assets/alert-the-sales-rep-3.png)

1. **名稱** 電子郵件「我的電子郵件警示」，選擇範本並按一下 **[!UICONTROL 建立]**.

   ![](assets/alert-the-sales-rep-4.png)

1. 輸入 **發件人名稱**， **來自電子郵件**， **[!UICONTROL 回覆]**、和 **[!UICONTROL 主旨]** 您希望您的銷售團隊看到的內容。

   ![](assets/alert-the-sales-rep-5.png)

1. 按兩下以編輯電子郵件文字。

   ![](assets/alert-the-sales-rep-6.png)

1. 輸入電子郵件內容。

   ![](assets/alert-the-sales-rep-7.png)

1. 將游標放在您要插入人員連絡資訊的位置，然後按一下 **插入Token** 圖示。

   ![](assets/alert-the-sales-rep-8.png)

1. 尋找並選取 `{{SP_Send_Alert_Info}}` **[!UICONTROL Token]** 並按一下 **[!UICONTROL 插入]**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} 是警報電子郵件的特殊Token。 另請參閱 [使用傳送警報資訊權杖](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"} 以深入瞭解。

1. 按一下 **[!UICONTROL 儲存]**.

   ![](assets/alert-the-sales-rep-10.png)

1. 按一下 **[!UICONTROL 電子郵件動作]** 下拉式清單並選取 **[!UICONTROL 核准並關閉]**.

   ![](assets/alert-the-sales-rep-11.png)

## 步驟2：建立警報觸發程式行銷活動 {#step-create-an-alert-trigger-campaign}

1. 選取 **我的程式** 先前建立，然後在 **[!UICONTROL 新增]** 按一下 **[!UICONTROL 新增Smart Campaign]**.

   ![](assets/alert-the-sales-rep-12.png)

1. **名稱** 行銷活動「我的警示行銷活動」並按一下 **[!UICONTROL 建立]**.

   ![](assets/alert-the-sales-rep-13.png)

1. 在 **[!UICONTROL 智慧清單]** 標籤，尋找並拖曳 **[!UICONTROL 填寫表單]** 觸發至畫布。

   ![](assets/alert-the-sales-rep-14.png)

1. 選取我們先前建立的表單。

   ![](assets/alert-the-sales-rep-15.png)

1. 在 **[!UICONTROL 流量]** 標籤，尋找並拖曳 **[!UICONTROL 傳送警報]** 流程動作至畫布。

   ![](assets/alert-the-sales-rep-16.png)

1. 選取 **[!UICONTROL 我的警示電子郵件]** 先前建立並離開 **[!UICONTROL 傳送至]** 作為 **[!UICONTROL 銷售負責人]**.

   ![](assets/alert-the-sales-rep-17.png)

1. 在「 」中輸入您的電子郵件地址 **[!UICONTROL 至其他電子郵件]** 欄位。

   ![](assets/alert-the-sales-rep-18.png)

1. 前往 **[!UICONTROL 排程]** 標籤並按一下 **[!UICONTROL 啟動]** 按鈕。

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >設定 **[!UICONTROL 資格規則]** 至 **[!UICONTROL 每次]** （透過編輯Smart Campaign）以允許同一人多次觸發警報。

1. 按一下 **[!UICONTROL 啟動]** 確認畫面上。

   ![](assets/alert-the-sales-rep-20.png)

## 步驟3：測試！ {#step-test-it-out}

1. 選取您的登入頁面，然後按一下 **[!UICONTROL 檢視已核准頁面]**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >別忘了核准登陸頁面；這些頁面要等到核准後才會上線。

1. 填寫表單並按一下 **[!UICONTROL 提交]**.

   ![](assets/alert-the-sales-22.png)

1. 您很快就會收到電子郵件。 在您確認一切都正常運作後，請從「傳送警報」流程中移除您的電子郵件地址（請參閱上述步驟2.7）。

   >[!NOTE]
   >
   >按一下 **[!UICONTROL 個人資訊]** 按Tab鍵檢視Marketo中的聯絡人資訊。

## 任務完成！ {#mission-complete}

<br> 

[◄任務7：個人化電子郵件](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[任務9：更新人員資料►](/help/marketo/getting-started/quick-wins/update-person-data.md)
