---
unique-page-id: 45417322
description: 刪除銷售機會或連絡人 — Marketo檔案 — 產品檔案
title: 刪除商機或聯絡人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 6%

---

# 刪除商機或聯絡人 {#deleting-a-lead-or-contact}

關於刪除[!DNL Microsoft Dynamics]中的銷售機會/聯絡人，有幾件事需要知道。

* Marketo不會因為潛在客戶已在[!DNL Dynamics]中刪除而自動刪除人員。 而是欄位「Microsoft已刪除」標幟設為true。 如有需要，您可以觸發此欄位以刪除Marketo中的記錄。

* 「刪除人員」流程動作：這只會刪除Marketo中的人員（也無法在Dynamics中使用刪除人員的選項）。

* 如果銷售機會在Marketo中刪除（但不在[!DNL Dynamics]中），並在之後在[!DNL Dynamics]中更新，則會在Marketo中建立新的人員（相同的電子郵件地址、新的人員ID）。

* 如果銷售機會在[!DNL Dynamics] (但不在Marketo中)中被刪除，然後透過「將人員同步到Microsoft」流程動作執行，它將在[!DNL Dynamics]中建立新的銷售機會。
