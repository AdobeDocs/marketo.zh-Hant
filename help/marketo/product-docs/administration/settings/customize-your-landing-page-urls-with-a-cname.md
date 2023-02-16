---
unique-page-id: 2360189
description: 使用CNAME（管理）自訂您的登錄頁面URL - Marketo檔案 — 產品檔案
title: 使用CNAME（管理）自訂您的登錄頁面URL
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 使用CNAME自訂您的登錄頁面URL  {#customize-your-landing-page-urls-with-a-cname}

即使Marketo托管您的登錄頁面，您也應根據公司自訂URL。

>[!NOTE]
>
>無CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>品牌CNAME:
>
>https://go。**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**需要管理權限**

讓我們幫你安排！

1. 選擇CNAME。

   這是URL的前部。 範例:

   * **go**.YourCompany.com/NameOfPage.html
   * **資訊**.YourCompany.com/NameOfPage.html
   * **頁面**.YourCompany.com/NameOfPage.html

   一個詞（加上YourCompany.com）稱為CNAME。 您稍後將需要此項，請記下。

1. 尋找您的帳戶字串。

1. 前往 **管理** 的上界。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 按一下 **登錄頁面**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. 在 **登錄頁面** 標籤，從「設定」區段複製「帳戶字串」。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. 您稍後也需要這個，請記下來。

1. 向IT發送請求。

1. 請您的IT人員設定下列CNAME(取代 [CNAME] 和 [帳戶字串] 與上一步的文字):

   [CNAME].YourCompany.com > [帳戶字串].mktoweb.com

1. 完成CNAME設定。

1. IT人員建立CNAME後，請返回 **管理** 的上界。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 按一下 **登錄頁面**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在 **設定** ，按一下 **編輯**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在 **登錄頁面的網域名稱**，請輸入 **後援頁面**，請輸入 **首頁**，然後按一下 **儲存**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

如果您的Marketo登錄頁面無法使用，系統會將人員重新導向您的後援頁面。

幹得好！ 您的登錄頁面現在已與您的公司網域加上品牌。
