---
description: Dynamic Chat 發行說明 - Marketo 文件 - 產品文件
title: Dynamic Chat 發行說明
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 342d52439a21668a3bf94e5149710b20e4ddb83f
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 3%

---

# TEMPDynamic Chat發行說明 {#dynamic-chat-release}

## 2024年9/10月發行版本 {#august-release}

### 增強型即時聊天分析 {#enhanced-live-chat-analytics}

Analytics Dashboard已進行數個增強功能，包括：

* 請求的即時聊天總數：「與代理商聊天」請求的訪客數

* 連線的即時聊天總數：已連線的訪客數與「與代理程式聊天」的請求總數

* 未接的即時聊天請求總數：「與代理聊天」的無人參與訪客數與請求總數

* 以分鐘為單位的平均聊天長度：分析訪客與您的代理之間的「平均聊天長度」

* 平均代理程式回應時間（以秒為單位）：分析代理程式回應其即時聊天問答所花費的「平均時間」

* 每日儀表板：即時聊天請求已成功連線、即時聊天請求已錯過、排序和篩選最近的即時聊天活動

熒幕擷圖

### 交談評分

根據潛在客戶聊天互動的品質來量化潛在客戶，並將該量度用作「Marketo Engage智慧行銷活動」中的觸發器/篩選器。 在下列活動中使用新屬性&#x200B;_交談分數_：

* 與對話方塊互動
* 已參與交談流程
* 與代理程式互動

**注意事項：**

* 分數值將來自0、1、2、3 （預設值為空值）

* 對話完成或捨棄後，活動中的會儲存評分值，並張貼無法編輯的文章????????????????????????????????（這是什麼意思）

* 設定分數：

   * 在代理程式收件匣中 — 在即時聊天期間，代理程式可以更新或設定對話的分數，該分數會儲存在對話活動中

   * 在資料流設計工具中 — 在目標卡片中，使用者可以更新或設定交談的分數

熒幕擷圖

熒幕擷圖

熒幕擷圖

### 新的潛在客戶建立邏輯 {#new-lead-creation-logic}

如果潛在客戶使用電子郵件`abc@test.com`填寫表單並以xyz編碼，稍後再使用電子郵件`def@test.com`填寫相同的表單，則會建立新的潛在客戶，但cookie xyz會與新的潛在客戶建立關聯並從潛在客戶`abc@test.com`中移除。

從那時起，`abc@test.com`將成為沒有Cookie的潛在客戶。 匿名銷售機會??

因此，當具有Cookie abc的訪客登陸頁面並提供電子郵件ID為`abc@p.com`時：

表格
