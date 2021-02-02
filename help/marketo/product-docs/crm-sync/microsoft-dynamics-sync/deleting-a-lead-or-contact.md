---
unique-page-id: 45417322
description: 刪除潛在客戶或聯絡人——行銷人員檔案——產品檔案
title: 刪除銷售線索或聯繫人
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# 刪除銷售線索或聯繫人{#deleting-a-lead-or-contact}

在Microsoft Dynamics中刪除潛在客戶／聯絡人時，有些事要知道。

* Marketo不會因為Dynamics中刪除了銷售機會而自動刪除人員。 而是將「Microsoft is Deleted」欄位標幟設為true。 您可以觸發此欄位，以視需要刪除Marketo中的記錄。

* 「刪除人員」流程操作：這只會刪除Marketo中的人員（在Dynamics中也不提供刪除他們的選項）。

* 如果銷售機會在Marketo中刪除（但在Dynamics中不刪除），並在Dynamics中更新，則會在Marketo中建立新人員（相同的電子郵件地址、新人員ID）。

* 如果Dynamics（但Marketo中未刪除銷售線索）中的銷售線索，然後透過「將人員同步至Microsoft」流動動作執行，則會在Dynamics中建立新的銷售線索。
