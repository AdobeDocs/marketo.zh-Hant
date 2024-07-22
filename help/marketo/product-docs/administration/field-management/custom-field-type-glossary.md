---
unique-page-id: 2951259
description: 自訂欄位型別字彙表 — Marketo檔案 — 產品檔案
title: 自訂欄位型別字彙表
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 2%

---

# 自訂欄位型別字彙表 {#custom-field-type-glossary}

在Marketo中建立自訂欄位時，您有一份型別清單可供選擇。

>[!PREREQUISITES]
>
>[在Marketo中建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>根據欄位型別，篩選器/觸發程式[運運算元](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md)將會不同。

>[!NOTE]
>
>大部分欄位不會以字元數為上限，而是以位元組數為上限。 因此，我們無法為每個欄位提供最終的字元限制。 例外狀況是&#x200B;**字串**，最大為255個字元。

## 布林值 {#boolean}

**範例名稱：**&#x200B;為Customer — 將您的人員標籤為客戶

**範例值：** True （已核取） / False （未核取）

**運運算元**：無

## 貨幣 {#currency}

**範例名稱：** Budget — 儲存公司預算的數值

**範例值：** 100

**運運算元**： is、is、not、between、greater than、less、最多、empty，不是空的

## 日期 {#date}

**範例名稱：**&#x200B;續約日期 — 儲存客戶的續約日期

**範例值：** 8/19/14

**運運算元**： is、is、not、between、past before、future、future before、in time frame、after、before、on或after、on或before是空的，不是空的

## 日期時間 {#datetime}

**範例名稱：**&#x200B;建立日期 — 儲存建立人員的日期和時間

**範例值：** 8/19/14 2:00

**運運算元**： is、is、not、between、past before、future、future before、in time frame、after、before、on或after、on或before是空的，不是空的

## 電子郵件 {#email}

**範例名稱：**&#x200B;備用電子郵件 — 為您的人員保留備用電子郵件地址（實際上無法像預設電子郵件位址列位那樣向此欄位傳送電子郵件，此欄位是特殊的）

**範例值：** name@company.com

**運運算元**： is、is、not、starts with、not starts with、contains、not contains、is empty、not empty

## 浮點數 {#float}

**範例名稱：**&#x200B;評分點平均值 — 保留個人的評分點平均值或任何其他有小數點的數值

**範例值：** 2.47

**運運算元**：介於、大於、小於、至少是空的，不是空的

## 公式 {#formula}

**範例名稱：**&#x200B;稱呼 — 在[解決方案中使用此特殊欄位以取得基於性別的正確稱呼](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md)

**範例值：**&#x200B;檢查連結的解決方案

## 整數 {#integer}

**範例名稱：**&#x200B;員工人數 — 儲存不需要小數的數值

**範例值：** 600

**運運算元**： is、is、not、between、greater than、less、最多、empty，不是空的

## 百分比 {#percent}

**範例名稱：**&#x200B;可能購買 — 儲存百分比值（可能在CRM端計算）

**範例值：** 85%

**運運算元**： is、is、not、between、greater than、less、最多、empty，不是空的

## 電話 {#phone}

**範例名稱：**&#x200B;備用電話 — 為您的人員儲存額外的電話號碼

**範例值：** 650-555-5555

**運運算元**： is、is、not、starts with、not starts with、contains、not contains、is empty、not empty

## 分數 {#score}

**範例名稱：**&#x200B;行為分數/人口統計分數 — 建立多個分數欄位以追蹤不同的屬性

**範例值：** 14

**運運算元**： is、is、not、between、greater than、less、最多、empty，不是空的

## 字串 {#string}

**範例名稱：**&#x200B;中間名 — 儲存額外的文字屬性

**範例值：** Rose

**運運算元**： is、is、not、starts with、not starts with、contains、not contains、is empty、not empty

## 文字區域 {#text-area}

**範例名稱：**&#x200B;註解 — 新增註解欄位至您的表單以允許多行文字輸入

**範例值：**&#x200B;這篇文章太棒了！

**運運算元**： is、is、not、starts with、not starts with、contains、not contains、is empty、not empty

## URL {#url}

**範例名稱：**&#x200B;部落格 — 建立欄位以儲存個人部落格url

**範例值：** www.myblog.com

**運運算元**： is、is、not、starts with、not starts with、contains、not contains、is empty、not empty
