---
description: '[!DNL Dynamic Chat]活動 — Marketo檔案 — 產品檔案'
title: '[!DNL Dynamic Chat]個活動'
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# [!DNL Dynamic Chat]個活動 {#dynamic-chat-activities}

[!DNL Dynamic Chat]提供數個篩選器和觸發器以用於您的智慧清單。

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
    <td>當訪客與Dynamic Chat代理程式預約會議時發生。
    <br>每個訪客、每個工作階段可以有多個會議預約事件。</td>
  </tr>
</tbody>
</table>

## 注意事項 {#things-to-note}

* [!DNL Dynamic Chat]個流程步驟支援條件
* [!DNL Dynamic Chat]個活動可以同步至[[!DNL Marketo Sales Insight]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* 您可以在人員記錄的活動記錄檔中檢視個別[!DNL Dynamic Chat]活動
