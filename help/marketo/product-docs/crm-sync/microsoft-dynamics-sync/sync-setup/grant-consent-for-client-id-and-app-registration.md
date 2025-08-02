---
description: 授予使用者端ID和應用程式註冊的同意 — Marketo檔案 — 產品檔案
title: 授予使用者端ID和應用程式註冊的同意
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
feature: Microsoft Dynamics
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# 授予使用者端ID和應用程式註冊的同意 {#grant-consent-for-client-id-and-app-registration}

請依照下列步驟瞭解如何授與必要同意/許可權。

## 授與同步處理使用者的委派使用者許可權 {#grant-delegated-user-permissions-for-the-sync-user}

1. 使用純文字程式(Windows的Notepad，Mac的Text Edit)建立統一資源識別碼(URI)以進行授權，方法是貼上以下文字並替代`client_id`、`redirect_uri`和`state`值。

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

   最終URL應該看起來像這樣： `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 在任何瀏覽器中開啟您建立的URI。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 以您要授與許可權的同步處理使用者身分登入。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >如果您已在其他索引標籤中以管理員身分登入Azure，您將需要使用不同的瀏覽器或無痕模式以同步使用者身分登入。

1. 按一下「**[!UICONTROL Accept]**」。

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## 授予所有使用者同意 {#grant-consent-for-all-users}

身為管理員，您也可以代表租使用者中的所有使用者同意應用程式的委派許可權。 管理同意可防止租使用者中的每個使用者都出現同意對話方塊，並且可由具有管理員角色的使用者在Azure入口網站中完成。 瞭解哪些管理員角色可以[在此同意委派許可權](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference)。

1. 在您的Azure入口網站中，導覽至應用程式首頁。

1. 在[!UICONTROL Manage]底下，按一下&#x200B;**[!UICONTROL API Permissions]**。

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 按一下&#x200B;**[!UICONTROL Grant admin consent]** （適用於租使用者）按鈕。

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. 按一下&#x200B;**[!UICONTROL Yes]**&#x200B;確認。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)
