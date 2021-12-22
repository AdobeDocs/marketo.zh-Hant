---
description: 將新管理員連線至Marketo - Marketo檔案 — 產品檔案
title: 將新管理員連線至Marketo
hide: true
hidefromtoc: true
source-git-commit: 0ed5981470998dadd5f42384cd2e9572fec94ef6
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# 將新管理員連線至Marketo {#connect-new-admin-to-marketo}

如果其他管理員已連線至Marketo，則只需執行步驟1。

如果第二個管理員未以管理員身分連線至Marketo...

1. 主要管理員需從「設定> Marketo >使用者存取」中，從Marketo中斷第二名管理員的連線

1. 次要管理員登入其MSC帳戶，前往「設定> Marketo」並按一下 **Connect**.

1. 現在，次要使用者已以管理員身分連線至Marketo。

1. 主要管理員現在可登入並中斷與Marketo的連線。

>[!NOTE]
>
>只要使用者B在使用者A中斷連線前以管理員身分連線，其他使用者就會持續連線。

## 更新您的Marketo連線 {#update-your-marketo-connection}

如果您決定移除設定Marketo整合的管理員，請檢閱本文章以了解如何。

Marketo整合將系結至Sales Connect/Actions管理員使用者。 這通常是先按一下Marketo連線頁面上的「連線」按鈕並建立連線的管理員。

若要移除建立Marketo連線的管理員，必須先由其他管理員使用者建立新連線。 我們列出了以下需要完成的任務，以便執行此操作。

為了簡化指示，我們會將目前連線的管理員稱為管理員A，並將您想要以管理員B身分建立與Marketo的新連線的管理員稱為：

1. 管理員A（目前連線的管理員）需要從管理員B（新的管理員）移除與Marketo整合的存取權。

1. 請管理員B（新管理員）建立與Marketo的新連線。

1. 斷開管理員A的連接（最初連接的管理員）。

>[!NOTE]
>
>負責Marketo整合的原始管理員會看到「中斷連線」選項，導覽至Marketo整合頁面時可點按。 其他管理員（尚未建立連線）則不會。 此外，已獲得Marketo整合存取權的管理員將無法按一下「連線」，因此您必須先依照步驟移除整合的存取權。

**從管理員B移除Marketo存取權**

管理員A（原本負責連線的管理員）應遵循下列步驟。

1. 導覽至設定。

1. 按一下 **Marketo**.

1. 按一下 **使用者存取**.

1. 搜尋您要建立新Marketo連線的管理員。

1. 移除存取權。

**為管理員B建立新連線**

管理員B（新管理員）應遵循這些步驟

1. 導覽至設定。

1. 按一下 **Marketo**.

1. 按一下 **斷開連接**.

**中斷管理A的Marketo整合**

管理員A（原先連接的管理員）應遵循這些步驟

1. 導覽至設定。

1. 按一下 **Marketo**.

1. 按一下 **斷開連接**.

現在，新管理員已建立與Marketo的連線，且原始管理員已中斷連線，即可安全地從Sales Connect/Actions例項中移除原本連線的管理員。
