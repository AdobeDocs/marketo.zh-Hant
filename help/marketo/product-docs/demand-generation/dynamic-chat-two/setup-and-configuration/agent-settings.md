---
description: 代理程式設定 — Marketo檔案 — 產品檔案
title: 專員設定
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: d22849c01d55dc4c5bca30cbd39bfe66bfaeb473
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 2%

---

# 專員設定 {#agent-settings}

設定行事曆並設定會議/即時聊天可用性。

![](assets/agent-settings-1.png)

## 連線行事曆 {#connect-calendar}

在[行事曆設定]索引標籤中，連線您的Outlook或Gmail行事曆，以用於聊天機器人中的約會排程。

![](assets/agent-settings-2.png)

一旦使用者的行事曆連線到Dynamic Chat，他們就會新增到佇列中，網站訪客將可使用此行事曆排程約會。

>[!NOTE]
>
>您可以為每個使用者連線一個行事曆。 如果您想要在多個行事曆上接收會議，您必須新增多個使用者，並讓每個使用者連線其行事曆。

使用者也可以在排程使用者行事曆上的約會時，自訂傳送給訪客的邀請內文。 他們也可以選取底部的核取方塊，以包含Google會議或Microsoft Teams連結（視連線的行事曆而定）。

![](assets/agent-settings-3.png)

>[!TIP]
>
>使用權杖圖示（大括弧），使用人員或公司屬性個人化您的會議預約確認電子郵件。

### 權限 {#permissions}

使用Outlook設定可授予Dynamic Chat下列許可權：

* 行事曆的完整存取權
* 登入並讀取您的設定檔
* 維護您授予其資料存取權的資料存取權
* 讀取您的信箱設定

使用Google設定可授予Dynamic Chat下列許可權：

* 建立、變更或刪除行事曆
* 更新個別的行事曆事件
* 變更您的設定，包括誰能看見您的活動
* 變更與誰共用行事曆
* 存取您的姓名、電子郵件地址、語言偏好設定和設定檔圖片

## 會議預約可用性 {#meeting-booking-availability}

設定您的時區與每週時間/日期以接收會議預約。

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>會議持續時間</b></td>
   <td>會議長度上限。  — 會發生什麼事？ 自動結束？</td>
  </tr> 
  <tr> 
   <td><b>會議之間的緩衝時間</b></td>
   <td>您設定為會議後緩衝的時間。 如果您設定30分鐘，則沒有人能夠在您的行事曆上排定的會議結束31分鐘之後與您預約會議。 - 31或30???????????</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>您可以在同一天選取多個時間區塊(例如，從8a到12p的星期五 _和_ 1p-5p)，按一下 **+** 在右側登入。

## 即時聊天可用性 {#live-chat-availability}

設定您的時區以及每週時間/日期以接收即時聊天。

![](assets/agent-settings-5.png)

如果您已登入應用程式，您將會收到傳入聊天的應用程式內通知。 如果您未登入，將會收到瀏覽器通知(在Google Chrome中)。

>[!IMPORTANT]
>
>此 [可用性切換](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md#availability-toggle){target="_blank"} 在代理程式收件匣中 **將覆寫** 您在「即時聊天可用性」標籤中輸入的內容。 因此，如果您排程從1p到5p，但需要在3p快速休息，您就不需要變更代理程式設定。 可用性切換狀態將一直保留，直到您手動切換它，或直到到達您的可用性中的下一個時間區塊為止。

>[!TIP]
>
>您可以在同一天選取多個時間區塊(例如，從8a到12p的星期五 _和_ 1p-5p)，按一下 **+** 在右側登入。
