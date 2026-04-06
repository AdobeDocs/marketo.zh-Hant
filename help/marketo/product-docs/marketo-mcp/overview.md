---
description: 即將推出。
title: MCP概述檔案
hide: true
hidefromtoc: true
source-git-commit: 62f5166e6a77c8ef50e7c596754205e8f02c6dc7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# MCP概述檔案 {#overview}

其他人的文字：

Marketo Engage公用MCP伺服器是雲端型服務，可讓AI代理程式將Marketo REST API視為結構化工具來存取。 它以模型上下文通訊協定(MCP)為基礎，提供標準化的結構描述導向介面，可讓AI系統安全有效地與Marketo互動。

MCP伺服器不以手動方式將Marketo端點整合到每個應用程式中，而是提供單一AI原生閘道，讓MCP相容的代理程式能夠探索可用的作業、瞭解必要的引數，並透過一致的通訊協定執行動作。

有許多可用的工具，包含公用REST API和內部API，可在UI中執行Marketo核心功能，但透過API呼叫。 隨著工具的開發，將會持續新增更多工具。 &lt;----需要釐清

MCP伺服器是作為自助服務提供，並可透過Adobe IO架構設定，方法是建立端點並驗證連線。 如需詳細資訊和設定詳細資訊，請造訪Adobe Developer網站（在這裡新增連結）。 這個？ https://developer.adobe.com/marketo-apis/

顯示為SOAP API的Campaign工具已轉換為REST API並已新增。

設定之後，若要檢視可用的工具清單，請遵循此處（超連結）的指示。

注意：沒有可用的工具包括「停用行銷活動」和「刪除靜態清單」（待定）。

//////////////////////////////////////////////

## 設定 {#settings}

請依照下列步驟，將NAME連線至您的Marketo Engage帳戶。

1. 在「我的Marketo」中，按一下&#x200B;**使用AI建置**&#x200B;圖磚。

熒幕擷圖

1. 按一下齒輪圖示

需要尚未連線的執行個體