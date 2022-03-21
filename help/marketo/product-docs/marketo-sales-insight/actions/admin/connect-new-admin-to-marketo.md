---
description: 將新管理員連接到Marketo-Marketo文檔 — 產品文檔
title: 將新管理員連接到Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 將新管理員連接到Marketo {#connect-new-admin-to-marketo}

如果另一個管理員已連接到Marketo，則他們只需執行步驟1。

如果第二個管理員未作為管理員連接到Marketo...

1. 主Admin需要從「設定」>「Marketo」>「用戶訪問」中斷開第二個Admin與Marketo的連接。

1. 輔助管理員登錄到其MSC帳戶，轉到「設定」>「Marketo」，然後按一下 **連接**。

1. 現在，輔助用戶已以管理員身份連接到Marketo。

1. 主管理員現在可以登錄並斷開與Marketo的連接。

>[!NOTE]
>
>只要用戶B在用戶A斷開連接之前以管理員身份連接，其他用戶將保持連接。

## 更新您的Marketo連接 {#update-your-marketo-connection}

如果您決定刪除設定Marketo整合的管理員，請查看此文章以瞭解如何。

Marketo整合將與Sales Connect/Actions Admin用戶關聯。 通常，這是管理員，他首先按一下了Marketo連接頁上的「連接」按鈕並建立了連接。

要刪除建立Marketo連接的管理員，必須先由其他管理員用戶建立新連接。 下面列出了為完成此操作需要完成的任務。

為簡化說明，我們將參考當前連接的Admin（管理員A）和您要用Admin B（管理員B）與Marketo建立新連接的Admin（管理員A）:

1. 管理員A（當前連接的管理員）需要從管理員B（新管理員）中刪除對與Marketo整合的訪問權限。

1. 讓管理員B（新管理員）建立到Marketo的新連接。

1. 斷開管理員A（最初連接的管理員）。

>[!NOTE]
>
>負責Marketo整合的原始管理員將看到一個「斷開」選項，該選項在導航到Marketo整合頁面時可按一下。 其他管理員（尚未建立連接）將不會。 此外，已獲准訪問Marketo整合的管理員將無法按一下連接，因此您必須首先執行刪除整合訪問權限的步驟。

**從管理員B中刪除Marketo訪問**

管理員A（最初負責連接的管理員）應執行以下步驟。

1. 在Web應用程式中，按一下齒輪表徵圖並選擇 **設定**。

1. 按一下 **Marketo**。

1. 按一下 **用戶訪問**。

1. 搜索要為其建立新Marketo連接的管理員。

1. 刪除訪問權限。

**為管理員B建立新連接**

這些步驟應由Admin B（新管理員）執行

1. 在Web應用程式中，按一下齒輪表徵圖並選擇 **設定**。

1. 按一下 **Marketo**。

1. 按一下 **斷開**。

**斷開管理員A的Marketo整合**

這些步驟應由管理員A（最初連接的管理員）執行。

1. 在Web應用程式中，按一下齒輪表徵圖並選擇 **設定**。

1. 按一下 **Marketo**。

1. 按一下 **斷開**。

現在，新管理員已建立到Marketo的連接，並且原管理員已斷開連接，因此可以安全地從Sales Connect/Actions實例中刪除原來連接的管理員。
