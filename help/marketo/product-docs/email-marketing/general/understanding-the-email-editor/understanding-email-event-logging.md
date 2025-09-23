---
unique-page-id: 1147356
description: 瞭解電子郵件事件記錄 — Marketo檔案 — 產品檔案
title: 了解電子郵件事件記錄
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 3%

---

# 了解電子郵件事件記錄 {#understanding-email-event-logging}

傳送電子郵件時，Marketo會將不同的資料點記錄到個人的活動記錄中。 以下是基本內容。

| 事件 | 說明 |
|---|---|
| [!UICONTROL Sent] | 每次從Marketo伺服器傳送電子郵件時都會記錄，無論該電子郵件是否實際傳送。 跳出的電子郵件仍會記錄為「已傳送」。 |
| [!UICONTROL Delivered] | 每次收件者郵件伺服器接受電子郵件時都會記錄。 這並不意味著它避免了垃圾郵件過濾器。 每個已傳送電子郵件只能有1個傳遞。 |
| [!UICONTROL Hard Bounced] | 部分硬跳出是垃圾郵件封鎖的結果，因此我們不會嘗試在任何行銷活動中24小時內傳送電子郵件給該人。 其他硬跳出（例如不存在收件匣）是永久性的，我們絕不會從任何行銷活動再次傳送電子郵件給使用者。 |
| [!UICONTROL Soft Bounced] | 當伺服器回應不清楚、信箱已滿或一般伺服器問題時記錄。 我們會讓這些人員接受24到36小時的重試邏輯，以備未來傳送時使用。 這不會使該人失去其他郵件的資格。 |
| [!UICONTROL Opened] | 當收件者檢視包含「未封鎖」影像的電子郵件時記錄。 每個電子郵件、每個人、每個智慧行銷活動僅會記錄一個開啟事件。 如果他們從收件匣開啟相同電子郵件兩次，記錄不會超過一次。 |
| [!UICONTROL Clicked] | 每次在瀏覽器中載入電子郵件中經過裝飾的URL時（按一下連結的結果），都會記錄下來。 這通常是收件者點按，但也可能是剪下/貼上。 |
| [!UICONTROL Unsubscribed] | 當有人點按電子郵件的取消訂閱連結並提交取消訂閱表單時記錄。 |

>[!CAUTION]
>
>如果相同的電子郵件從相同的行銷活動傳送給同一個人兩次，則會記錄&#x200B;**[!UICONTROL Opened]**&#x200B;事件，最多記錄1次。
