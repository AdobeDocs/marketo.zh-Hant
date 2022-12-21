---
unique-page-id: 2950578
description: 管理社交設定檔資料 — Marketo檔案 — 產品檔案
title: 管理社交設定檔資料
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 5%

---

# 管理社交設定檔資料 {#manage-social-profile-data}

有人與Marketo互動時 [社交應用程式](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)，或授權其社交網路以預填Marketo表單 [社交表單填寫](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md),Marketo會從其社交設定檔中擷取所有可用資料。 您可以在 [人員詳細資訊頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)，或將其新增為 [智慧清單的自訂檢視](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

社交表單填寫與社交應用程式會擷取稍微不同的欄位集；請參閱下方各節的相關內容。

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請連絡您的銷售代表。

## 透過社交應用程式擷取 {#captured-via-social-app}

系統會根據網路和使用者的隱私權設定，擷取以下一或多個欄位：

>[!NOTE]
>
>來自社交網路的其他資訊會在人員授權後大約5分鐘出現在「人員詳細資訊」頁面上。

## 從Twitter: {#from-twitter}

* 名字（從顯示名字剖析）
* 姓氏（從顯示名稱剖析）
* 個人資料照片URL
* 設定檔頁面URL
* 社交觸及（追隨者人數）

>[!NOTE]
>
>社交應用程式不會擷取人員的電子郵件地址。

## 從Facebook: {#from-facebook}

* 名字
* 姓氏
* 設定檔URL
* 個人資料照片URL
* 性別
* 社交觸及（朋友人數）

### 透過社交表單填寫擷取 {#captured-via-social-form-fill}

系統會根據網路和使用者的隱私權設定，擷取以下一或多個欄位：

>[!CAUTION]
>
>由社交表單擷取的資料會填寫相符的欄位，除非您 [封鎖對表單層級欄位的更新](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## 從Twitter: {#from-twitter-1}

* 名字（從顯示名字剖析）
* 姓氏（從顯示名稱剖析）
* 電子郵件

## 從Facebook: {#from-facebook-1}

* 名字
* 姓氏
* 電子郵件
* 出生日期
* 職稱
* 公司

>[!NOTE]
>
>社交表單填入會擷取電子郵件地址 _僅限_ 如果該人在表單中輸入。 如果您需要電子郵件地址，您應 [在表單中設為必填欄位](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>若要從表單中擷取此資訊，請啟用 [社交表單填寫](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
