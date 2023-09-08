---
description: 路由 — Marketo檔案 — 產品檔案
title: 路由
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: ea9e02d9ad52991757f137c7c2b549b98f139ba5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 1%

---

# 路由 {#routing}

以Dynamic Chat預約的會議可以兩種方式傳送。 循環配置資源，或使用自訂規則。

循環配置資源：會議會依序指派給代理程式。 因此，如果您有五個代理程式，而代理程式三參加最後一個會議，則代理程式四會取得下一個會議，接著是代理程式五，然後回到代理程式一。

自訂規則：您可以根據您選取的屬性選擇特定代理以接收會議。

## 建立自訂規則 {#create-a-custom-rule}

在此範例中，我們會將推斷的CA、OR和WA狀態的所有會議傳送給代理程式John。

1. 在Dynamic Chat中選取 **路由**.

   ![](assets/routing-1.png)

1. 按一下 **自訂規則** 標籤。

   ![](assets/routing-2.png)

1. 按一下 **建立規則**.

   ![](assets/routing-3.png)

1. 為規則命名，然後按一下 **下一個**.

   ![](assets/routing-4.png)

1. 選擇所需的代理程式。

   ![](assets/routing-5.png)

1. 拖曳到您所需的屬性上。

   ![](assets/routing-6.png)

1. 尋找並選取所需的值。

   ![](assets/routing-7.png)

1. 選取所有所需值時，按一下 **儲存**.

   ![](assets/routing-8.png)
