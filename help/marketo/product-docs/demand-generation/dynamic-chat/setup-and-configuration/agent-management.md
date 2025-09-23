---
description: 代理程式管理 — Marketo檔案 — 產品檔案
title: 代理人管理
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# 代理人管理 {#agent-management}

在「代理程式管理」中，檢視您Dynamic Chat執行個體中的代理程式清單、管理團隊並設定遞補規則。

![](assets/agent-management-1.png)

## 專員 {#agents}

此標籤會列出您Dynamic Chat執行個體中的所有代理程式，並包含其名稱、電子郵件地址、即時聊天狀態等資訊。

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>沒有看到您&#x200B;_只是_&#x200B;新增的代理程式？ 在Adobe Admin Console中新增這些量度後，最多可能需要兩個小時才會顯示在這裡。

## 團隊 {#teams}

管理員可以建立代理程式團隊，以方便路由至特定的銷售代理程式群組。

>[!AVAILABILITY]
>
>若要存取Teams需要Dynamic Chat Prime訂閱。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

![](assets/agent-management-3.png)

### 建立團隊 {#create-a-team}

1. 按一下&#x200B;**+建立團隊**。

   ![](assets/agent-management-4.png)

1. 為團隊命名。

   ![](assets/agent-management-5.png)

1. 按一下&#x200B;**新增代理程式**&#x200B;下拉式清單，然後選取所需的代理程式。

   ![](assets/agent-management-6.png)

1. 按一下&#x200B;**建立**。

   ![](assets/agent-management-7.png)

## 遞補規則 {#fallback-rules}

### 會議遞補 {#meeting-fallback}

選取標準（系統）訊息或撰寫自訂訊息，讓訪客在無法預約會議時檢視。

![](assets/agent-management-8.png)

### 即時聊天遞補 {#live-chat-fallback}

選取標準（系統）訊息或撰寫自訂訊息，讓訪客在即時聊天無法使用時檢視。

![](assets/agent-management-9.png)

>[!NOTE]
>
>* 選取&#x200B;_包含會議預約選項_&#x200B;核取方塊會讓聊天訪客在沒有代理程式可供即時聊天時預約會議。
>
>* **對於任何自訂規則/團隊作為即時聊天卡**：檢查代理時，如果代理無法使用或無法連線，則會退回循環配置資源以嘗試「可用的代理」（所有當時可用的代理，無論將哪個路由邏輯/規則放在資料流中）。

>[!TIP]
>
>建立自訂訊息時，您可以設定字型樣式、使用連結，甚至插入表情符號！`:)`
