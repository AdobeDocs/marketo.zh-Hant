---
unique-page-id: 1900597
description: 匯入清單——行銷人員檔案——產品檔案以定義觀眾
title: 匯入清單以定義對象
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---


# 匯入清單{#define-an-audience-by-importing-a-list}以定義對象

>[!PREREQUISITES]
>
>[建立電子郵件方案的電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

一旦您建立了電子郵件程式，您就會想告訴它要將電子郵件傳送給誰。 您可以通過[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)或通過導入清單來執行此操作。 以下說明如何匯入清單以達成此目的。

>[!NOTE]
>
>只有在未核准電子郵件方案時，才能定義您的觀眾。
>
>匯入的任何日期／時間欄位都會視為「中央時間」。 如果您在不同時區有日期／時間欄位，則可使用Excel公式將其轉換為中時（美國／芝加哥）。

1. 前往&#x200B;**行銷活動**。

   ![](assets/login-marketing-activities-1.png)

1. 選取您的電子郵件程式，然後按一下「對象」方塊下的「匯入清單」。

   ![](assets/importlist.png)

1. 清單導入窗口開啟，按一下&#x200B;**瀏覽**&#x200B;並選擇要導入的檔案。 選擇人員清單後，按一下&#x200B;**Next**。

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >請確定清單是已編碼的UTF-8、UTF-16、Shift-JIS或EUC-JP，且檔案大小不超過50MB。

1. 驗證檔案中的欄位已正確映射，然後按一下&#x200B;**Next**。

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo將記住未來進口的映射！

1. 為清單輸入&#x200B;**名稱** ，然後按一下&#x200B;**導入**。

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. 完成導入後，返回主程式頁籤。 您將瞭解有多少人符合資格。

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**定義**
>
>您注意到Blocked號碼了嗎？ 此數字是合格人員的子集，代表無法傳送此電子郵件的人員，因為他們：
>
>* 取消訂閱
>* 暫停行銷
>* 封鎖清單
>* 電子郵件無效
>* 空電子郵件

>
>
按一下號碼，以取得封鎖郵件的詳細清單。
>
>使用&#x200B;**觀眾**&#x200B;方塊上的![—](assets/image2014-10-23-16-3a32-3a36-1.png)按鈕，查看有多少人符合智慧型清單准則接收電子郵件的資格。 從「人員」號碼中減去「已封鎖」號碼，即可獲得接收電子郵件的總人數。

>[!TIP]
>
>您不必等待清單匯入完成。 如果你願意，你可以繼續工作。

太棒了！ 現在，您應該選擇已有的電子郵件，或建立新的電子郵件，以傳送給這些人。

>[!MORELIKETHIS]
>
>* [選擇現有電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [建立電子郵件方案的電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

