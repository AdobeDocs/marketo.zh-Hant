---
unique-page-id: 2951259
description: 自訂欄位類型辭彙表-Marketo文檔——產品檔案
title: 自訂欄位類型辭彙表
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# 自定義欄位類型辭彙表{#custom-field-type-glossary}

當您在Marketo建立自訂欄位時，您有可選擇的類型清單。

>[!PREREQUISITES]
>
>[在Marketo建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>視欄位類型而定，filter/trigger [operators](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md)將不同。

>[!NOTE]
>
>大部分欄位不會以字元數為上限，而是以位元組數為上限。 因此，我們無法為每個欄位提供明確的字元限制。 例外是&#x200B;**String**，最大值為255個字元。

## 布林{#boolean}

**範例名稱：** 是客戶——將您的人員標籤為客戶

**範例值：** True（勾選）/False（未勾選）

**營運商**:無

## 貨幣{#currency}

**範例名稱：** 預算——儲存公司預算的數字值

**範例值：** 100

**營運商**:is, is not, between, greater, less than, allyst, ald mots, is empty, not empty

## 日期{#date}

**範例名稱：續** 約日期——儲存客戶續約日期

**範例值：** 8/19/14

**營運商**:is, is not is betwen, prest, power, in future, in time frame, after, after, on, of, on, of, of, of, of fer, in expty

## 日期時間{#datetime}

**範例名稱：** 建立日期——儲存建立人員的日期和時間

**範例值：** 8/19/14 2:00

**營運商**:is, is not is betwen, prest, power, in future, in time frame, after, after, on, of, on, of, of, of, of fer, in expty

## 電子郵件 {#email}

**範例名稱：** 替代電子郵件——為您的人員保留替代電子郵件地址（無法實際傳送電子郵件至此欄位，例如預設電子郵件地址欄位，此欄位為特殊）

**範例值：** name@company.com

**營運商**:is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## 浮點數{#float}

**範例名稱：** 平均分級點數——保留人員的平均分級點數，或任何其他具有小數的數值

**範例值：** 2.47

**營運商**:介於、大於、小於、至少至多為空，不是空的

## 公式{#formula}

**範例名稱：** 問候語——在解決方案中使用此特殊欄 [位，以根據性別取得](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) 正確的問候語

**範例值：檢** 查連結的解決方案

## 整數{#integer}

**範例名稱：** 員工人數——儲存不需要小數位數的數值

**範例值：** 600

**營運商**:is, is not, between, greater, less than, allyst, ald mots, is empty, not empty

## 百分比{#percent}

**範例名稱：** 可能購買——儲存百分比值（可能是在CRM端計算）

**範例值：** 85%

**營運商**:is, is not, between, greater, less than, allyst, ald mots, is empty, not empty

## 電話 {#phone}

**範例名稱：** 替代電話——為您的人員儲存額外的電話號碼

**範例值：** 650-555-5555

**營運商**:is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## 分數{#score}

**範例名稱：行** 為分數／人口統計分數——建立多個分數欄位以追蹤不同屬性。

**範例值：** 14

**營運商**:is, is not, between, greater, less than, allyst, ald mots, is empty, not empty

## 字串{#string}

**範例名稱：** 中間名稱——儲存其他文字屬性

**示例值：** Rose

**營運商**:is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## 文字區域{#text-area}

**範例名稱：** 注釋——在表單中新增注釋欄位，以允許多行文字輸入

**範例值：這** 篇文章太棒了！

**營運商**:is, is not, starts with, not starts with, contains, not contains, is empty, is not empty

## URL {#url}

**範例名稱：** 部落格——建立欄位以儲存人員部落格URL

**範例值：** www.myblog.com

**營運商**:is, is not, starts with, not starts with, contains, not contains, is empty, is not empty
