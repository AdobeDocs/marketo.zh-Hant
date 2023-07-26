---
description: 將新管理員連線至Marketo - Marketo檔案 — 產品檔案
title: 連線新管理員至Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 連線新管理員至Marketo {#connect-new-admin-to-marketo}

如果其他管理員已連線至Marketo，他們只需執行步驟1。

如果第二個管理員未以管理員身分連線至Marketo...

1. 主要管理員需要從「設定> Marketo >使用者存取」中斷第二位管理員與Marketo的連線。

1. 次要管理員登入其MSC帳戶，前往「設定> Marketo」，然後按一下 **連線**.

1. 現在，次要使用者以管理員身分連線至Marketo。

1. 主要管理員現在可以登入並從Marketo中斷連線。

>[!NOTE]
>
>只要使用者B在使用者A中斷連線之前以管理員身分連線，其他使用者就會維持連線。

## 更新您的Marketo連線 {#update-your-marketo-connection}

如果您決定要移除設定Marketo整合的管理員，請參閱本文以瞭解如何進行。

Marketo整合會繫結至Sales Connect/Actions管理員使用者。 通常，這是先按一下Marketo連線頁面上的「連線」按鈕並建立連線的管理員。

若要移除建立Marketo連線的管理員，必須先由其他管理員使用者建立新連線。 我們已列出以下需要完成才能完成的工作。

為了簡化指示，我們會將目前連線的管理員稱為管理員A，並將您要建立與Marketo的新連線的管理員稱為管理員B：

1. 管理員A （目前連線的管理員）需要從管理員B （新管理員）中移除與Marketo整合的存取權。

1. 請管理員B （新管理員）建立與Marketo的新連線。

1. 中斷Admin A連線（原本連線的Admin）。

>[!NOTE]
>
>負責Marketo整合的原始管理員會看到「中斷連線」選項，該選項可在導覽至Marketo整合頁面時點選。 其他管理員（尚未建立連線）則不會。 此外，已授予Marketo整合存取權的管理員將無法按一下「連線」，這就是為什麼您必須先依照步驟移除整合存取權的原因。

**從管理員B中移除Marketo存取權**

管理員A （最初負責連線的管理員）應遵循下列步驟。

1. 在網頁應用程式中，按一下齒輪圖示並選取 **設定**.

1. 按一下 **Marketo**.

1. 按一下 **使用者存取**.

1. 搜尋您要為其建立新Marketo連線的管理員。

1. 移除存取權。

**建立管理員B的新連線**

管理員B （新管理員）應完成這些步驟

1. 在網頁應用程式中，按一下齒輪圖示並選取 **設定**.

1. 按一下 **Marketo**.

1. 按一下 **中斷連線**.

**中斷管理員A的Marketo整合**

管理員A （原本連線的管理員）應完成這些步驟。

1. 在網頁應用程式中，按一下齒輪圖示並選取 **設定**.

1. 按一下 **Marketo**.

1. 按一下 **中斷連線**.

現在，新的管理員已建立與Marketo的連線，且原始管理員已中斷連線，可以安全地從Sales Connect/Actions執行個體移除原始連線的管理員。
