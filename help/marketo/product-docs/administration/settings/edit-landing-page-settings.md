---
unique-page-id: 2359918
description: 編輯登陸頁面設定 — Marketo檔案 — 產品檔案
title: 編輯登陸頁面設定
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 9%

---

# 編輯登陸頁面設定 {#edit-landing-page-settings}

您可以編輯網域名稱和遞補頁面、啟用或停用表單預填、防止登陸頁面誤用等等。 方法如下。

>[!NOTE]
>
>**需要管理員許可權**

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/edit-landing-page-settings-1.png)

1. 按一下「**[!UICONTROL Landing Pages]**」。

   ![](assets/edit-landing-page-settings-2.png)

1. 在&#x200B;**[!UICONTROL Landing Pages]**&#x200B;區段中，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/edit-landing-page-settings-3.png)

1. 輸入您的網域和頁面資訊。

   ![](assets/edit-landing-page-settings-4.png)

   | 術語 | 定義 |
   |---|---|
   | [!UICONTROL Domain name for landing pages] | 這是您的CNAME。 CNAME是您為登陸頁面提供的網址(URL)的第一部分。 例如，在`https://go.yourCompany.com`中，「go」是CNAME。 您可以有多個，但大多數人只使用一個。 |
   | [!UICONTROL Fallback page] | 如果登入頁面不存在或已關閉，便可前往此處。 深入瞭解[後援頁面](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md)。 |
   | [!UICONTROL Homepage] | 輸入您的公司網站URL。 |

1. 核取&#x200B;**[!UICONTROL Form Prefill]**&#x200B;核取方塊，允許表單預先填入已知(cookie)人員的資訊。 取消勾選以封鎖。

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >如果您希望預填`<script>`標籤顯示在程式碼中`<head>`標籤的結尾，請核取&#x200B;**[!UICONTROL Inject Prefill Script at End of Head]**&#x200B;方塊。 如果您希望它顯示在開頭，請保持取消勾選狀態。
   >
   >檢查&#x200B;**[!UICONTROL Remove default favicon links]**&#x200B;以防止Marketo將任何Favicon連結插入程式碼中。

1. 選取之後，按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/edit-landing-page-settings-6.png)

   做得好！您的登入頁面現在擁有正確的資訊，應該會立即開始運作。
