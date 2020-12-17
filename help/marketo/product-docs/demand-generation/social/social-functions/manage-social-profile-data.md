---
unique-page-id: 2950578
description: 管理社交設定檔資料——行銷檔案——產品檔案
title: 管理社交設定檔資料
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# 管理社交設定檔資料{#manage-social-profile-data}

當某人與Marketo [社交應用程式](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)互動，或授權其社交網路以[社交表單fill](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)預先填入Marketo表單時，Marketo會擷取其社交設定檔中所有可用的資料。 您可以在[「人員詳細資訊」頁面](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)中查看此資訊，或將其作為[智慧清單的自定義視圖](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)中的列添加。

社交表單填寫和社交應用程式會擷取略有不同的欄位集；請參閱以下各節。

>[!NOTE]
>
>**可用性**
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請洽詢您的銷售代表。

## 透過社交應用程式擷取{#captured-via-social-app}

根據網路和用戶的隱私權設定，將檢索以下一個或多個欄位：

>[!NOTE]
>
>來自社交網路的其他資訊會在人員授權後大約5分鐘內顯示在「人員詳細資料」頁面上。

## 從Twitter:{#from-twitter}

* 名字（從顯示名稱解析）
* 姓氏（從顯示名稱解析）
* 簡介像片URL
* 描述檔頁面URL
* 社交觸及（追隨者人數）

>[!NOTE]
>
>社交應用程式不會擷取該人員的電子郵件地址。

## 來自Facebook:{#from-facebook}

* 名字
* 姓氏
* 描述檔URL
* 簡介像片URL
* 性別
* 社交觸及面（朋友人數）

### 透過社交表單填寫{#captured-via-social-form-fill}擷取

根據網路和用戶的隱私權設定，將檢索以下一個或多個欄位：

>[!CAUTION]
>
>由社交表單填寫擷取的資料會覆寫相符的欄位，除非您[區塊會更新至表單層級的欄位](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)。

## 從Twitter:{#from-twitter-1}

* 名字（從顯示名稱解析）
* 姓氏（從顯示名稱解析）
* 電子郵件

## 來自Facebook:{#from-facebook-1}

* 名字
* 姓氏
* 電子郵件
* 出生日期
* 職稱
* 公司

>[!NOTE]
>
>社交表單填寫會在人員在表單中輸入時，只擷取電子郵件地址&#x200B;**。 如果您需要電子郵件地址，您應[將它設為表單中的必填欄位。](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)

>[!MORELIKETHIS]
>
>若要從表單擷取此資訊，請啟用[社交表單fill](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)。

>[!NOTE]
>
>**深入探討**
>
>進一步瞭解如何在[Forms](http://docs.marketo.com/display/docs/forms)深入探討中使用表格。

