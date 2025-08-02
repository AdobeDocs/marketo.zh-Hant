---
description: Dynamic Chat常見問題集 — Marketo檔案 — 產品檔案
title: Dynamic Chat常見問題集
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Dynamic Chat常見問題集 {#dynamic-chat-faq}

請參閱下方的Dynamic Chat相關常見問題解答。

**我似乎無法存取Dynamic Chat。 我要如何取得？**

請洽詢您的Marketo Engage管理員，確定他們已在Adobe Admin Console中[將您新增為使用者](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"}。

**我可以在公司網站上的任何地方安裝Dynamic Chat，還是只能在Marketo登陸頁面上運作？**

Dynamic Chat JavaScript程式碼片段可安裝在任何網站以及Marketo登陸頁面上。

**資料會儲存多久以用於報告？**

90天。 如需限制/引數的完整清單，請造訪Marketo Engage [產品說明頁面](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}。

**Dynamic Chat是否支援英文以外的任何語言？**

可以。Dynamic Chat支援下列語言：法文、西班牙文、德文、日文、荷蘭文、義大利文、巴西葡萄牙文、韓文、簡體和繁體中文。 深入瞭解[變更語言](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}。

**您支援AI/NLP功能嗎？**

我們不支援AI/NLP功能。

**我如何鎖定匿名人員？**

在您的對話方塊中，您需要使用&#x200B;_人員電子郵件為空白_&#x200B;屬性。

**什麼符合參與交談的資格？**

當訪客在對話方塊或對話流程中回應機器人時，參與的對話就會發生。 如果訪客開啟聊天機器人但未回應機器人（例如，選取回應或提交資訊），則不會計為參與。

**如果我達到每月參與交談的上限，會發生什麼事？**

當您達到每月參與交談上限時，所有發佈的對話與交談流程都將停止觸發，直到您提高上限或在下個月初重設上限為止。

**我如何知道何時接近參與交談的上限？**

當您達到90%的參與交談限制時，Dynamic Chat管理員會收到電子郵件通知，而所有使用者都會在Dynamic Chat中看到橫幅通知。

**如果訪客參與對話方塊，然後連線到即時代理程式，這會計為一次參與還是兩次參與？**

對於Select套件的客戶，這將計為兩個獨立的參與 — 一個用於Dialog參與，另一個用於即時聊天參與。 對於Prime套件上的客戶，即時聊天參與不會個別計算，因此這只會計為一次參與。

**參與交談限制重設的頻率為何？**

每個日曆月的第一天會重設參與的交談限制。

**為什麼聊天機器人在我完成交談後沒有回來？**

對話方塊的設計僅向訪客顯示一次。 因此，當訪客到達對話方塊中任何指定分支的結尾時，該對話方塊就會被視為完成，且不會再向該訪客顯示。

**當我在「我的Marketo」中按一下Dynamic Chat圖磚並登入Adobe Experience Cloud時，為何會收到下列訊息？ _您的Adobe ID似乎未連結Adobe Experience Cloud解決方案帳戶_。&quot;**

這很可能表示您尚未在Adobe Admin Console中新增為Dynamic Chat使用者。 請聯絡您Adobe組織的系統管理員或Dynamic Chat的產品管理員，以要求Dynamic Chat的存取權。

**如何存取參與交談的記錄？**

任何已知的潛在客戶可以透過Dynamic Chat中的「參與對話方塊」活動，與Dynamic Chat對話方塊互動，且其對話狀態為「已完成」或「已捨棄」，即可存取Marketo Engage成績單。

**訪客參與對話後，可以重新開始對話或返回上一個問題嗎？**

目前沒有系統化的方式可重新啟動交談或返回上一個時間點，但這是在Dynamic Chat藍圖上的。

**Dynamic Chat是否與Salesforce整合？**

Dynamic Chat透過Salesforce整合與Marketo Engage Salesforce整合。

**我的行事曆已在Dynamic Chat中連線，而且我包含在路由規則中，所以為什麼我沒有收到任何會議？**

這很可能代表您的行事曆連線需要重新驗證。 當您變更行事曆提供者的密碼，而Dynamic Chat中斷連線時，最常會發生這種情況。 您只需前往Dynamic Chat中的「代理程式設定」頁面，然後按一下「重新驗證行事曆」即可。

**對話方塊和對話流程之間有何差異？**

對話方塊是自動顯示給符合一組已定義目標定位條件的Web訪客的對話。 「對話流程」只會顯示在網頁上執行特定動作（例如按下按鈕）的訪客。

**是否有辦法使用Dynamic Chat直接從電子郵件預約會議？**

是！[瞭解如何進行](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}。

**「已參與」或「已取得人員」等辭彙的意義是什麼？**

Dynamic Chat中使用多個辭彙。 其中許多的定義可在各自區域的說明文章中找到。

* 您可以在此找到「已取得人員」之類的Analytics辭彙[](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}。
* 智慧清單觸發程式/篩選器定義[可以在這裡找到](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}。
* 各種串流Designer卡片[的說明可在此找到](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}。

**我可以在沒有Marketo Engage的情況下使用Dynamic Chat嗎？**

不可以。 雖然Dynamic Chat是獨立於Marketo Engage的應用程式，但兩者有千絲萬縷的聯絡。
