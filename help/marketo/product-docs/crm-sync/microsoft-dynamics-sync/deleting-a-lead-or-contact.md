---
unique-page-id: 45417322
description: 刪除銷售機會或連絡人 — Marketo檔案 — 產品檔案
title: 刪除銷售機會或聯繫人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 刪除銷售機會或聯繫人 {#deleting-a-lead-or-contact}

在Microsoft Dynamics中刪除銷售機會/聯絡人時，有一些需知。

* Marketo不會因為Dynamics中刪除了銷售機會而自動刪除人員。 而是將欄位「Microsoft已刪除」標幟設為true。 您可以視需要觸發此欄位以刪除Marketo中的記錄。

* 「刪除人員」流程操作：這只會刪除Marketo中的人員（不提供在Dynamics中也刪除人員的選項）。

* 如果銷售機會在Marketo中刪除（但在Dynamics中不刪除），之後在Dynamics中更新，則會在Marketo中建立新人員（相同的電子郵件地址、新人員ID）。

* 如果在Dynamics中刪除銷售機會(但在Marketo中不刪除)，然後再透過「將人員同步至Microsoft」流程動作執行，則會在Dynamics中建立新銷售機會。
