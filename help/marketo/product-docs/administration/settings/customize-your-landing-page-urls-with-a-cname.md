---
unique-page-id: 2360189
description: 使用CNAME （管理）自訂您的登陸頁面URL - Marketo檔案 — 產品檔案
title: 使用CNAME （管理）自訂您的登陸頁面URL
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 使用CNAME自訂您的登陸頁面URL  {#customize-your-landing-page-urls-with-a-cname}

即使Marketo代管您的登陸頁面，也應針對您的公司自訂URL。

>[!NOTE]
>
>無CNAME：
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>品牌CNAME：
>
>https://go.**您的公司**.com/UnsuscribePage.html

>[!NOTE]
>
>**需要管理員許可權**

讓我們設定您！

1. 選擇CNAME。

   這是URL的前端。 範例:

   * **執行**.YourCompany.com/NameOfPage.html
   * **資訊**.YourCompany.com/NameOfPage.html
   * **頁面**.YourCompany.com/NameOfPage.html

   一個字(加上YourCompany.com)稱為CNAME。 您稍後將需要此資訊，請記下該資訊。

1. 尋找您的帳戶字串。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 按一下 **[!UICONTROL 登陸頁面]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. 在 **[!UICONTROL 登陸頁面]** 索引標籤中，從設定區段複製帳戶字串。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. 您稍後也會需要此專案，請記下它。

1. 傳送要求給IT。

1. 請您的IT人員設定下列CNAME (取代文字 [CNAME] 和 [帳戶字串] 使用上一步驟的文字)：

   [CNAME].YourCompany.com > [帳戶字串].mktoweb.com

1. 完成CNAME設定。

1. 在您的IT建立CNAME後，請返回 **[!UICONTROL 管理員]** 區域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 按一下 **[!UICONTROL 登陸頁面]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在 **[!UICONTROL 設定]** 區段，按一下 **[!UICONTROL 編輯]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在中輸入您的CNAME **[!UICONTROL 登陸頁面的網域名稱]**，輸入您的 **[!UICONTROL 備援頁面]**，輸入您的 **[!UICONTROL 首頁]**，然後按一下 **[!UICONTROL 儲存]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

如果您的Marketo登陸頁面無法使用，備援頁面會將使用者重新導向。

做得好！ 您的登入頁面現在以公司網域命名。
