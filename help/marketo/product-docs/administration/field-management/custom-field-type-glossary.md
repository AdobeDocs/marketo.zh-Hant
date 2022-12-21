---
unique-page-id: 2951259
description: 自訂欄位類型字彙表 — Marketo檔案 — 產品檔案
title: 自訂欄位類型字彙表
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 1%

---

# 自訂欄位類型字彙表 {#custom-field-type-glossary}

在Marketo中建立自訂欄位時，您有要選擇的類型清單。

>[!PREREQUISITES]
>
>[在Marketo中建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>視欄位類型而定，篩選/觸發 [運算子](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) 會不同。

>[!NOTE]
>
>大部分欄位不會以字元數為上限，而是以位元組數為上限。 因此，我們無法為每個欄位提供明確的字元限制。 例外是 **字串**，最大值為255個字元。

## 布林值 {#boolean}

**範例名稱：** 是客戶 — 將您的人員標籤為客戶

**範例值：** True（已勾選）/ False（未勾選）

**運算子**:無

## 貨幣 {#currency}

**範例名稱：** 預算 — 儲存公司預算的數字值

**範例值：** 100

**運算子**:是，不是，介於，大於，小於，至少，是空的，不是空的

## 日期 {#date}

**範例名稱：** 續訂日期 — 儲存客戶續訂日期

**範例值：** 8/19/14

**運算子**:是，不是，在以前，在以前，在將來，在以後，在時間範圍內，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，是空的

## 日期時間 {#datetime}

**範例名稱：** 建立日期 — 儲存建立人員的日期和時間

**範例值：** 8/19/14 2:00

**運算子**:是，不是，在以前，在以前，在將來，在以後，在時間範圍內，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，在之前，是空的

## 電子郵件 {#email}

**範例名稱：** 備用電子郵件 — 為您的人員保留備用電子郵件地址（實際上無法像預設電子郵件地址欄位那樣向此欄位發送電子郵件，該欄位是特殊的）

**範例值：** name@company.com

**運算子**:is, not, starts with, not starts with, contains, not contains, is empty, is not empty

## 浮點數 {#float}

**範例名稱：** 級別點平均值 — 保留人員的級別點平均值或具有小數的任何其他數值

**範例值：** 2.47

**運算子**:介於，大於，小於，至少，最多為空，不是空

## 公式 {#formula}

**範例名稱：** 稱呼 — 在 [獲得正確稱呼的解決方案](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) 基於性別

**範例值：** 檢查連結的解決方案

## 整數 {#integer}

**範例名稱：** 員工人數 — 儲存不需要小數的數值

**範例值：** 600

**運算子**:是，不是，介於，大於，小於，至少，是空的，不是空的

## 百分比 {#percent}

**範例名稱：** 可能購買 — 儲存百分比值（可能是在CRM端計算）

**範例值：** 85%

**運算子**:是，不是，介於，大於，小於，至少，是空的，不是空的

## 電話 {#phone}

**範例名稱：** 備用電話 — 為您的人員儲存附加電話號碼

**範例值：** 650-555-5555

**運算子**:is, not, starts with, not starts with, contains, not contains, is empty, is not empty

## 分數 {#score}

**範例名稱：** 行為分數/人口統計分數 — 建立多個分數欄位以追蹤不同屬性。

**範例值：** 14

**運算子**:是，不是，介於，大於，小於，至少，是空的，不是空的

## 字串 {#string}

**範例名稱：** 中間名稱 — 儲存附加文本屬性

**範例值：** 玫瑰

**運算子**:is, not, starts with, not starts with, contains, not contains, is empty, is not empty

## 文字區域 {#text-area}

**範例名稱：** 備注 — 在表單中新增備注欄位，以允許多行文字輸入

**範例值：** 這篇文章真棒！

**運算子**:is, not, starts with, not starts with, contains, not contains, is empty, is not empty

## URL {#url}

**範例名稱：** 部落格 — 建立欄位以儲存人員部落格url

**範例值：** www.myblog.com

**運算子**:is, not, starts with, not starts with, contains, not contains, is empty, is not empty
