---
unique-page-id: 1900579
description: 停用電子郵件連結的追蹤 — Marketo檔案 — 產品檔案
title: 停用電子郵件連結的追蹤
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# 停用電子郵件連結的追蹤 {#disable-tracking-for-an-email-link}

有時您並不想在電子郵件中的連結上啟用&#x200B;**Marketo追蹤URL**。 當目的地頁面不支援URL引數並且可能導致連結中斷時，這項功能會很有用。

1. 選取您的電子郵件並按一下&#x200B;**編輯草稿**。

   ![](assets/one-7.png)

1. 連按兩下包含連結的可編輯區段。

   ![](assets/two-6.png)

1. 按一下有問題的連結，然後按一下&#x200B;**插入/編輯連結**&#x200B;按鈕。

   ![](assets/three-6.png)

1. 在「編輯連結」快顯視窗中，取消勾選&#x200B;**追蹤連結**&#x200B;核取方塊。

   ![](assets/four-4.png)

1. 您會注意到&#x200B;**包含mkt_tok方塊**&#x200B;已消失。 按一下&#x200B;**套用**。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >取消僅核取&#x200B;**包含mkt_tok**&#x200B;仍可追蹤連結，但在重新導向後，目的地URL將不會包含mkt_tok查詢字串引數。 Marketo登陸頁面和Munchkin會使用此引數，以確保正確追蹤人員活動（例如當人員取消訂閱電子郵件時）。 您應該避免使用此功能，除非您因引數出現而在網站上看到奇怪的行為。

1. 按一下&#x200B;**保存**。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >想要停用電子郵件&#x200B;**範本**中連結的點選追蹤？ 使用此格式：
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >若您需要實作此專案的協助，請洽詢您的網頁開發人員。

很好！ 您現在已停用連結的追蹤。
