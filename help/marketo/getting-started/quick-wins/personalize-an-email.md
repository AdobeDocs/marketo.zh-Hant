---
unique-page-id: 2359422
description: 個人化電子郵件 — Marketo檔案 — 產品檔案
title: 個人化電子郵件
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 個人化電子郵件 {#personalize-an-email}

## 任務：新增資料權杖，讓您的電子郵件更個人化 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [傳送電子郵件Blast](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [滴水，滴水， Nurture](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## 步驟1：選取要個人化的電子郵件 {#step-select-an-email-to-personalize}

1. 選取在[上一個快速入門](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}中建立的其中一個Nurture電子郵件，然後按一下&#x200B;**[!UICONTROL 建立草稿]**。

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >這會建立一份電子郵件作為草稿。 請記得核准草稿，讓變更生效。

如果您尚未啟用快顯封鎖程式，電子郵件編輯器將在新的索引標籤/視窗中開啟。 否則，請按兩下[建立草稿]。**&#x200B;**

## 步驟2：將業務代表設為寄件者 {#step-make-the-salesperson-the-sender}

1. 選取&#x200B;**[!UICONTROL 從]**&#x200B;欄位，反白顯示並&#x200B;**刪除**&#x200B;目前名稱。

   ![](assets/personalize-an-email-2.png)

1. 按一下&#x200B;**[!UICONTROL 寄件者]**&#x200B;欄位右側的&#x200B;**Token**&#x200B;圖示。

   ![](assets/personalize-an-email-3.png)

1. 尋找並選取&#x200B;**`{{lead.Lead Owner First Name}}`**&#x200B;權杖。

   ![](assets/personalize-an-email-4.png)

1. 輸入您的公司名稱和&#x200B;**預設值**&#x200B;的破折號，以確保在銷售代表的名字無法使用時會顯示某些內容。 按一下&#x200B;**插入**。

   ![](assets/personalize-an-email-5.png)

1. 按一下&#x200B;**[!UICONTROL 從]**&#x200B;欄位中的空格列，確定游標在您剛插入的Token後閃爍一個空格。 然後再次按一下&#x200B;**Token**&#x200B;圖示。

   ![](assets/personalize-an-email-6.png)

1. 尋找並選取&#x200B;**`{{lead.Lead Owner Last Name}}`**&#x200B;權杖。

   ![](assets/personalize-an-email-7.png)

1. 輸入&#x200B;**預設值**&#x200B;的[銷售]並按一下&#x200B;**插入**。

   ![](assets/personalize-an-email-8.png)

## 步驟3：將潛在客戶名稱新增至電子郵件 {#step-add-the-leads-name-to-the-email}

1. 選取頂端可編輯的區段，按一下齒輪圖示並選取&#x200B;**[!UICONTROL 編輯]**。

   ![](assets/personalize-an-email-9.png)

1. 在「Hello」後面加上空格，並將游標放在逗號前面，然後按一下&#x200B;**插入Token**&#x200B;圖示。

   ![](assets/personalize-an-email-10.png)

1. 尋找並選取&#x200B;**`{{lead.First Name}}`**&#x200B;權杖。

   ![](assets/personalize-an-email-11.png)

1. 在&#x200B;**[!UICONTROL 預設值]**&#x200B;欄位中輸入「朋友」（或您想要的任何標籤），然後按一下&#x200B;**[!UICONTROL 插入]**。

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >一律包含代號的預設值；這可確保在缺少部分個人資訊時，電子郵件中會顯示預設值。

1. 按一下&#x200B;**[!UICONTROL 保存]**。

   ![](assets/personalize-an-email-13.png)

1. 在「**[!UICONTROL 電子郵件動作]**」下，選取「**[!UICONTROL 核准並關閉]**」。

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>需要快速重新整理一下如何傳送電子郵件給您自己？ 請參閱[傳送電子郵件爆炸訊息](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}。

### 任務完成 {#mission-complete}

恭喜，您已個人化您的電子郵件！

<br> 

[◄任務6：滴水、滴水、Nurture](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任務8：通知銷售代表►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
