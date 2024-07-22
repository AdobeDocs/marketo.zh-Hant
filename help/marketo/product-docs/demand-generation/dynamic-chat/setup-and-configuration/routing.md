---
description: 路由 — Marketo檔案 — 產品檔案
title: 路由
feature: Dynamic Chat
exl-id: e20193b9-55c1-40f2-9e42-5b5dc9b88144
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# 路由 {#routing}

以Dynamic Chat預約的會議可以兩種方式傳送。 循環配置資源，或使用自訂規則。

循環配置資源：會議會依序指派給代理程式。 因此，如果您有五個代理程式，而代理程式三參加最後一個會議，則代理程式四會取得下一個會議，接著是代理程式五，然後回到代理程式一。

自訂規則：您可以根據您選取的屬性選擇特定代理以接收會議。

>[!NOTE]
>
>帳戶路由會獲得最高優先順序。 當訪客到達交談點以預約會議或啟動即時交談時，會先檢查[帳戶路由](#account-routing)，然後再考慮其他路由選項。

## 建立自訂規則 {#create-a-custom-rule}

在此範例中，我們會將推斷的CA、OR和WA狀態的所有會議傳送給代理程式John。

1. 在[設定]下，按一下[路由規則]。****。

   ![](assets/routing-1.png)

1. 按一下「**自訂規則**」標籤。

   ![](assets/routing-2.png)

1. 按一下&#x200B;**建立規則**。

   ![](assets/routing-3.png)

1. 為規則命名。 您可以選擇新增說明並設定其優先順序層級。 按一下&#x200B;**下一步**。

   ![](assets/routing-4.png)

1. 選擇所需的代理程式。

   ![](assets/routing-5.png)

1. 拖曳到您所需的屬性上。

   ![](assets/routing-6.png)

1. 尋找並選取所需的值。

   ![](assets/routing-7.png)

1. 選取所有所需值時，按一下[儲存]。****

   ![](assets/routing-8.png)

## 帳戶路由 {#account-routing}

識別並上傳您的目標帳戶與個別銷售負責人，並將來自這些帳戶的訪客直接路由至個別帳戶負責人。

![](assets/routing-9.png)

### 新增帳戶 {#add-an-account}

在此範例中，我們會直接將所有員工從樂高路由到代理程式Steven。

1. 在[帳戶路由]索引標籤中，按一下[**+新增帳戶**]。

   ![](assets/routing-10.png)

   >[!TIP]
   >
   >您可以按一下&#x200B;**上傳帳戶清單**&#x200B;並上傳CSV，一次建立多個帳戶。

1. 輸入公司名稱、網域，然後選取所需的代理程式。

   ![](assets/routing-11.png)
