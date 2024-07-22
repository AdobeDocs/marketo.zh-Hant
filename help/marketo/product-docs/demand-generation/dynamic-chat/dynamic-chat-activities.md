---
description: Dynamic Chat活動 — Marketo檔案 — 產品檔案
title: Dynamic Chat活動
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 79b439a9bb3d3cd130eb5a7b52cea13988e7b88e
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Dynamic Chat活動 {#dynamic-chat-activities}

Dynamic Chat提供數個篩選器和觸發器用於您的智慧清單。

![](assets/dynamic-chat-activities-1.png)

## 定義 {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>已觸發</b></td>
    <td>當訪客符合對話方塊或對話流程的鎖定目標條件時，就會發生觸發事件，並顯示對話方塊。
    <br>每個訪客、每個工作階段一個觸發事件。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>已參與交談流程/對話方塊</b></td>
    <td>Web訪客首次在對話方塊或對話流程（按一下多重選擇選項、提交資訊、預約會議、開啟檔案等）中點選提示時就會發生參與。 如果訪客開啟對話方塊或對話流程，但未點按提示，則參與<b>未</b>記錄。 
    <br>每個訪客、每個工作階段一個參與事件。</td>
  </tr>
   <tr>
    <td style="width:25%"><b>已與Agent互動</b></td>
    <td>當訪客成功連線到即時聊天代理程式時發生。
    <br>每個訪客、每個工作階段都有1個參與代理程式事件。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>與檔案互動</b></td>
    <td>當訪客點按檔案卡中的檔案時發生。
    <br>每個訪客、每個工作階段可以有多個檔案互動。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>達成的目標</b></td>
    <td>當訪客達到目標時發生。 <br>每個訪客、每個工作階段可以有多個目標達成的事件。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>排定的會議</b></td>
    <td>當訪客與Dynamic Chat代理預訂會議時發生。
    <br>每個訪客、每個工作階段可以有多個會議預約事件。</td>
  </tr>
</tbody>
</table>

## 注意事項 {#things-to-note}

* Dynamic Chat流程步驟支援條件
* Dynamic Chat活動可以同步至[Marketo銷售分析](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* 您可以在人員記錄的活動記錄中檢視個別Dynamic Chat活動
