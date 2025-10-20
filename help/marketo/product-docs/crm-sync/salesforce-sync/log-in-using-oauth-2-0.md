---
description: 使用OAuth 2.0登入 — Marketo檔案 — 產品檔案
title: 使用 OAuth 2.0 登入
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 7234082102356fc05c760f359ef19ca8cff375b5
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 2%

---

# 使用 OAuth 2.0 登入 {#log-in-using-oauth-2-0}

Salesforce使用OAuth通訊協定，讓應用程式的使用者能夠安全存取（使用OAuth 2.0驗證應用程式）資料，不必揭露登入認證。 以下是將Marketo Engage安全地連線並與Salesforce同步要執行的步驟。

>[!IMPORTANT]
>
>若要使用OAuth連線Marketo和[!DNL Salesforce]，請透過私人（無痕）瀏覽器登入Marketo，以避免使用錯誤的使用者名稱連線到[!DNL Salesforce]。

## 設定外部使用者端應用程式 {#set-up-external-client-app}

>[!NOTE]
>
>自2025年9月起，Salesforce開始限制[連線應用程式](https://help.salesforce.com/s/articleView?id=005132365&type=1){target="_blank"}的使用。 若現有使用者已根據我們的檔案設定連線應用程式，您可以將「核准已解除安裝的連線應用程式」許可權新增至Marketo Sync使用者的設定檔，或使用下列指示建立新的外部使用者端應用程式。

1. 在Salesforce中，按一下齒輪圖示並選取&#x200B;**設定**。

   ![](assets/log-in-using-oauth-1.png)

1. 在[快速尋找]方塊中，輸入`App Manager`，然後選取&#x200B;**應用程式管理員**。

   ![](assets/log-in-using-oauth-2.png)

1. 按一下&#x200B;**新增外部使用者端應用程式**。

   ![](assets/log-in-using-oauth-3.png)

1. 在&#x200B;_基本資訊_&#x200B;下填寫詳細資料。 將&#x200B;_散發狀態_&#x200B;設定為&#x200B;**本機**。

   ![](assets/log-in-using-oauth-4.png)

1. 展開&#x200B;**API （啟用OAuth設定）**&#x200B;區段並選取&#x200B;**[!UICONTROL Enable OAuth]**&#x200B;核取方塊。 針對&#x200B;_回撥URL_，請輸入`https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`。 選取所有可用的OAuth範圍，然後按一下向右箭頭以新增它們。

   ![](assets/log-in-using-oauth-5.png)

1. 在「_流量啟用_」下，確定未選取任何方塊。

   ![](assets/log-in-using-oauth-6.png)

1. 在&#x200B;_安全性_&#x200B;下，確定只選取&#x200B;**Web伺服器流程需要密碼**&#x200B;和&#x200B;**重新整理權杖流程需要密碼**。

   ![](assets/log-in-using-oauth-7.png)

1. 略過最後四個區段，然後按一下[建立]。**&#x200B;**

   ![](assets/log-in-using-oauth-8.png)

1. 建立新的外部使用者端應用程式之後，請選取&#x200B;**設定**&#x200B;標籤，並展開&#x200B;**OAuth設定**&#x200B;區段。

   ![](assets/log-in-using-oauth-9.png)

1. 按一下&#x200B;**消費者金鑰和密碼**&#x200B;按鈕，提示開啟新標籤。 複製並儲存這兩個數字(您稍後需要它們以用於Marketo Engage)。

   ![](assets/log-in-using-oauth-10.png)

## 設定Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* 必須為Salesforce Sync使用者啟用API存取權(如果您是Salesforce Professional Edition使用者，預設將無法使用該存取權 — 請聯絡您的Salesforce帳戶主管)。
>* 必須在Salesforce中建立Marketo Sync使用者。
>* 針對現有客戶，系統會在客戶的訂閱上啟用「為SFDC同步啟用OAuth」功能。
>* 快顯封鎖程式已停用。
>* 已建立連線應用程式，而且我們有[!UICONTROL Consumer Key]和[!UICONTROL Consumer Secret]可供使用。

>[!CAUTION]
>
>按一下&#x200B;**[!UICONTROL Sync Fields]**&#x200B;之前，請務必向同步使用者隱藏Marketo中所有不需要的欄位。 按一下「同步欄位」後，使用者在SFDC中看到的所有欄位將會在Marketo中永久建立，且無法刪除。

1. 在Marketo管理區段中，按一下&#x200B;**[!UICONTROL CRM]**，然後按&#x200B;**[!UICONTROL Sync with Salesforce]**。

   ![](assets/log-in-using-oauth-11.png)

1. 新增您先前錄製的消費者金鑰和消費者密碼資訊，然後按一下「**[!UICONTROL Save]**」。

   ![](assets/log-in-using-oauth-12.png)

1. 在Marketo Salesforce同步頁面上，按一下&#x200B;**[!UICONTROL Login with Salesforce]**&#x200B;按鈕。

   ![](assets/log-in-using-oauth-13.png)

   >[!CAUTION]
   >
   >如果您看到使用者名稱/密碼/權杖欄位，而不是「使用Salesforce登入」按鈕，表示您的Marketo訂閱已啟用基本驗證。 請參考[使用基本驗證設定Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}。 使用一組憑證開始同步後，Salesforce憑證或訂閱即無法切換。 若要設定Oauth 2.0以進行Salesforce驗證，請連絡[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

1. 隨即顯示包含Salesforce登入頁面的快顯視窗。 輸入「Marketo同步使用者」認證並登入。

   ![](assets/log-in-using-oauth-14.png)

1. 輸入您透過電子郵件(由Salesforce傳送)收到的驗證碼，然後按一下&#x200B;**[!UICONTROL Verify]**。

   ![](assets/log-in-using-oauth-15.png)

1. 在成功驗證後，存取頁面將會顯示以請求存取。 按一下「**[!UICONTROL Allow]**」。

   ![](assets/log-in-using-oauth-16.png)

1. 幾分鐘後，Marketo中將會顯示快顯視窗。 按一下「**[!UICONTROL Confirm Credentials]**」。

   ![](assets/log-in-using-oauth-17.png)

1. 欄位同步完成後，請按一下&#x200B;**[!UICONTROL Start Salesforce Sync]**。

   ![](assets/log-in-using-oauth-18.png)

1. 按一下「**[!UICONTROL Start Sync]**」。

   ![](assets/log-in-using-oauth-19.png)

您在Marketo和[!DNL Salesforce]之間的同步處理目前正在進行中。

![](assets/log-in-using-oauth-20.png)

>[!MORELIKETHIS]
>
>* [步驟3之1：將Marketo欄位新增至Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [步驟2之3：建立Marketo (Enterprise/Unlimited)的Salesforce使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [在Marketo AppExchange中安裝Salesforce Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [在Marketo Enterprise/Unlimited中設定Salesforce Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
