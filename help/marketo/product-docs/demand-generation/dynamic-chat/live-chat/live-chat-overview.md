---
description: 即時聊天概述 — Marketo檔案 — 產品檔案
title: 即時聊天總覽
feature: Dynamic Chat
source-git-commit: 8b2eed5e28c46ea9c467fd25dd732c1654a09bed
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# 即時聊天總覽 {#live-chat-overview}

即時聊天可讓網站訪客與銷售代理進行即時聊天交談。

## 新增即時聊天代理 {#add-live-chat-agents}

若要開始進行即時聊天，您需要將即時聊天代理新增為 [Adobe Admin Console中的使用者](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. 完成後，您可以新增 [即時聊天卡](#using-the-live-chat-card) 至新的或現有的對話方塊。

當訪客透過Dialog要求與代理程式聊天時，代理程式將擁有多個 [通知選項](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} 他們可以在哪裡開始與訪客聊天。

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

>[!MORELIKETHIS]
>
>[專員收件匣](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
