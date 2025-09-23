---
description: 使用對話式流程登陸頁面 — Marketo檔案 — 產品檔案
title: 使用對話式流程登陸頁面
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 2%

---

# 使用對話式流程登陸頁面{#use-a-conversational-flow-landing-page}

將Dynamic Chat對話流程直接內嵌至Marketo Engage登陸頁面，讓訪客可透過Dynamic Chat排程會議，無須填寫表單或與聊天機器人互動。

>[!PREREQUISITES]
>
>建立僅包含[會議預訂](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md)卡片的簡單&#x200B;**交談流程**。

## 引導式登陸頁面 {#guided-landing-pages}

將下列程式碼內嵌在您的引導式登陸頁面範本中： `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`。

在編輯器中開啟引導式登陸頁面範本，並選取「對話流程」預留位置。

按一下「轉換流程」下拉式清單，並選取您在步驟1中建立的CF。

一律將傳遞型別保留為&#x200B;**內嵌**。 按一下「**插入**」。

您剛輸入的「對話流程」會在右側顯示為「要素」。

熒幕擷圖

>[!NOTE]
>
>目前，轉換流量不會出現在主預覽視窗中。

## 自由格式的登陸頁面 {#free-form-landing-pages}

文字

STEVE會議的筆記

引導式lp，範本的新div id，選擇conv flow

自由格式lp，帶入圖示 — 警告：新增附註 — 當您將cf放在編輯器上時，不會顯示預覽（沒有預留位置） — 「您看不到預覽」 — 在側邊欄上，他們會看到cf在頁面上 — 引導式lp將其列為元素 — 說明時使用「此時」 — 功能可能會在22日當週上線
