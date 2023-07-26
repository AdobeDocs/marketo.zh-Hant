---
unique-page-id: 1900597
description: 透過匯入清單來定義對象 — Marketo檔案 — 產品檔案
title: 透過匯入清單來定義對象
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# 透過匯入清單來定義對象 {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[為電子郵件計畫建立電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

建立電子郵件程式後，您會想要告訴程式要將電子郵件傳送給誰。 您可以透過以下方式達成此目的 [建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 或匯入清單。 以下說明如何匯入清單來達到此目的。

>[!NOTE]
>
>只有當電子郵件計畫未獲核準時，定義您的對象才能運作。
>
>匯入的任何日期/時間欄位都會視為中央時間。 如果您的日期/時間欄位位於不同的時區，可以使用Excel公式將其轉換為中部時間（美洲/芝加哥）。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-1.png)

1. 選取您的電子郵件程式，然後按一下「對象」方塊下的「匯入清單」 。

   ![](assets/importlist.png)

1. 清單匯入視窗隨即開啟，按一下 **瀏覽** 並選取您要匯入的檔案。 選取人員清單後，按一下 **下一個**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >請確定此清單編碼為UTF-8、UTF-16、Shift-JIS或EUC-JP，且檔案大小不超過50MB。

1. 確認檔案中的欄位已正確對應，然後按一下 **下一個**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo將會記住未來匯入的對應！

1. 輸入 **名稱** ，然後按一下 **匯入**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. 匯入完成後，請返回主計畫標籤。 您將看到有多少人符合資格。

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**定義**
>
>您注意到封鎖的號碼嗎？ 此數字是合格人員的子集，代表因下列原因而無法傳送此電子郵件的人員：
>
>* 退訂
>* 行銷活動已暫停
>* 已加入封鎖清單
>* 電子郵件無效
>* 空白電子郵件
>
>按一下數字，即可取得封鎖郵件之人員的詳細清單。
>
>使用 ![—](assets/image2014-10-23-16-3a32-3a36-1.png) 上的按鈕 **對象** 圖磚，用來根據智慧清單條件檢視有多少人符合接收電子郵件的資格。 從「人物」號碼中減去「已封鎖」號碼，即可取得將收到電子郵件的人物總數。

>[!TIP]
>
>您不必等待清單匯入完成。 您可以視需要繼續工作。

太棒了！ 現在該選擇現有電子郵件或建立新電子郵件以傳送給這些人員了。

>[!MORELIKETHIS]
>
>* [選擇現有電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [為電子郵件計畫建立電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
