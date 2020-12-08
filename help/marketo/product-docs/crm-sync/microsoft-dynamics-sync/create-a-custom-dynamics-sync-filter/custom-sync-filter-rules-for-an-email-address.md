---
unique-page-id: 10095307
description: 電子郵件地址的自訂同步篩選規則——行銷人員檔案——產品檔案
title: 電子郵件地址的自訂同步篩選規則
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# 電子郵件地址的自訂同步篩選規則 {#custom-sync-filter-rules-for-an-email-address}

為避免同步沒有電子郵件地址的記錄，請遵循這些規則。

* 當銷售線索建立為OR時，當銷售線索的電子郵件地址欄位更新時，請檢查銷售線索是否有電子郵件地址，如果有，請將「同步至Mkto」變更為 **True**。 否則變更為 **False**

* 當建立連絡人或更新連絡人的電子郵件地址欄位時，請檢查連絡人是否有電子郵件地址，如果有，請將「帳戶」記錄上的「同步至Mkto」變更為 **True** ，並將「同步至Mkto」變更為 **True** 。 否則，請變更為 **False**

* 當連絡人的「公司名稱」(parentcustomerid)欄位更新時，檢查連絡人的「同步至Mkto」欄位是否正確。 如果是，請將帳戶上的「同步至Mkto」變更為 **True** 。
* 當業務機會的「潛在客戶」（客戶ID）欄位或「聯絡人」（括弧）欄位更新時，請檢查帳戶的「同步至Mkto」欄位是否正確，或連絡人的「同步至Mkto」欄位是否正確。 如果是，請將機會上的「同步到Mkto」更改為 **True** 。

