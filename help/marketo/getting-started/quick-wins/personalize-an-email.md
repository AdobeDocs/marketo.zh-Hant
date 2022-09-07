---
unique-page-id: 2359422
description: 個人化電子郵件 — Marketo檔案 — 產品檔案
title: 個人化電子郵件
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 8aa2f3069c0168f57ac00dfc7270484a9045584c
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 個人化電子郵件 {#personalize-an-email}

## 任務：新增資料代號，讓您的電子郵件成為個人電子郵件 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [傳送電子郵件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}
>* [滴水，滴水，撫育](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}


## 步驟1:選取要個人化的電子郵件 {#step-select-an-email-to-personalize}

1. 選取 [上一次快速成功](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}，按一下 **建立草稿**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >這會以草稿形式建立電子郵件副本。 請記得核准草稿，變更才會上線。

如果您尚未啟用快顯封鎖程式，電子郵件編輯器將會在新索引標籤/視窗中開啟。 否則，按一下 **建立草稿** 兩次。

## 步驟2:將銷售人員設為寄件者 {#step-make-the-salesperson-the-sender}

1. 選取 **從** 欄位、突出顯示和 **刪除** 目前的名稱。

   ![](assets/personalize-an-email-2.png)

1. 按一下 **代號** 表徵圖 **從** 欄位。

   ![](assets/personalize-an-email-3.png)

1. 尋找並選取 **`{{lead.Lead Owner First Name}}`** 代號。

   ![](assets/personalize-an-email-4.png)

1. 輸入您的公司名稱，並加上破折號 **預設值** 以確保在銷售代表的名字不可用時顯示某些內容。 按一下 **插入**.

   ![](assets/personalize-an-email-5.png)

1. 點擊 **從** 欄位，確保游標在剛插入的令牌後閃爍一個空格。 然後按一下 **代號** 圖示。

   ![](assets/personalize-an-email-6.png)

1. 尋找並選取 **`{{lead.Lead Owner Last Name}}`** 代號。

   ![](assets/personalize-an-email-7.png)

1. 鍵入「Sales」 **預設值** 按一下 **插入**.

   ![](assets/personalize-an-email-8.png)

## 步驟3:將銷售機會名稱新增至電子郵件 {#step-add-the-leads-name-to-the-email}

1. 選取頂端可編輯的區段，按一下齒輪圖示並選取 **編輯**.

   ![](assets/personalize-an-email-9.png)

1. 在&quot;Hello&quot;後面添加一個空格，並將游標放在逗號前面，然後按一下 **插入代號** 表徵圖。

   ![](assets/personalize-an-email-10.png)

1. 尋找並選取 **`{{lead.First Name}}`** 代號。

   ![](assets/personalize-an-email-11.png)

1. 在 **預設值** 欄位，按一下 **插入**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >一律包含代號的預設值；這可確保在缺少部分個人資訊時，在電子郵件中顯示預設值。

1. 按一下 **儲存**.

   ![](assets/personalize-an-email-13.png)

1. 在 **電子郵件動作** 選取 **核准並關閉**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>需要快速重新整理一下如何傳送電子郵件給您自己嗎？ 請參閱 [傳送電子郵件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}。

### 任務完成 {#mission-complete}

恭喜，您的電子郵件已個性化！

<br> 

[◄任務6:滴水，滴水，撫育](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任務8:提醒銷售代表►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
