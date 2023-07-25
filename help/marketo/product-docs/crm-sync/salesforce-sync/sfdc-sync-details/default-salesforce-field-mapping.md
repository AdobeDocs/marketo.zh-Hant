---
unique-page-id: 4719314
description: 預設Salesforce欄位對應 — Marketo檔案 — 產品檔案
title: 預設Salesforce欄位對應
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 43%

---

# 預設Salesforce欄位對應 {#default-salesforce-field-mapping}

當您初次將Marketo帳戶與Salesforce同步時，Marketo會在您內建的Salesforce和Marketo欄位之間自動建立這些關聯。 Marketo也會同步處理潛在客戶、帳戶、商機和聯絡人上的自訂欄位。

## 潛在客戶欄位 {#lead-fields}

| SFDC欄位 | Marketo欄位 |
|---|---|
| 年收入 | 年收入 |
| 城市 | 城市 |
| 公司 | 公司名稱 |
| 轉換日期 | SFDC 轉換日期 |
| 國家 | 國家 |
| 建立日期 | SFDC建立日期 |
| 說明 | 個人附註 |
| 電子郵件 | 電子郵件地址 |
| 傳真 | 傳真號碼 |
| 名字 | 名字 |
| 電子郵件選擇退出 | 退訂 |
| 產業 | 產業 |
| 已轉換 | SFDC 已轉換 |
| 已刪除 | SFDC 已刪除 |
| 姓氏 | 姓氏 |
| 銷售機會來源 | 來源 |
| 銷售機會分數 | 分數 |
| 行動電話 | 手機號碼 |
| 員工 | 員工人數 |
| 電話 | 電話號碼 |
| 郵遞區號 | 郵遞區號 |
| 評等 | 評等 |
| 問候語 | 問候語 |
| 州/省 | 州別 |
| 狀態 | 狀態 |
| 街道 | 地址 |
| 標題 | 職稱 |
| 網站 | 網站 |

## 連絡人欄位 {#contact-fields}

| SFDC欄位 | Marketo欄位 |
|---|---|
| 出生日期 | 出生日期 |
| 建立日期 | SFDC建立日期 |
| 連絡人說明 | 個人附註 |
| 電子郵件 | 電子郵件地址 |
| 商務傳真 | 傳真號碼 |
| 名字 | 名字 |
| 電子郵件選擇退出 | 退訂 |
| 已刪除 | SFDC 已刪除 |
| 姓氏 | 姓氏 |
| 銷售機會來源 | 來源 |
| 銷售機會分數 | 分數 |
| 郵寄城市 | 城市 |
| 郵寄國家 | 國家 |
| 郵遞區號 | 郵遞區號 |
| MailingState | 州別 |
| 郵寄街 | 地址 |
| 行動電話 | 手機號碼 |
| 商務電話 | 電話號碼 |
| 問候語 | 問候語 |
| 標題 | 職稱 |

## 帳戶欄位 {#account-fields}

| SFDC欄位 | Marketo欄位 |
|---|---|
| 年收入 | 年收入 |
| 帳單城市 | 帳單城市 |
| 帳單國家 | 帳單國家 |
| 帳單郵遞區號 | 帳單郵遞區號 |
| 帳單州/省 | 帳單州別 |
| 帳單街道 | 帳單地址 |
| 帳戶說明 | 公司備註 |
| 產業 | 產業 |
| 已刪除 | SFDC 已刪除 |
| 帳戶名稱 | 公司名稱 |
| 員工 | 員工人數 |
| 帳戶電話 | 主要電話 |
| SIC 代碼 | SIC 代碼 |
| 帳戶網站 | 網站 |
| 帳戶型別 | SFDC 類型 |
| 網站 | 網站 |

## Marketo中的Salesforce相關系統欄位（唯讀） {#salesforce-related-system-fields-in-marketo-read-only}

這些欄位是在Marketo中建立的，但客戶無法調整。

| 欄位 | 說明 |
|---|---|
| SFDC Id | 18個字元的Salesforce Id |
| SFDC 類型 | 潛在客戶或連絡人。 如果留空，則潛在客戶只會以Marketo中的個人身分存在 |
| SFDC建立日期 | 在SFDC中建立的日期(可以與Marketo中建立的日期不同) |
| SFDC已刪除 | 此人員之前在SFDC中，但已被刪除，現在僅居住在Marketo中 |
