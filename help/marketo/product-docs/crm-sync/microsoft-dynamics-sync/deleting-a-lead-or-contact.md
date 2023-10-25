---
unique-page-id: 45417322
description: 刪除銷售機會或連絡人 — Marketo檔案 — 產品檔案
title: 刪除潛在客戶或連絡人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 刪除潛在客戶或連絡人 {#deleting-a-lead-or-contact}

關於刪除Microsoft Dynamics中的銷售機會/聯絡人，有幾件事需要知道。

* Marketo Engage不會因為潛在客戶已在Dynamics中刪除而自動刪除人員。 而是欄位「Microsoft已刪除」標幟設為true。 如有需要，您可以觸發此欄位以刪除Marketo中的記錄。

* 「刪除人員」流程動作：這只會刪除Marketo中的人員（也無法在Dynamics中使用刪除人員的選項）。

* 如果銷售機會在Marketo中刪除（但不在Dynamics中），並在之後在Dynamics中更新，則會在Marketo中建立新的人員（相同的電子郵件地址、新的人員ID）。

* 如果在Dynamics中刪除銷售機會(但不在Marketo中)，然後透過「將人員同步至Microsoft」流程動作執行，則會在Dynamics中建立新的銷售機會。
