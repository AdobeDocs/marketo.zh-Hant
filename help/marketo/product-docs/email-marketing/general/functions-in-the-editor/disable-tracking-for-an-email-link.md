---
unique-page-id: 1900579
description: 停用電子郵件連結的追蹤 — Marketo檔案 — 產品檔案
title: 停用電子郵件連結的追蹤
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# 停用電子郵件連結的追蹤 {#disable-tracking-for-an-email-link}

有時您不想啟用 **Marketo追蹤URL** 在電子郵件的連結上。 當目的地頁面不支援URL參數且可能導致連結中斷時，這個用法就很實用。

1. 選取您的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/one-7.png)

1. 連按兩下包含連結的可編輯區段。

   ![](assets/two-6.png)

1. 按一下相關連結，然後按一下 **插入/編輯連結** 按鈕。

   ![](assets/three-6.png)

1. 在「編輯連結」快顯視窗中，取消勾選 **追蹤連結** 核取方塊。

   ![](assets/four-4.png)

1. 你會注意到 **包括mkt_tok盒** 消失了。 按一下 **套用**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >取消檢查 **包括mkt_tok** 仍會允許追蹤連結，但在重新導向後，目的地URL將不包含mkt_tok查詢字串參數。 此參數供Marketo登陸頁面和Munchkin使用，以確保正確追蹤人員活動（例如當人員取消訂閱電子郵件時）。 除非您因參數存在而在網站上看到異常行為，否則應避免使用此功能。

1. 按一下 **儲存**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >想要停用電子郵件中連結的點擊追蹤 **範本**? 使用此格式：
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >若您需要實作此功能的協助，請洽詢您的網頁開發人員。

不錯！ 您現在已停用連結的追蹤。
