---
unique-page-id: 2359422
description: 個人化電子郵件-Marketo文檔——產品文檔
title: 個人化電子郵件
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 個人化電子郵件{#personalize-an-email}

## 任務：新增資料Token {#mission-make-your-emails-personal-by-adding-data-tokens}，讓您的電子郵件變成個人化

>[!PREREQUISITES]
>
>* [設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [傳送電子郵件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md)
>* [滴水，滴水，培養](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)


## 步驟1:選擇要個性化{#step-select-an-email-to-personalize}的電子郵件

1. 選擇在[上一個quick win](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)中建立的培訓電子郵件之一，然後按一下&#x200B;**編輯草稿**。

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >這會建立電子郵件的草稿副本。 您必須核准變更的草稿才能上線。

如果您尚未啟用快顯封鎖程式，電子郵件編輯器將會在新的標籤／視窗中開啟。 否則，請按兩下「編輯草稿」。****

## 步驟2:讓銷售人員成為發件人{#step-make-the-salesperson-the-sender}

1. 選擇&#x200B;**From**&#x200B;欄位、反白顯示並刪除&#x200B;**目前名稱。**

   ![](assets/two-5.png)

1. 按一下&#x200B;**From**&#x200B;欄位右側的&#x200B;**Token**&#x200B;表徵圖。

   ![](assets/three-4.png)

1. 尋找並選取&#x200B;**`{{lead.Lead Owner First Name}}`**&#x200B;代號。

   ![](assets/four-3.png)

1. 鍵入您的公司名稱，並為&#x200B;**預設值**&#x200B;加上破折號，以確保在銷售代表的名字無法使用時顯示某些內容。 按一下&#x200B;**插入**。

   ![](assets/five-4.png)

1. 按一下&#x200B;**From**&#x200B;欄位中的空格鍵，確定游標會在您剛插入的Token後閃爍一個空格。 然後再按一下&#x200B;**Token**&#x200B;圖示。

   ![](assets/six-4.png)

1. 尋找並選取&#x200B;**`{{lead.Lead Owner Last Name}}`**&#x200B;代號。

   ![](assets/seven-5.png)

1. 為&#x200B;**預設值**&#x200B;鍵入「銷售」，然後按一下&#x200B;**插入**。

   ![](assets/eight-3.png)

## 步驟3:將銷售線索的名稱添加到電子郵件{#step-add-the-leads-name-to-the-email}

1. 選擇頂部的可編輯部分，按一下齒輪表徵圖並選擇&#x200B;**編輯**。

   ![](assets/nine-2.png)

1. 在&quot;Hello&quot;後面加一個空格，並將游標置於逗號前面，然後按一下「插入Token **」圖示。**

   ![](assets/ten-4.png)

1. 尋找並選取&#x200B;**`{{lead.First Name}}`**&#x200B;代號。

   ![](assets/eleven-4.png)

1. 在&#x200B;**Default Value**&#x200B;欄位中輸入&quot;Friend&quot;（或您想要的任何標籤），然後按一下&#x200B;**Insert**。

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >一律包含Token的預設值；這可確保在遺失部分個人資訊時，會在電子郵件中顯示預設值。

1. 按一下&#x200B;**保存**。

   ![](assets/thirteen-3.png)

1. 關閉電子郵件編輯器頁籤／窗口。

   ![](assets/fourteen-3.png)

1. 在&#x200B;**電子郵件操作**&#x200B;下，選擇&#x200B;**批准草稿**。

   ![](assets/fifteen-3.png)

>[!TIP]
>
>需要快速複習一下如何自己傳送電子郵件？ 請參閱[傳送電子郵件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md)。

### 任務完成{#mission-complete}

恭喜您，您的電子郵件已個人化！

<br> 

[◄使命6:滴水，滴水，培養](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任務8:通知銷售代表►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
