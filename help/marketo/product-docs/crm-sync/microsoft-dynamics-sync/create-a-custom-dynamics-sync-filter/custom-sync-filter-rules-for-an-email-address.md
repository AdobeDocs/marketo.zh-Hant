---
unique-page-id: 10095307
description: 電子郵件地址的自訂同步篩選規則 — Marketo檔案 — 產品檔案
title: 電子郵件地址的自訂同步篩選規則
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# 電子郵件地址的自訂同步篩選規則 {#custom-sync-filter-rules-for-an-email-address}

若要防止同步沒有電子郵件地址的記錄，請遵循這些規則。

* 建立潛在客戶或更新潛在客戶電子郵件位址列位時，請檢查潛在客戶是否有電子郵件地址，如果有，請將「同步」變更為Mkto **真**. 否則變更為 **假**

* 建立連絡人或更新連絡人的電子郵件位址列位時，請檢查連絡人是否有電子郵件地址，如果有，請將[同步]變更為[Mkto] **真** 並將同步處理變更為Mkto **真** 在帳戶記錄上。 否則，將變更為 **假**

* 連絡人的公司名稱(parentcustomerid)欄位更新時，請檢查連絡人的「同步至Mkto」欄位是否為true。 如果是，則將帳戶上的Sync變更為Mkto **真** 另外
* 當機會的「潛在客戶」 (customerid)欄位或「連絡人」 (parentcontactid)更新時，檢查帳戶的「同步至Mkto」欄位是否為true，或連絡人的「同步至Mkto」欄位是否為true。 如果是，請將機會上的Sync變更為Mkto，並變更為 **真** 另外
