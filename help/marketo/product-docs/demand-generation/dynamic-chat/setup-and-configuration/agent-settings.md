---
description: 代理程式設定 — Marketo檔案 — 產品檔案
title: 專員設定
feature: Dynamic Chat
exl-id: a782ef9b-6a89-448a-8bd9-f127ceea3bf5
source-git-commit: 19f7a38a6a87bc66084e7e45f5bf49cd0d29c3cd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 2%

---

# 專員設定 {#agent-settings}

設定行事曆並設定會議/即時聊天可用性。

>[!PREREQUISITES]
>
>請確定您的代理程式已被授與適當的[許可權](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}。

![](assets/agent-settings-1.png)

## 連線行事曆 {#connect-calendar}

在[行事曆設定]索引標籤中，連線您的Outlook或Gmail行事曆，以用於聊天機器人中的約會排程。

![](assets/agent-settings-2.png)

使用者的行事曆連線至Dynamic Chat後，即會新增至佇列，且網站訪客的行事曆可用於排程約會。

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
   <td>決定訪客在可用的會議位置中看到的時間長度。</td>
  </tr> 
  <tr> 
   <td><b>會議之間的緩衝時間</b></td>
   <td>您設定為會議後緩衝的時間。 如果您設定30分鐘，則沒有人能夠在您的行事曆上排定的會議結束30分鐘之後與您預約會議。</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>您可以按一下右側的&#x200B;**+**&#x200B;符號，選取同一天的多重時間區塊（例如，8a-12p _和_ 1p-5p的星期五）。

## 即時聊天可用性 {#live-chat-availability}

設定您的時區以及每週時間/日期以接收即時聊天。

![](assets/agent-settings-5.png)

如果您已登入應用程式，您將會收到傳入聊天的應用程式內通知。 如果您未登入，將會收到瀏覽器通知（如果您已[設定](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}）。

>[!IMPORTANT]
>
>代理程式收件匣&#x200B;**中的[可用性切換](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"}將會覆寫您在[即時聊天可用性]索引標籤中輸入的內容**。 因此，如果您排程從1p到5p，但需要在3p快速休息，您就不需要變更代理程式設定。 可用性切換狀態將一直保留，直到您手動變更它，或直到到達您的可用性中的下一個時間區塊為止。

>[!TIP]
>
>您可以按一下右側的&#x200B;**+**&#x200B;符號，選取同一天的多重時間區塊（例如，8a-12p _和_ 1p-5p的星期五）。

## 代理程式設定檔像片

雖然代理程式可以上傳自己的設定檔像片，但該動作不會在Dynamic Chat中執行。 他們需要導覽至`account.adobe.com/profile`。 在這裡瞭解更多： [更新您的帳戶設定檔](https://helpx.adobe.com/tw/manage-account/using/edit-adobe-account-personal-profile.html)。

>[!NOTE]
>
>`experience.adobe.com`中顯示的設定檔影像&#x200B;**不支援**。
