---
unique-page-id: 11382535
description: 在My Token中使用URL - Marketo檔案 — 產品檔案
title: 在我的權杖中使用 URL
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# 在我的權杖中使用 URL {#using-urls-in-my-tokens}

請依照下列步驟，使用[!UICONTROL My Tokens]將URL插入您的電子郵件中。

1. 選取您的程式並按一下&#x200B;**[!UICONTROL My Tokens]**。

   ![](assets/one-4.png)

1. 選取「**[!UICONTROL Text]**&#x200B;我的Token」，將其拖放到畫布上。

   ![](assets/two-4.png)

1. 為權杖指定唯一的名稱，輸入URL (不含https://)並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**使用http/https...**
   >
   >* 若要確定在您的電子郵件中追蹤點按，請&#x200B;**不**&#x200B;輸入https:// _在裡面_&#x200B;權杖的值。 在Token之外使用它，如步驟7所示。
   >
   >* 強烈建議您不要遺漏http/https。 這麼做可能會造成您電子郵件的[網頁版本](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}無法正確呈現。

1. 在您的程式中選取電子郵件。

   ![](assets/four-3.png)

1. 按一下「**[!UICONTROL Edit Draft]**」。

   ![](assets/five-3.png)

1. 在文字區域中連按兩下以編輯。

   ![](assets/six-1.png)

1. 在電子郵件中的任一處，輸入`https://` （後面不留空格），然後按一下「插入Token」圖示。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >如果您的網站未使用https，您當然也可以選擇輸入`http://`。

1. 找到您的「我的Token」，選取並按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/eight.png)

1. 反白顯示https://和Token，然後按Ctrl/Cmd+X (Ctrl = Windows/Cmd = Mac)以剪下文字。

   ![](assets/nine.png)

1. 反白您要顯示連結的文字，然後按一下[!UICONTROL Insert/Edit Link]圖示。

   ![](assets/ten.png)

1. 按Ctrl/Cmd+V將內容貼到&#x200B;**[!UICONTROL URL]**&#x200B;方塊中，然後按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/eleven.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/twelve.png)

   而您已完成！ 您的URL將在傳送後填入，由於您將https://放在權杖前，它會產生可追蹤連結。
