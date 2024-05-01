---
description: 回呼函式 — Marketo檔案 — 產品檔案
title: 回呼函式
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: f355022fb7e6f733bb7485229e395b0fe1a9818f
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 3%

---

# 回呼函式 {#callback-functions}

您可以使用Dynamic ChatWidget回呼函式，將交談事件傳送至任何協力廠商平台。

## 快速入門 {#getting-started}

此事件代表Dynamic ChatWidget已可供使用，並在網頁中載入與Dynamic Chat相關的所有指令碼時引發。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
}); 
```

## 交談事件 {#conversation-events}

這些事件與針對特定訪客之特定頁面的對話有關。

### 交談已觸發

會解析針對網站訪客的對話（例如，對話方塊），並向他們顯示聊天機器人。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // code here will execute when the chatbot is loaded for a visitor 
    }); 
});  
```

### 交談已參與 {#conversation-engaged}

訪客與聊天機器人互動（例如，提供他們的第一個回應）。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when a visitor engages with the chatbot 
     }); 
}); 
```

### 交談已完成 {#conversation-completed}

訪客已達到交談的結尾。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when a conversation is completed 
     }); 
}); 
```

### 交談已關閉

訪客在到達結尾前已關閉交談。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when a conversation is closed 
    }); 
}); 
```

此 `event` parameter是物件，其中包含與交談相關的中繼資料。 您可以存取此中繼資料 `event.data`.

以下是您可以存取的一些主要中繼資料值：

<table>
<thead>
  <tr>
    <th style="width:75%">中繼資料</th>
    <th style="width:25%">屬性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>對話名稱</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>交談ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>交談型別（對話方塊/交談流程）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI型別（快顯/聊天機器人/內嵌）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>工作階段ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## 訪客輸入事件

當參與交談的訪客提供其聯絡資訊（例如電話號碼或電子郵件地址）時，就會觸發這些事件。 以下是屬於此類別的事件。

### 電話號碼 {#phone-number}

當訪客在交談期間提供電話號碼時，就會觸發此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
 // code here will execute when a visitor provides their phone number 
    }); 
});  
```

### 電子郵件ID {#email-id}

當訪客在交談期間提供其電子郵件地址時，就會觸發此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
}); 
```

此 `event` parameter是物件，其中包含與交談相關的中繼資料。 您可以存取此中繼資料 `event.data`.

以下是您可以存取的一些主要中繼資料值：

<table>
<thead>
  <tr>
    <th style="width:75%">中繼資料</th>
    <th style="width:25%">屬性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>對話名稱</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>交談ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>交談型別（對話方塊/交談流程）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI型別（快顯/聊天機器人/內嵌）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>工作階段ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## 會議預約事件 {#meeting-booking-events}

當訪客與您的業務代表預約會議時，就會觸發這些事件。

以下是屬於此類別的事件。

### 會議已預訂 {#meeting-booked}

當訪客在代理人的行事曆上預約會議時，就會觸發此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
}); 
```

此 `event` parameter是物件，其中包含與交談相關的中繼資料。 您可以存取此中繼資料 `event.data`.

以下是您可以存取的一些主要中繼資料值：

<table>
<thead>
  <tr>
    <th style="width:75%">中繼資料</th>
    <th style="width:25%">屬性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>對話名稱</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>交談ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>交談型別（對話方塊/交談流程）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI型別（快顯/聊天機器人/內嵌）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>工作階段ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>專員名稱</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>代理程式ID</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>會議資訊</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## 即時聊天活動 {#live-chat-events}

當訪客在參與聊天機器人期間與即時代理連線時，就會觸發這些事件。

以下是屬於此類別的事件。

### 已要求即時交談 {#live-chat-requested}

當訪客選取選項與即時代理程式聊天且正在解析可用的代理程式時，就會觸發此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests a live chat 
    }); 
}); 
```

### 即時聊天已啟動 {#live-chat-initiated}

當訪客選取選項與即時代理程式聊天且代理程式接受聊天時，就會觸發此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepts the chat 
    }); 
}); 
```

### 即時聊天已結束 {#live-chat-ended}

當訪客與即時代理程式之間的交談結束時，就會觸發此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
}); 
```

### 即時聊天逾時 {#live-chat-timeout}

當即時聊天對話因訪客停止回應或捨棄而逾時時，就會觸發此事件。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandons a live chat 
    }); 
}); 
```

此 `event` parameter是物件，其中包含與交談相關的中繼資料。 您可以存取此中繼資料 `event.data`.

以下是您可以存取的一些主要中繼資料值：

<table>
<thead>
  <tr>
    <th style="width:75%">中繼資料</th>
    <th style="width:25%">屬性</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>對話名稱</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>交談ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>交談型別（對話方塊/交談流程）</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI型別（快顯/聊天機器人/內嵌）</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>工作階段ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>專員名稱</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>代理程式ID</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

如果您想要將任何這些事件傳送至Adobe Analytics或Google Analytics之類的Dynamic Chat平台，則必須在分析事件內新增其各自的追蹤呼叫。 它看起來會類似於下面的範例。

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // Enter Adobe Analytics or Google Analytics function here 
    ga('send', 'event', { 
      eventCategory: Dynamic Chat Conversations', 
      eventAction: 'Conversation Triggered', 
      eventLabel: event.data.payload.id, 
    }); 
    }); 
}); 
```
