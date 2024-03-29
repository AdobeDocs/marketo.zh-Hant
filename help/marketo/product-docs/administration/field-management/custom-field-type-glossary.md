---
unique-page-id: 2951259
description: 自訂欄位型別字彙表 — Marketo檔案 — 產品檔案
title: 自訂欄位型別字彙表
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# 自訂欄位型別字彙表 {#custom-field-type-glossary}

在Marketo中建立自訂欄位時，您有一份型別清單可供選擇。

>[!PREREQUISITES]
>
>[在Marketo中建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>根據欄位型別，篩選/觸發 [運運算元](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) 將會不同。

>[!NOTE]
>
>大部分欄位不會以字元數為上限，而是以位元組數為上限。 因此，我們無法為每個欄位提供最終的字元限制。 例外情況是 **字串**，最多可包含255個字元。

## 布林值 {#boolean}

**範例名稱：** 是否為客戶 — 將您的人員標籤為客戶

**範例值：** True （已核取） / False （未核取）

**運運算元**：無

## 貨幣 {#currency}

**範例名稱：** 預算 — 儲存公司預算的數值

**範例值：** 100

**運運算元**：是、不是、介於、大於、小於、至少、最多、空白、不是空白

## 日期 {#date}

**範例名稱：** 續約日期 — 儲存客戶的續約日期

**範例值：** 19/14/8/19

**運運算元**：是、不是、介於、過去、之前、將來、將來、之後、時間範圍內、之後、之前、或之後、在或之前、空白，不是空白

## 日期時間 {#datetime}

**範例名稱：** 建立日期 — 儲存建立人員的日期和時間

**範例值：** 2014年8月19日2:00

**運運算元**：是、不是、介於、過去、之前、將來、將來、之後、時間範圍內、之後、之前、或之後、在或之前、空白，不是空白

## 電子郵件 {#email}

**範例名稱：** 備用電子郵件 — 為您的人員保留備用電子郵件地址（實際上無法像預設電子郵件位址列位那樣向此欄位傳送電子郵件，此欄位是特殊的）

**範例值：** name@company.com

**運運算元**：是、不是、開頭為、開頭為、包含、不包含、空白、不空白

## 浮點數 {#float}

**範例名稱：** 薪等點平均 — 保留個人的薪等點平均，或其他有小數點的數值

**範例值：** 2.47

**運運算元**：介於、大於、小於、最少、空白、不是空白

## 公式 {#formula}

**範例名稱：** 問候語 — 在 [取得正確稱呼的解決方案](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) 根據性別

**範例值：** 檢查連結的解決方案

## 整數 {#integer}

**範例名稱：** 員工人數 — 儲存不需要小數的數值

**範例值：** 600

**運運算元**：是、不是、介於、大於、小於、至少、最多、空白、不是空白

## 百分比 {#percent}

**範例名稱：** 可能購買 — 儲存百分比值（可能在CRM端計算）

**範例值：** 85%

**運運算元**：是、不是、介於、大於、小於、至少、最多、空白、不是空白

## 電話 {#phone}

**範例名稱：** 備用電話 — 為您的人員儲存額外的電話號碼

**範例值：** 650-555-5555

**運運算元**：是、不是、開頭為、開頭為、包含、不包含、空白、不空白

## 分數 {#score}

**範例名稱：** 行為分數/人口統計分數 — 建立多個分數欄位以追蹤不同屬性

**範例值：** 14

**運運算元**：是、不是、介於、大於、小於、至少、最多、空白、不是空白

## 字串 {#string}

**範例名稱：** 中間名 — 儲存額外的文字屬性

**範例值：** 玫瑰

**運運算元**：是、不是、開頭為、開頭為、包含、不包含、空白、不空白

## 文字區域 {#text-area}

**範例名稱：** 註解 — 在表單中新增註解欄位，以允許多行文字輸入

**範例值：** 這篇文章真是棒極了！

**運運算元**：是、不是、開頭為、開頭為、包含、不包含、空白、不空白

## URL {#url}

**範例名稱：** 部落格 — 建立欄位以儲存個人部落格url

**範例值：** www.myblog.com

**運運算元**：是、不是、開頭為、開頭為、包含、不包含、空白、不空白
