---
description: 授予使用者端ID和應用程式註冊的同意 — Marketo檔案 — 產品檔案
title: 授予使用者端ID和應用程式註冊的同意
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 授予使用者端ID和應用程式註冊的同意 {#grant-consent-for-client-id-and-app-registration}

## 授與已委派使用者許可權給同步使用者 {#grant-delegated-user-permissions-for-the-sync-user}

1. 使用簡潔的文字程式(Windows專用的「記事本」、Mac專用的「文字編輯」)來建立統一資源識別碼(URI)以進行授權，方法是貼上以下文字並替代client_id、redirect_uri和狀態值。

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
      <td>應為應用程式註冊程式中產生的client_id</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri值</strong></td> 
      <td>應與應用程式註冊&gt;重新導向URI時輸入的值相同</td> 
     </tr> 
     <tr> 
      <td><strong>狀態值</strong></td> 
      <td>可以是任何ID (例如，12345)</td> 
     </tr> 
    </tbody> 
   </table>

   最終URL看起來應該像這樣： `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 在任何瀏覽器中開啟您建立的URI。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 以您授與許可權的同步處理使用者身分登入。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >如果您已在其他索引標籤中以管理員身分登入Azure，則需使用不同的瀏覽器或無痕模式才能以同步使用者身分登入。

1. 按一下 **Accept**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## 授予所有使用者同意 {#grant-consent-for-all-users}

身為管理員，您也可以代表租使用者中的所有使用者，同意應用程式的委派許可權。 管理同意可防止租使用者中的每個使用者都出現同意對話方塊，並且可由具有管理員角色的使用者在Azure入口網站中完成。 瞭解哪些管理員角色可以 [在此同意委派許可權](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. 在您的Azure入口網站中，導覽至應用程式首頁。

1. 在管理底下，按一下 **API許可權**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 按一下 **授予管理員同意** （適用於租使用者）按鈕。

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. 按一下 **是** 以確認。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

