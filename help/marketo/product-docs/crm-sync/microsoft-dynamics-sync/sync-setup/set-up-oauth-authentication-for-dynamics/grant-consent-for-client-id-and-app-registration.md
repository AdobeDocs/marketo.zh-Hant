---
description: 授與用戶端ID和應用程式註冊的同意——行銷人員檔案——產品檔案
title: 授與用戶端ID和應用程式註冊的同意
translation-type: tm+mt
source-git-commit: 3a6d9987e214aa8606b9f5abdc780a81355b1001
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# 授與用戶端ID和應用程式註冊的同意{#grant-consent-for-client-id-and-app-registration}

## 授予同步用戶{#grant-delegated-user-permissions-for-the-sync-user}的授權用戶權限

1. 使用簡潔的文字程式(Notepad for Windows, Text Edit for Mac)建立統一資源識別碼(URI)以進行授權，方法是貼上下列文字並取代client_id、redirect_uri和state值。

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>client_id值</strong></td> 
      <td>應為「應用程式註冊」程式中產生的client_id</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri值</strong></td> 
      <td>應與在「應用程式註冊&gt;重新導向URI」時輸入的值相同</td> 
     </tr> 
     <tr> 
      <td><strong>狀態值</strong></td> 
      <td>可以是任何ID（例如，12345）</td> 
     </tr> 
    </tbody> 
   </table>

   最終URL應如下所示：`https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 開啟您在任何瀏覽器中建立的URI。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 以您要授予權限的同步用戶身份登錄。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >如果您已以管理員的身分在另一個索引標籤中登入Azure，您將需要使用不同的瀏覽器或Incognito模式，才能以同步使用者的身分登入。

1. 按一下&#x200B;**接受**。

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## 授予所有使用者的同意{#grant-consent-for-all-users}

身為管理員，您也可以代表您的租用戶中的所有使用者同意應用程式的授權權限。 管理許可會防止在租用戶中出現每個使用者的許可對話，而具有管理員角色的使用者也可以在Azure入口網站中完成。 瞭解哪些管理員角色可以[同意此處授予的權限](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference)。

1. 在Azure入口網站中，導覽至應用程式首頁。

1. 在「管理」下，按一下「API權限&#x200B;**」。**

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 按一下「授予管理員同意&#x200B;**（適用於租用戶）」按鈕。**

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. 按一下&#x200B;**是**&#x200B;確認。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[設定Microsoft Dynamics CRM應用程式以進行預備](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)
