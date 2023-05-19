---
unique-page-id: 2359422
description: 個性化電子郵件 — Marketo文檔 — 產品文檔
title: 個性化電子郵件
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 80512816eaf0a70a3f10a50c34aeea14edd9046b
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 個性化電子郵件 {#personalize-an-email}

## 任務：通過添加資料令牌，將您的電子郵件變為個人電子郵件 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [設定並添加人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [發送電子郵件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [滴水，滴水，撫育](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}


## 步驟1:選擇要個性化的電子郵件 {#step-select-an-email-to-personalize}

1. 選擇在 [上一場速勝](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} 按一下 **[!UICONTROL 建立草稿]**。

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >這將建立電子郵件的草稿副本。 切記批准要生效的更改的草稿。

如果尚未啟用彈出窗口阻止程式，電子郵件編輯器將在新的頁籤/窗口中開啟。 否則，按一下 **[!UICONTROL 建立繪製]** 兩次。

## 步驟2:將銷售人員設定為發件人 {#step-make-the-salesperson-the-sender}

1. 選擇 **[!UICONTROL 從]** 欄位，突出顯示和 **刪除** 當前名稱。

   ![](assets/personalize-an-email-2.png)

1. 按一下 **令牌** 表徵圖 **[!UICONTROL 從]** 的子菜單。

   ![](assets/personalize-an-email-3.png)

1. 查找並選擇 **`{{lead.Lead Owner First Name}}`** 標籤。

   ![](assets/personalize-an-email-4.png)

1. 鍵入公司名稱，並為 **預設值** 以確保在銷售代表的名字不可用時顯示某些內容。 按一下 **插入**。

   ![](assets/personalize-an-email-5.png)

1. 按下 **[!UICONTROL 從]** 欄位，確保游標在您剛剛插入的標籤後閃爍一個空格。 然後按一下 **令牌** 的子菜單。

   ![](assets/personalize-an-email-6.png)

1. 查找並選擇 **`{{lead.Lead Owner Last Name}}`** 標籤。

   ![](assets/personalize-an-email-7.png)

1. 鍵入「銷售」 **預設值** 按一下 **插入**。

   ![](assets/personalize-an-email-8.png)

## 第3步：將Lead的名稱添加到電子郵件 {#step-add-the-leads-name-to-the-email}

1. 選擇頂部可編輯部分，按一下齒輪表徵圖並選擇 **[!UICONTROL 編輯]**。

   ![](assets/personalize-an-email-9.png)

1. 在「Hello」後添加空格，將游標置於逗號前，然後按一下 **插入標籤** 表徵圖

   ![](assets/personalize-an-email-10.png)

1. 查找並選擇 **`{{lead.First Name}}`** 標籤。

   ![](assets/personalize-an-email-11.png)

1. 在中輸入「朋友」（或您想要的任何標籤） **[!UICONTROL 預設值]** 按一下 **[!UICONTROL 插入]**。

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >始終包含令牌的預設值；這可確保在丟失部分個人資訊時，在電子郵件中顯示預設值。

1. 按一下 **[!UICONTROL 保存]**。

   ![](assets/personalize-an-email-13.png)

1. 下 **[!UICONTROL 電子郵件操作]** 選擇 **[!UICONTROL 批准和關閉]**。

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>需要快速複習一下如何自己發送電子郵件嗎？ 請參閱 [發送電子郵件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}。

### 任務完成 {#mission-complete}

恭喜，您已個性化了您的電子郵件！

<br> 

[◄任務6:滴水，滴水，撫育](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任務8:通知銷售代表►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
