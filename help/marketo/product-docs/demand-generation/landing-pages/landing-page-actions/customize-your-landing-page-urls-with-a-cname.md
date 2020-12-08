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


# 使用CNAME自訂著陸頁面URL {#customize-your-landing-page-urls-with-a-cname}

即使Marketo代管您的著陸頁面，URL仍可完全自訂。 沒有CNAME的情況：`<pre data-theme="Confluence">http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html</pre>` 它的外觀：
`<pre data-theme="Confluence"> http://go.YourCompany.com/UnsubscribePage.html</pre>`

## 選擇CNAME {#choose-a-cname}

選擇要移至著陸頁面URL開頭的字詞。 它只是一個詞，應該比較短。 範例：

* 走。 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* 資訊。 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* 頁面。 [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)

單字(加上 [YourCompany.com](http://YourCompany.com))稱為CNAME。 您稍後需要這個，請記下。

## 尋找您的帳戶字串 {#find-your-account-string}

1. 前往「管 **理** 」區域，然後按一 **下「著陸頁面」。**

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**需要管理員權限**

1. 在「著陸頁 **面****」頁籤下** ，複製Account **String Settings** from the Landing Pages（從著陸頁面）設定中複製Account ******** String Settings（帳戶字串）部分。

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. 您稍後也需要，請記下。

## 傳送要求給IT人員 {#send-request-to-it}

請您的IT人員設定下列CNAME:(將單字 [CNAME][] 和ACCOUNT STRING取代為上一步驟的文字。)

[CNAME]。 [YourCompany.com](http://yourcompany.com/) >帳 [戶字串]。 [mktoweb.com](http://mktoweb.com/)

## 完成CNAME設定 {#complete-cname-setup}

1. IT人員建立CNAME後，請前往「管 **理員** 」並按一下「 **著陸****頁面」**。

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. 在「設 **定** 」區段下，按一 **下編輯**。

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. 在域名中為 **Landing Landing** Save **AldingPages的Domain** name, Enter Your AldingPage，輸入您的NAME，在Domain **************************** name中輸入您的NAME。

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>如果您的行銷人員著陸頁面無法使用，您的後援頁面將是頁面銷售機會，會被重新導向至。

幹得好！ 您的登陸頁面現在會與您的公司網域一起加上品牌。