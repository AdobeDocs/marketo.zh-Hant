---
unique-page-id: 45417322
description: 刪除潛在客戶或聯繫人-Marketo文檔——產品文檔
title: 刪除銷售線索或聯繫人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 刪除銷售線索或聯繫人{#deleting-a-lead-or-contact}

在Microsoft Dynamics中刪除潛在客戶／聯絡人時，有些事要知道。

* Marketo不會因為Dynamics中刪除了銷售線索而自動刪除人員。 而是將「Microsoft is Deleted」欄位標幟設為true。 您可以觸發此欄位，視需要刪除Marketo的記錄。

* 「刪除人員」流程操作：這只會刪除Marketo的人員（在Dynamics中也不提供刪除他們的選項）。

* 如果銷售線索在Marketo（但在Dynamics中不是）被刪除，之後在Dynamics中更新，則會在Marketo建立新人員（相同的電子郵件地址、新人員ID）。

* 如果Dynamics(但不是在Marketo)中刪除銷售線索，然後透過「將人員同步至Microsoft」流動動作執行，則會在Dynamics中建立新的銷售線索。
