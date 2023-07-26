---
unique-page-id: 2359746
description: 使用CNAME自訂您的登陸頁面URL - Marketo檔案 — 產品檔案
title: 使用CNAME自訂您的登陸頁面URL
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 使用CNAME自訂您的登陸頁面URL {#customize-your-landing-page-urls-with-a-cname}

即使Marketo代管您的登陸頁面，您也可以完全自訂URL。 在沒有CNAME時的外觀：

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

外觀：

`https://go.YourCompany.com/UnsubscribePage.html`

## 選擇CNAME {#choose-a-cname}

從登陸頁面URL的開頭選取要前往的單字。 只是一個字，應該相對較短。 範例:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

一個字(加上YourCompany.com)稱為CNAME。 您稍後需要此資訊，請記下資訊。

## 尋找您的Munchkin ID {#find-your-munchkin-id}

1. 前往 **管理員** 區域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. 按一下 **我的帳戶**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**需要管理員許可權**

1. 向下捲動至「支援資訊」並複製您的Munchkin ID。

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## 傳送要求給IT {#send-request-to-it}

請您的IT人員設定下列CNAME： (取代 [CNAME] 和 [Munchkin ID] 與上一步驟的文字連結。)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## 完成CNAME設定 {#complete-cname-setup}

1. 在您的IT建立CNAME後，請前往 **管理員** 區域。

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. 按一下 **登陸頁面**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. 在 **設定** 區段，按一下 **編輯**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. 輸入您的CNAME，在 **登陸頁面的網域名稱**，輸入您的 **後援頁面**，輸入您的 **首頁** 並按一下 **儲存**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>如果您的Marketo登陸頁面無法使用，您的後援頁面將會是重新導向到的頁面銷售機會。

做得好！ 您的登入頁面現在以公司網域命名。
