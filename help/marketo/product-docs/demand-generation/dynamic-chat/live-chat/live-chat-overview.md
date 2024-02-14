---
description: 即時聊天概述 — Marketo檔案 — 產品檔案
title: 即時聊天總覽
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: b05ae6f1b5a63cdf5a0d5da1cb1a6a3641d973c1
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 即時聊天總覽 {#live-chat-overview}

即時聊天可讓網站訪客與銷售代理進行即時聊天交談。

>[!NOTE]
>
>對話流程和即時聊天是共用的試用功能，對Dynamic Chat選取套件上的使用者具有100個參與的總生命週期限制。 達到此限制時，所有已發佈的交談流程將停止觸發，而要求與即時代理程式聊天的訪客將收到全域遞補訊息。 若要提高此上限，請聯絡您的客戶代表以討論套件升級選項。

## 新增即時聊天代理 {#add-live-chat-agents}

若要開始進行即時聊天，您需要將即時聊天代理新增為 [Adobe Admin Console中的使用者](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. 完成後，您可以新增 [即時聊天卡](#using-the-live-chat-card) 至新的或現有的對話方塊。

當訪客透過Dialog要求與代理程式聊天時，代理程式將擁有多個 [通知選項](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} 他們可以在哪裡開始與訪客聊天。

>[!NOTE]
>
>即時代理程式頭像會使用代理程式Adobe帳戶設定檔中的設定檔圖片。 若要更新影像，請依照 [這些步驟](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## 使用即時聊天卡 {#using-the-live-chat-card}

使用中的即時聊天卡 [串流設計工具](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} 您希望訪客與即時代理程式聊天時。

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>即時聊天卡必須一律為分支中的最後一張卡。 如果卡片放置在分支中的隨機點，可能會讓訪客突然將其連線到代理程式，感到驚訝。

### 最佳實務 {#best-practices}

* 在即時聊天卡之前使用問題卡詢問訪客是否想要連線。
* 訪客同意連線後，請使用資訊擷取卡片來收集部分資訊，例如名字/姓氏、電子郵件地址、職稱等。 （建議至少索取名字和電子郵件地址）。

## 即時聊天卡選項 {#live-chat-card-options}

按一下串流中的即時聊天卡片可讓您選擇訪客路由的方式。 從循環配置資源、代理程式、自訂規則或團隊中選擇。

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>循環配置資源</b></td>
   <td>聊天會依序指派給代理程式。</td>
  </tr> 
  <tr> 
   <td><b>專員</b></td>
   <td>選擇要接收聊天的特定代理程式。</td>
  </tr>
    <tr> 
   <td><b>自訂規則</b></td>
   <td>考慮將訪客路由到何處時，所有自訂規則都會循環使用。 如果訪客不符合任何自訂規則的資格，他們會取得 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">即時聊天遞補訊息</a>.</td>
  </tr> 
  <tr> 
   <td><b>團隊</b></td>
   <td>選擇要接收聊天的特定團隊。 如果選取此選項，則會在該群組中指派循環配置資源。</td>
  </tr>
 </tbody> 
</table>

## 即時聊天通知 {#live-chat-notifications}

為了接收即時聊天所需的瀏覽器通知，所有即時聊天代理程式必須在提示時啟用瀏覽器通知以進行Dynamic Chat。

### 啟用通知 {#enabling-notifications}

即時聊天代理程式在登入時會在熒幕上方看到橫幅，上面顯示「請啟用瀏覽器通知以接收即時聊天通知」。 按一下 **啟用**.

![](assets/live-chat-overview-4.png)

然後，瀏覽器會提示即時聊天代理顯示通知。 按一下 **允許**.

![](assets/live-chat-overview-5.png)

如果代理程式在允許瀏覽器後仍未收到瀏覽器通知，則可能需要在作業系統通知設定中啟用瀏覽器的通知：

[Mac的步驟](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[適用於Windows的步驟](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### 當即時聊天被路由到代理程式時 {#when-a-live-chat-is-routed-to-an-agent}

當即時聊天路由給代理時，他們會看到畫面頂端的藍色橫幅，要求他們接受。

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>您也可以選擇設定瀏覽器通知，若您未登入Dynamic Chat，通知會提醒您。
>
>* 在中啟用瀏覽器通知 [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* 在中啟用瀏覽器通知 [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### 注意事項 {#things-to-note}

* 在「接受聊天」訊息逾時之前，代理程式有45秒的時間回應。 之後，訪客將收到 [遞補訊息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. 對於將路由選項設定為的Dynamic Prime訂閱者 **團隊**，在後援訊息出現之前，將再嘗試一個代理程式。
* 目前每個代理程式限製為10個即時聊天。

>[!MORELIKETHIS]
>
>[代理程式收件匣](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
