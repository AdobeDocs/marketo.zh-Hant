---
unique-page-id: 1147340
description: 傳送潛在客戶擁有者的電子郵件 — Marketo檔案 — 產品檔案
title: 傳送來自商機所有者的電子郵件
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 7%

---

# 傳送來自商機所有者的電子郵件 {#send-emails-from-the-lead-owner}

如果您要代表潛在客戶擁有者傳送電子郵件給潛在客戶，該怎麼做？  方法如下。

1. 尋找您的電子郵件，選取並按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/one.png)

1. 按一下&#x200B;**[!UICONTROL From]**&#x200B;欄位（刪除任何現有的名稱），然後按一下&#x200B;**插入Token**&#x200B;按鈕。

   ![](assets/two.png)

1. 開始輸入&quot;`{{lead.Lead Owner`&quot;並選取&#x200B;**`{{lead.Lead Owner First Name}}`**&#x200B;權杖。

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. 輸入預設值，以防止潛在客戶尚未擁有潛在客戶擁有者，然後按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. 在第一個權杖之後按一下，新增空格，然後按一下&#x200B;**插入權杖**&#x200B;按鈕。

   ![](assets/five.png)

1. 開始輸入&quot;`{{lead.Lead Owner`&quot;並選取&#x200B;**`{{lead.Lead Owner Last Name}}`**&#x200B;權杖。

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. 輸入預設值，以防止潛在客戶尚未擁有潛在客戶擁有者，然後按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >請務必在名字和姓氏代號之間新增空格。

1. 按一下&#x200B;**[!UICONTROL From Address]**&#x200B;欄位（刪除任何現有的電子郵件地址），然後按一下&#x200B;**插入權杖**&#x200B;按鈕。

   ![](assets/eight.png)

1. 開始輸入&quot;`{{lead.Lead Owner`&quot;並選取&#x200B;**`{{lead.Lead Owner Email Address}}`**&#x200B;權杖。

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. 輸入預設值，以防止潛在客戶尚未擁有潛在客戶擁有者，然後按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/ten.png)

1. 確定已填入&#x200B;**[!UICONTROL Reply-to]**&#x200B;和&#x200B;**[!UICONTROL Subject]**&#x200B;欄位，且您已完成！

   ![](assets/eleven.png)
