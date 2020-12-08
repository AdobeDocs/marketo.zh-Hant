---
unique-page-id: 1900597
description: 匯入清單——行銷人員檔案——產品檔案以定義觀眾
title: 匯入清單以定義對象
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---


# 匯入清單以定義對象 {#define-an-audience-by-importing-a-list}

>[!NOTE]
>
>**必要條件**
>
>[建立電子郵件方案的電子郵件](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

一旦您建立了電子郵件程式，您就會想告訴它要將電子郵件傳送給誰。 您可以建立智慧型 [清單](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) ，或匯入清單來執行此動作。 以下說明如何匯入清單以達成此目的。

>[!NOTE]
>
>只有在未核准電子郵件方案時，才能定義您的觀眾。
>
>匯入的任何日期／時間欄位都會視為「中央時間」。 如果您在不同時區有日期／時間欄位，則可使用Excel公式將其轉換為中時（美國／芝加哥）。

1. 前往行 **銷活動**。

   ![](assets/login-marketing-activities-1.png)

   選取您的電子郵件程式，然後按一下「對象」方塊下的「匯入清單」。
   ![](assets/importlist.png)

1. 清單導入窗口開啟，按一下「瀏 **覽** 」(Browse)，然後選擇要導入的檔案。 在您選取人員清單後，按一下「下一步」。
1. ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >請確定清單是已編碼的UTF-8、UTF-16、Shift-JIS或EUC-JP，且檔案大小不超過50MB。

   確認您檔案中的欄位已正確映射，然後按一下「下一步」。
   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo將記住未來進口的映射！

1. 輸入列 **表的名稱** ，然後按一下 **導入**。

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
>使用「對 ![像」方塊](assets/image2014-10-23-16-3a32-3a36-1.png) 上的「-按鈕 **** 」，查看有多少人符合資格根據智慧清單條件接收電子郵件。 從「人員」號碼中減去「已封鎖」號碼，即可獲得接收電子郵件的總人數。

>[!TIP]
>
>您不必等待清單匯入完成。 如果你願意，你可以繼續工作。

太棒了！ 現在，您應該選擇已有的電子郵件，或建立新的電子郵件，以傳送給這些人。

>[!NOTE]
>
>**相關文章**
>
>* [選擇現有電子郵件](../../../../product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [建立電子郵件方案的電子郵件](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

>



