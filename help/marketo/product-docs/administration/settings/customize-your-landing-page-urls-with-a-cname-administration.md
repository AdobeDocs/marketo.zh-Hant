---
unique-page-id: 2360189
description: 使用CNAME（管理）自訂著陸頁面URL -Marketo檔案——產品檔案
title: 使用CNAME（管理）自訂著陸頁面URL
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 使用CNAME（管理）{#customize-your-landing-page-urls-with-a-cname-administration}自訂著陸頁面URL

即使Marketo代管著陸頁面，URL仍應為您的公司自訂。

>[!NOTE]
>
>無CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>品牌化CNAME:
>
>https://go。**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**需要管理員權限**

讓我們幫你安排！

1. 選擇CNAME。

   它是URL的前部。 範例：

   * **前往**.YourCompany.com/NameOfPage.html
   * **資訊**.YourCompany.com/NameOfPage.html
   * **頁面**.YourCompany.com/NameOfPage.html

   這個單字（加上YourCompany.com）稱為CNAME。 您稍後需要這個，請記下。

1. 尋找您的帳戶字串。

1. 前往&#x200B;**Admin**&#x200B;區域，然後按一下&#x200B;**Landing Pages**。

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. 在&#x200B;**著陸頁面**&#x200B;標籤下，從「設定」區段複製帳戶字串。

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. 您稍後也需要這個，請記下。

1. 傳送要求給IT人員。

1. 請您的IT人員設定下列CNAME（以上步驟的文字取代字詞[CNAME]和[ACCOUNT STRING]）:

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

1. 完成CNAME設定。

1. 在您的IT建立CNAME後，請前往&#x200B;**Admin**，然後按一下&#x200B;**著陸頁面**。

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. 在&#x200B;**Settings**&#x200B;區段下，按一下&#x200B;**Edit**。

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. 在「著陸頁面&#x200B;**網域名稱」中輸入您的CNAME，輸入**&#x200B;後援頁面&#x200B;**，輸入**&#x200B;首頁&#x200B;**，然後按一下**&#x200B;儲存&#x200B;**。**

   ![](assets/image2014-9-16-13-3a10-3a45.png)

如果您的Marketo登陸頁面無法使用，您的後援頁面會重新導向訪客。

幹得好！ 您的登陸頁面現在會與您的公司網域一起加上品牌。
