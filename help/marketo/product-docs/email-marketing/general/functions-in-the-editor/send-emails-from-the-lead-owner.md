---
unique-page-id: 1147340
description: 傳送潛在客戶擁有者的電子郵件 — Marketo檔案 — 產品檔案
title: 從潛在客戶擁有者傳送電子郵件
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# 從潛在客戶擁有者傳送電子郵件 {#send-emails-from-the-lead-owner}

如果您要代表潛在客戶擁有者傳送電子郵件給潛在客戶，該怎麼做？  方法如下。

1. 尋找您的電子郵件，選取並按一下 **編輯草稿**.

   ![](assets/one.png)

1. 按一下 **從** 欄位（刪除任何現有名稱），然後按一下 **插入權杖** 按鈕。

   ![](assets/two.png)

1. 開始輸入&quot;`{{lead.Lead Owner`」並選取 **`{{lead.Lead Owner First Name}}`** Token。

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. 輸入預設值，以防止潛在客戶尚未擁有潛在客戶擁有者，然後按一下 **插入**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. 在第一個Token之後按一下，新增空格，然後按一下 **插入權杖** 按鈕。

   ![](assets/five.png)

1. 開始輸入&quot;`{{lead.Lead Owner`」並選取 **`{{lead.Lead Owner Last Name}}`** Token。

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. 輸入預設值，以防止潛在客戶尚未擁有潛在客戶擁有者，然後按一下 **插入**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >請務必在名字和姓氏代號之間新增空格。

1. 按一下「寄件者電子郵件」欄位（刪除任何現有的電子郵件地址），然後按一下「插入Token」按鈕。

   ![](assets/eight.png)

1. 開始輸入&quot;`{{lead.Lead Owner`」並選取 **`{{lead.Lead Owner Email Address}}`** Token。

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. 輸入預設值，以防止潛在客戶尚未擁有潛在客戶擁有者，然後按一下 **插入**.

   ![](assets/ten.png)

1. 確定 **回覆** 和 **主旨** 欄位已填入，您已完成！

   ![](assets/eleven.png)
