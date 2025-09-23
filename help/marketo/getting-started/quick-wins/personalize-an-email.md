---
unique-page-id: 2359422
description: 電子郵件個人化 - Marketo 文件 - 產品文件
title: 電子郵件個人化
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 100%

---

# 電子郵件個人化 {#personalize-an-email}

## 任務：新增資料權杖，製作個人化的電子郵件 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [完成設定與新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [傳送群發電子郵件](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [點滴式培養](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## 步驟 1：選取要進行個人化的電子郵件 {#step-select-an-email-to-personalize}

1. 選取在[前一項快速成果](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}中建立的其中一封培養電子郵件，然後按一下「**[!UICONTROL Create draft]**」。

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >此動作會以草稿形式建立一封電子郵件副本。請記得核准草稿讓變更生效。

在未啟用快顯視窗封鎖程式的情況下，電子郵件編輯器會在新的索引標籤/視窗中開啟。若未開啟，請按一下「**[!UICONTROL Create Draft]**」兩次。

## 步驟 2：讓銷售人員成為寄件者 {#step-make-the-salesperson-the-sender}

1. 選取「**[!UICONTROL From]**」欄位，反白標示目前的名稱，然後將其&#x200B;**刪除**。

   ![](assets/personalize-an-email-2.png)

1. 按一下「**[!UICONTROL From]**」欄位右側的「**權杖**」圖示。

   ![](assets/personalize-an-email-3.png)

1. 找到並選取「**`{{lead.Lead Owner First Name}}`**」權杖。

   ![](assets/personalize-an-email-4.png)

1. 於「**預設值**」欄位輸入您的公司名稱並加上一個破折號 (-)，確保當銷售代表的名字無法使用時仍能顯示某些內容。按一下「**插入**」。

   ![](assets/personalize-an-email-5.png)

1. 在「**[!UICONTROL From]**」欄位中按下空白鍵，確認在您剛插入的權杖後面一個空格處，有游標正在閃爍。然後再次按一下「**權杖**」圖示。

   ![](assets/personalize-an-email-6.png)

1. 找到並選取「**`{{lead.Lead Owner Last Name}}`**」權杖。

   ![](assets/personalize-an-email-7.png)

1. 於「**預設值**」欄位輸入「銷售」，然後按一下「**插入**」。

   ![](assets/personalize-an-email-8.png)

## 步驟 3：將商機的名稱新增至電子郵件中 {#step-add-the-leads-name-to-the-email}

1. 選取頂部可編輯的區段，按一下齒輪圖示並選取「**[!UICONTROL Edit]**」。

   ![](assets/personalize-an-email-9.png)

1. 在「Hello」後面加入一個空格，將游標放在逗號前面，然後按一下「**插入權杖**」圖示。

   ![](assets/personalize-an-email-10.png)

1. 找到並選取「**`{{lead.First Name}}`**」權杖。

   ![](assets/personalize-an-email-11.png)

1. 在「**[!UICONTROL Default Value]**」欄位中輸入「朋友」(或任何您想要的標籤)，然後按一下「**[!UICONTROL Insert]**」。

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >權杖務必要包含一個預設值；若遇到缺少部分個人資訊的情況，可確保電子郵件中會顯示預設值。

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/personalize-an-email-13.png)

1. 在「**[!UICONTROL Email Actions]**」之下然後選取「**[!UICONTROL Approve and Close]**」。

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>需要快速複習如何傳送電子郵件給自己嗎？請參閱[傳送群發電子郵件](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}。

### 任務完成 {#mission-complete}

恭喜，您已製作出個人化的電子郵件！

<br>

[◄ 任務 6：點滴式培養](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任務 8：通知銷售代表 ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
