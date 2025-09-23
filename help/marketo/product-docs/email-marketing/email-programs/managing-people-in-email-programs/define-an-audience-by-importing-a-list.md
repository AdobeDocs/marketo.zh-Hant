---
unique-page-id: 1900597
description: 透過匯入清單來定義對象 — Marketo檔案 — 產品檔案
title: 透過匯入清單定義客群
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 15%

---

# 透過匯入清單定義客群 {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[為電子郵件程式建立電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

建立電子郵件程式後，您會想要告訴程式要將電子郵件傳送給誰。 您可以透過[建立智慧列示](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)或匯入清單來執行此操作。 以下說明如何匯入清單來達到此目的。

>[!NOTE]
>
>只有當電子郵件計畫未獲核準時，定義您的對象才能運作。
>
>所匯入的任何日期/時間欄位均被視為北美中部時間。若您有位在不同時區的日期/時間欄位，可以使用 Excel 公式將其轉換為北美中部時間 (美國/芝加哥)。

1. 移至&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/login-marketing-activities-1.png)

1. 選取您的電子郵件程式，然後按一下「**[!UICONTROL Import List]**」方塊下方的「**[!UICONTROL Audience]**」。

   ![](assets/importlist.png)

1. 清單匯入視窗開啟，按一下&#x200B;**[!UICONTROL Browse]**&#x200B;並選取您要匯入的檔案。 選取您的人員清單後，按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >請確定此清單編碼為UTF-8、UTF-16、Shift-JIS或EUC-JP，且檔案大小不超過50MB。

1. 確認檔案中的欄位已正確對應，然後按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo將會記住未來匯入的對應！

1. 輸入清單的&#x200B;**[!UICONTROL Name]**&#x200B;並按一下&#x200B;**[!UICONTROL Import]**。

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. 匯入完成後，請返回主計畫標籤。 您將看到有多少人符合資格。

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**定義**
>
>您注意到封鎖的號碼嗎？ 此數字是合格人員的子集，代表因下列原因而無法傳送此電子郵件的人員：
>
>* 已取消訂閱
>* 行銷活動暫停
>* 已加入封鎖清單
>* 電子郵件無效
>* 空白電子郵件
>
>按一下數字，即可取得封鎖郵件之人員的詳細清單。
>
>使用![圖磚上的](assets/image2014-10-23-16-3a32-3a36-1.png)—**[!UICONTROL Audience]**&#x200B;按鈕，根據智慧清單條件檢視有多少人符合接收電子郵件的資格。 從「人物」號碼中減去「已封鎖」號碼，即可取得將收到電子郵件的人物總數。

>[!TIP]
>
>您不必等待清單匯入完成。 您可以視需要繼續工作。

太棒了！ 現在該選擇現有電子郵件或建立新電子郵件以傳送給這些人員了。

>[!MORELIKETHIS]
>
>* [選擇現有的電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [為電子郵件程式建立電子郵件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
