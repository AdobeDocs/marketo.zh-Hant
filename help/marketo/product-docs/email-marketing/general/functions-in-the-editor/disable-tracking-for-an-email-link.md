---
unique-page-id: 1900579
description: 停用電子郵件連結的追蹤——行銷檔案——產品檔案
title: 停用電子郵件連結的追蹤
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---


# 停用電子郵件連結的追蹤 {#disable-tracking-for-an-email-link}

有時您不想在電子郵件中的連 **結上啟用** 「行銷人員追蹤URL」。 當目標頁面不支援URL參數且可能導致連結中斷時，這個功能會很有用。

>[!NOTE]
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](/help/marketo/getting-started/updates-to-marketo-terminology.md)。

1. 選擇您的電子郵件，然後按一 **下「編輯****草稿**」。

   ![](assets/one-7.png)

1. 連按兩下包含連結的可編輯區段。

   ![](assets/two-6.png)

1. 按一下相關連結，然後按一下「插入/ **編輯連結」按鈕** 。

   ![](assets/three-6.png)

1. 在「編輯連結」快顯視窗中，取消勾選「追 **蹤連結** 」核取方塊。

   ![](assets/four-4.png)

1. 您會注意到「包 **含mkt_tok」方塊消失** 。 按一 **下套用**。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >只取消 **勾選「包含mkt_tok** 」仍允許追蹤連結，但在重新導向後，目標URL將不包含mkt_tok查詢字串參數。 Marketo Landing Pages和Munchkin會使用此參數，以確保正確追蹤人員活動（例如當人員取消訂閱電子郵件時）。 您應避免使用此功能，除非您看到網站上因為參數存在而出現奇怪的行為。

1. 按一下 **儲存**。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >想要停用電子郵件範本中連結的點按追 **蹤**? 使用下列格式：
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >如果您需要實作此內容的協助，請洽詢您的網頁開發人員。

不錯！ 您現在已停用連結的追蹤。
