---
unique-page-id: 2950578
description: 管理社交設定檔資料——行銷檔案——產品檔案
title: 管理社交設定檔資料
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---


# 管理社交設定檔資料 {#manage-social-profile-data}

當某人與Marketo社交應用程式互動 [，或授權其社交網路以預先填入Marketo表格並填入](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)Social表格時 [](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md),Marketo會擷取其社交個人檔案中的所有可用資料。 您可以在「人員詳細資訊」頁 [面上查看此資訊](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)，或將其作為列添加到智 [能清單的自定義視圖中](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

社交表單填寫和社交應用程式會擷取略有不同的欄位集；請參閱以下各節。

>[!NOTE]
>
>**可用性**
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請洽詢您的銷售代表。

## 透過社交應用程式擷取 {#captured-via-social-app}

根據網路和用戶的隱私權設定，將檢索以下一個或多個欄位：

>[!NOTE]
>
>來自社交網路的其他資訊會在人員授權後大約5分鐘內顯示在「人員詳細資料」頁面上。

## 從Twitter: {#from-twitter}

* 名字（從顯示名稱解析）
* 姓氏（從顯示名稱解析）
* 簡介像片URL
* 描述檔頁面URL
* 社交觸及（追隨者人數）

>[!NOTE]
>
>社交應用程式不會擷取該人員的電子郵件地址。

## 來自Facebook: {#from-facebook}

* 名字
* 姓氏
* 描述檔URL
* 簡介像片URL
* 性別
* 社交觸及面（朋友人數）

### 透過社交表單填寫擷取 {#captured-via-social-form-fill}

根據網路和用戶的隱私權設定，將檢索以下一個或多個欄位：

>[!CAUTION]
>
>社交表單填寫擷取的資料會覆寫相符的欄位，除非您 [封鎖表單層級上這些欄位的更新](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)。

## 從Twitter: {#from-twitter-1}

* 名字（從顯示名稱解析）
* 姓氏（從顯示名稱解析）
* 電子郵件

## 來自Facebook: {#from-facebook-1}

* 名字
* 姓氏
* 電子郵件
* 出生日期
* 職稱
* 公司

>[!NOTE]
>
>社交表單填寫只會在 *人員* 在表單中輸入時擷取電子郵件地址。 如果您需要電子郵件地址，您應 [該在表單中將其設為必填欄位](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md)。

>[!MORELIKETHIS]
>
>若要從表單擷取此資訊，請啟用社 [交表單填寫](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)。

>[!NOTE]
>
>**深入探討**
>
>進一步瞭解如何在 [Forms中深入探討使用表格](http://docs.marketo.com/display/docs/forms) 。

