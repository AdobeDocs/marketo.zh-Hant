---
unique-page-id: 14352581
description: 調節錯誤——行銷人員文檔——產品文檔
title: 調節錯誤
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# 調節錯誤 {#throttling-errors}

## 已達到檔案限制 {#file-limit-reached}

如果您要透過自己的伺服器傳送，則會限制您同時傳送的電子郵件數量。 透過Sales Connect傳送時，您可以傳送許多電子郵件，但我們會嘗試同時傳送所有電子郵件。 因此，如果您知道伺服器每分鐘會中斷100封電子郵件，您只需要透過網路應用程式傳送多達100封 [電子郵件](http://toutapp.com/login)。 否則，由於您的伺服器中已調節電子郵件，這些電子郵件可能會降落在這裡。

## 驗證錯誤 {#authentication-error}

這表示我們無法驗證到SMTP伺服器的連接。 最有可能的是，您的密碼最近有所變更，您只需要驗證新的認證。

要執行此操作，請轉至 [SMTP設定](http://docs.marketo.com/display/docs/assets/external-link-1.jspa) `where you should see the same error message. Update your credentials and hit **Authenticate and Save** to see a confirmation message.`

進入您的「傳送失敗」，嘗試重新傳送這些電子郵件。
