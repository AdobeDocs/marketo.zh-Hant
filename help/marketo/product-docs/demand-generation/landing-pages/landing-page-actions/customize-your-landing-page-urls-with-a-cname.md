---
unique-page-id: 2359746
description: 使用CNAME自訂您的登陸頁面URL - Marketo檔案 — 產品檔案
title: 使用 CNAME 自訂您的登陸頁面 URL
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 7%

---

# 使用 CNAME 自訂您的登陸頁面 URL {#customize-your-landing-page-urls-with-a-cname}

即使Marketo代管您的登陸頁面，您也可以完全自訂URL。 在沒有CNAME時的外觀：

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

外觀：

`https://go.YourCompany.com/UnsubscribePage.html`

## 選擇CNAME {#choose-a-cname}

從登陸頁面URL的開頭選取要前往的單字。 只是一個字，應該相對較短。 範例：

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

一個字(加上YourCompany.com)稱為CNAME。 您稍後需要此資訊，請記下資訊。

## 尋找您的Munchkin ID {#find-your-munchkin-id}

1. 移至&#x200B;**管理員**&#x200B;區域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 按一下&#x200B;**我的帳戶**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**需要管理員許可權**

1. 向下捲動至「支援資訊」並複製您的Munchkin ID。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## 傳送要求給IT {#send-request-to-it}

請您的IT人員設定下列CNAME： (將單字[CNAME]和[Munchkin ID]取代為上一步驟的文字。)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## 完成CNAME設定 {#complete-cname-setup}

1. 在您的IT建立CNAME後，請移至&#x200B;**管理員**&#x200B;區域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 按一下&#x200B;**登陸頁面**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在&#x200B;**設定**&#x200B;區段下，按一下&#x200B;**編輯**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 在&#x200B;**[!UICONTROL Domain name for Landing Pages]**&#x200B;中輸入您的CNAME、輸入您的&#x200B;**[!UICONTROL Fallback page]**、輸入您的&#x200B;**[!UICONTROL Homepage]**&#x200B;並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>如果您的Marketo登陸頁面無法使用，您的後援頁面將會是重新導向到的頁面銷售機會。

做得好！ 您的登入頁面現在以公司網域命名。
