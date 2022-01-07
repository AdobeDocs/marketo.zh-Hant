---
description: 授與用戶端Id和應用程式註冊的同意 — Marketo檔案 — 產品檔案
title: 授予用戶端Id和應用程式註冊的同意
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
source-git-commit: e8ba27c09165aa844ae6df175464d989b1931bad
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 授予用戶端Id和應用程式註冊的同意 {#grant-consent-for-client-id-and-app-registration}

## 授予同步用戶的委派用戶權限 {#grant-delegated-user-permissions-for-the-sync-user}

1. 使用簡潔文本程式(Notepad for Windows, Text Edit for Mac)通過貼上以下文本並替換clientid、redirecturi和state值來建立統一資源標識符(URI)以進行授權。

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
      <td>應與在應用程式註冊&gt;重新導向URI時輸入的值相同</td> 
     </tr> 
     <tr> 
      <td><strong>狀態值</strong></td> 
      <td>可以是任何ID(例如12345)</td> 
     </tr> 
    </tbody> 
   </table>

   最終URL應如下所示： `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 開啟在任何瀏覽器中建立的URI。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 以要授予權限的同步用戶身份登錄。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >如果您已在其他索引標籤中以管理員身分登入Azure，則需使用不同的瀏覽器或Incognito模式才能以同步使用者身分登入。

1. 按一下 **接受**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## 授予所有使用者的同意 {#grant-consent-for-all-users}

身為管理員，您也可以代表租用戶中的所有使用者同意應用程式的委派權限。 管理同意會防止租戶中的每位使用者出現同意對話方塊，具有管理員角色的使用者可在Azure入口網站中完成。 了解哪些管理員角色可以 [同意此處的委派權限](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. 在您的Azure入口網站中，導覽至應用程式首頁。

1. 在管理下，按一下 **API權限**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 按一下 **授予管理員同意** （適用於租用戶）按鈕。

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. 按一下 **是** 確認。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

