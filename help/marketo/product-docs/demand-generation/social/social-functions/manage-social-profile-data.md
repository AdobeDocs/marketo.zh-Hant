---
unique-page-id: 2950578
description: 管理 Social 設定檔資料 - Marketo 檔 - 產品檔
title: 管理 Social 設定檔數據
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 5%

---

# 管理 Social 設定檔數據 {#manage-social-profile-data}

當有人與 Marketo [社交應用程式](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)互動，或授權其社交網路用社交表單填充](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)預[填充 Marketo 表單時，Marketo 會從其社交設定檔中捕獲所有可用數據。您可以在[個人詳細資料頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)上檢視此資訊，或將其新增為智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md)的[自訂檢視中的資料行。

>[!IMPORTANT]
>
>自2024年7月31日起，我們開始淘汰此功能的程式。 您將無法建立新資產。 現有資產將持續運作至2025年1月31日。 [了解更多](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

社交表單填寫和社交應用程式擷取略微不同的欄位集；請參閱以下每個欄位的區段。

>[!AVAILABILITY]
>
>並非所有Marketo Engage使用者都已購買此功能。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

## 透過社交應用程式擷取 {#captured-via-social-app}

根據網路和使用者的隱私權設定，系統會擷取以下一或多個欄位：

>[!NOTE]
>
>來自社交網路的其他資訊會在人員授權後大約五分鐘顯示在「人員詳細資訊」頁面上。

## 來自 Twitter： {#from-twitter}

* 名稱（從顯示名稱解析）
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
* 配置檔URL
* 個人資料照片URL
* 性別
* 社交觸及（好友數量）

### 已透過社交表單填寫擷取 {#captured-via-social-form-fill}

根據網路和使用者的隱私權設定，系統會擷取以下一或多個欄位：

>[!CAUTION]
>
>社交表單填入所擷取的資料會覆寫相符的欄位，除非您[封鎖表單層級](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md)這些欄位的更新。

## 從Twitter： {#from-twitter-1}

* 名字（從顯示名稱剖析）
* 姓氏（從顯示名稱剖析）
* 電子郵件

## 從臉書： {#from-facebook-1}

* 名字
* 姓氏
* 電子郵件
* 出生日期
* 職稱
* 公司

>[!NOTE]
>
>社交表單填入僅擷取電子郵件地址&#x200B;__ （如果有人在表單中輸入）。 如果您需要電子郵件地址，您應該[在表單中將其設為必要欄位](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)。

>[!MORELIKETHIS]
>
>若要從表單擷取此資訊，請啟用[社交表單填入](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)。
