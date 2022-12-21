---
unique-page-id: 10095307
description: 電子郵件地址的自訂同步篩選規則 — Marketo檔案 — 產品檔案
title: 電子郵件地址的自訂同步篩選規則
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# 電子郵件地址的自訂同步篩選規則 {#custom-sync-filter-rules-for-an-email-address}

若要防止同步沒有電子郵件地址的記錄，請遵循下列規則。

* 建立銷售機會時，或更新銷售機會的電子郵件地址欄位時，檢查銷售機會是否具有電子郵件地址，如果有，請將「同步」更改為「Mkto」 **True**. 否則，請變更為 **False**

* 當建立聯繫人時，或當聯繫人的電子郵件地址欄位更新時，檢查該聯繫人是否具有電子郵件地址，如果有，請將「同步」更改為「Mkto」 **True** 並將同步更改為Mkto **True** 在帳戶記錄上。 否則，請變更為 **False**

* 更新連絡人的「公司名稱(parentcustomerid)」欄位時，請檢查連絡人的「同步至Mkto」欄位是否為true。 如果是，請將帳戶上的「同步至Mkto」變更為 **True** an
* 更新業務機會的潛在客戶（客戶ID）欄位或聯繫人(parentcontactid)時，檢查帳戶的「同步到Mkto」欄位是否為true，或聯繫人的「同步到Mkto」欄位是否為true。 如果是，請將Sync更改為Mkto ，以便 **True** an
