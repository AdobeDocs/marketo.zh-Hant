---
unique-page-id: 2359746
description: 使用CNAME自訂著陸頁面URL —— 行銷人員檔案——產品檔案
title: 使用CNAME自訂著陸頁面URL
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# 使用CNAME {#customize-your-landing-page-urls-with-a-cname}自訂著陸頁面URL

即使Marketo代管您的著陸頁面，URL仍可完全自訂。 沒有CNAME的情況：
`<pre data-theme="Confluence">http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html</pre>`其外觀：
`<pre data-theme="Confluence"> http://go.YourCompany.com/UnsubscribePage.html</pre>`

## 選擇CNAME {#choose-a-cname}

選擇要移至著陸頁面URL開頭的字詞。 它只是一個詞，應該比較短。 範例：

* 走。 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* 資訊。 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* 頁面。 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)

單字（加上[YourCompany.com](http://YourCompany.com)）稱為CNAME。 您稍後需要這個，請記下。

## 尋找您的帳戶字串{#find-your-account-string}

1. 前往&#x200B;**Admin**&#x200B;區域，然後按一下&#x200B;**著陸頁面。**

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**需要管理員權限**

1. 在&#x200B;**Landing****Pages**&#x200B;標籤下，從&#x200B;**Settings**&#x200B;區複製&#x200B;**Account****String**。

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. 您稍後也需要，請記下。

## 向IT {#send-request-to-it}發送請求

請您的IT人員設定下列CNAME:（將字詞[CNAME]和[ACCOUNT STRING]取代為上一步驟的文字）。

[CNAME]。[YourCompany.com](http://yourcompany.com/) >帳 [戶字串]。[mktoweb.com](http://mktoweb.com/)

## 完成CNAME設定{#complete-cname-setup}

1. 在您的IT建立CNAME後，請前往&#x200B;**Admin**，然後按一下&#x200B;**Landing** **Pages**。

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. 在&#x200B;**Settings**&#x200B;區段下，按一下&#x200B;**Edit**。

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. 在&#x200B;**域****名稱** **中為** **著陸** **頁面**&#x200B;輸入您的&#x200B;**備援** **頁面&lt;a113/>，輸入您的** Homepage **，然後按一下「儲存」**「a17/」。****

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>如果您的行銷人員著陸頁面無法使用，您的後援頁面將是頁面銷售機會，會被重新導向至。

幹得好！ 您的登陸頁面現在會與您的公司網域一起加上品牌。