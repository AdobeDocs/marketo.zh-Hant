---
unique-page-id: 4719314
description: 預設Salesforce欄位對應-Marketo檔案——產品檔案
title: 預設Salesforce欄位對應
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 33%

---

# 預設Salesforce欄位對應{#default-salesforce-field-mapping}

當您最初將Marketo帳戶與Salesforce同步時，Marketo會自動在您內建的Salesforce和Marketo欄位之間建立這些關聯。 Marketo還將同步您的Lead、Accounts、Opportunity和Contacts上的自定義欄位。

## 銷售線索欄位{#lead-fields}

| SFDC欄位 | Marketo田 |
|---|---|
| 年營業額 | 年營業額 |
| 城市 | 城市 |
| 公司 | 公司名稱 |
| 轉換日期 | SFDC轉換日期 |
| 國家 | 國家 |
| 建立日期 | SFDC建立日期 |
| 說明 | 人員附註 |
| 電子郵件 | 電子郵件地址 |
| 傳真 | 傳真號碼 |
| 名字 | 名字 |
| 選擇退出電子郵件 | 退訂 |
| 行業 | 行業 |
| 已轉換 | 轉換SFDC |
| 已刪除 | 已刪除SFDC |
| 姓氏 | 姓氏 |
| 潛在客戶來源 | 來源 |
| 潛在客戶分數 | 分數 |
| 行動電話 | 手機號碼 |
| 員工 | 員工數 |
| 電話 | 電話號碼 |
| 郵遞區號 | 郵遞區號 |
| 評分 | 評分 |
| 稱謂 | 稱謂 |
| 州／省 | 州 |
| 狀態 | 狀態 |
| 街道 | 地址 |
| 標題 | 職稱 |
| 網站 | 網站 |

## 連絡人欄位{#contact-fields}

| SFDC欄位 | Marketo田 |
|---|---|
| 出生日期 | 出生日期 |
| 建立日期 | SFDC建立日期 |
| 連絡人說明 | 人員附註 |
| 電子郵件 | 電子郵件地址 |
| 企業傳真 | 傳真號碼 |
| 名字 | 名字 |
| 選擇退出電子郵件 | 退訂 |
| 已刪除 | 已刪除SFDC |
| 姓氏 | 姓氏 |
| 潛在客戶來源 | 來源 |
| 潛在客戶分數 | 分數 |
| MailingCity | 城市 |
| MailingCountry | 國家 |
| 郵遞區號 | 郵遞區號 |
| MailingState | 州 |
| MailingStreet | 地址 |
| 行動電話 | 手機號碼 |
| 商務電話 | 電話號碼 |
| 稱謂 | 稱謂 |
| 標題 | 職稱 |

## 帳戶欄位{#account-fields}

| SFDC欄位 | Marketo田 |
|---|---|
| 年營業額 | 年營業額 |
| 帳單寄送城市 | 帳單寄送城市 |
| 帳單寄送國家 | 帳單寄送國家 |
| 帳單郵遞區號 | 帳單郵遞區號 |
| 帳單州／省 | 帳單寄送州 |
| 帳單街 | 帳單寄送地址 |
| 帳戶說明 | 公司說明 |
| 行業 | 行業 |
| 已刪除 | 已刪除SFDC |
| 帳戶名稱 | 公司名稱 |
| 員工 | 員工數 |
| 帳戶電話 | 主要電話 |
| 標準產業分類（SIC）代碼 | 標準產業分類（SIC）代碼 |
| 帳戶網站 | 現場 |
| 帳戶類型 | SFDC類型 |
| 網站 | 網站 |

## Marketo的Salesforce相關系統欄位（唯讀）{#salesforce-related-system-fields-in-marketo-read-only}

這些欄位是在Marketo建立，但客戶無法調整。

| 欄位 | 說明 |
|---|---|
| SFDC ID | 18個字元的Salesforce Id |
| SFDC類型 | 潛在客戶或聯絡人。 如果空，則銷售線索僅作為人存在於Marketo |
| SFDC建立日期 | 在SFDC中建立的日期(可以與在Marketo中建立的日期不同) |
| 已刪除SFDC | 以前在SFDC的人被刪除，現在只住在Marketo |
