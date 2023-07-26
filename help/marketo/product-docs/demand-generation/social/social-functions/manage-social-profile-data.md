---
unique-page-id: 2950578
description: 管理社交設定檔資料 — Marketo檔案 — 產品檔案
title: 管理社交設定檔資料
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 5%

---

# 管理社交設定檔資料 {#manage-social-profile-data}

有人與Marketo互動時 [社交應用程式](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)，或授權其社交網路使用預先填入Marketo表單 [社交表單填寫](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)，Marketo會擷取其社交設定檔中的所有可用資料。 您可以在 [個人詳細資訊頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)，或將其新增為中的欄 [智慧清單的自訂檢視](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

社交表單填寫和社交應用程式擷取略微不同的欄位集；請參閱以下每個欄位的區段。

>[!AVAILABILITY]
>
>並非所有客戶都已購買此功能。 請聯絡您的銷售代表以取得詳細資訊。

## 透過社交應用程式擷取 {#captured-via-social-app}

根據網路和使用者的隱私權設定，系統會擷取以下一或多個欄位：

>[!NOTE]
>
>來自社交網路的其他資訊會在人員授權後約五分鐘出現在「人員詳細資訊」頁面上。

## 從Twitter： {#from-twitter}

* 名字（從顯示名稱剖析）
* 姓氏（從顯示名稱剖析）
* 設定檔像片URL
* 設定檔頁面URL
* 社交觸及（關注者數量）

>[!NOTE]
>
>社交應用程式不會擷取使用者的電子郵件地址。

## 從Facebook： {#from-facebook}

* 名字
* 姓氏
* 設定檔URL
* 設定檔像片URL
* 性別
* 社交觸及（好友數量）

### 已透過社交表單填寫擷取 {#captured-via-social-form-fill}

根據網路和使用者的隱私權設定，系統會擷取以下一或多個欄位：

>[!CAUTION]
>
>社交表單填入所擷取的資料會覆寫相符的欄位，除非您 [封鎖表單層級這些欄位的更新](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## 從Twitter： {#from-twitter-1}

* 名字（從顯示名稱剖析）
* 姓氏（從顯示名稱剖析）
* 電子郵件

## 從Facebook： {#from-facebook-1}

* 名字
* 姓氏
* 電子郵件
* 出生日期
* 職稱
* 公司

>[!NOTE]
>
>社交表單填寫會擷取電子郵件地址 _僅限_ 如果人員以表單輸入。 如果您需要電子郵件地址，請 [將其設為表單中的必填欄位](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>若要從表單擷取此資訊，請啟用 [社交表單填寫](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
