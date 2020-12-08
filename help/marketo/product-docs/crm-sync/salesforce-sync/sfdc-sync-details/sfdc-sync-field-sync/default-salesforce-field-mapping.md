---
unique-page-id: 4719314
description: 預設Salesforce欄位對應——行銷人員檔案——產品檔案
title: 預設Salesforce欄位對應
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 預設Salesforce欄位對應 {#default-salesforce-field-mapping}

當您最初將Marketo帳戶與Salesforce同步時，Marketo會自動在您內建的Salesforce和Marketo欄位之間建立這些關聯。 Marketo也會同步您的Lead、Accounts、Opportunity和Contacts上的自訂欄位。

## 銷售線索欄位 {#lead-fields}

| SFDC欄位 | Marketo欄位 |
|---|---|
| 年收入 | 年收入 |
| 城市 | 城市 |
| 公司 | 公司名稱 |
| 轉換日期 | SFDC轉換日期 |
| 國家／地區 | 國家／地區 |
| 建立日期 | SFDC建立日期 |
| 說明 | 人員附註 |
| 電子郵件 | 電子郵件地址 |
| 傳真 | 傳真號碼 |
| 名字 | 名字 |
| 選擇退出電子郵件 | 取消訂閱 |
| 產業 | 產業 |
| 已轉換 | 轉換SFDC |
| 已刪除 | 已刪除SFDC |
| 姓氏 | 姓氏 |
| 銷售線索來源 | 來源 |
| 銷售線索分數 | 分數 |
| 行動電話 | 行動電話號碼 |
| 員工 | 員工人數 |
| 電話 | 電話號碼 |
| 郵遞區號 | 郵遞區號 |
| 評分 | 評分 |
| 問候語 | 問候語 |
| 州／省 | 州 |
| 狀態 | 狀態 |
| 街道 | 地址 |
| 標題 | 職稱 |
| 網站 | 網站 |

## 連絡人欄位 {#contact-fields}

| SFDC欄位 | Marketo欄位 |
|---|---|
| 出生日期 | 出生日期 |
| 建立日期 | SFDC建立日期 |
| 連絡人說明 | 人員附註 |
| 電子郵件 | 電子郵件地址 |
| 企業傳真 | 傳真號碼 |
| 名字 | 名字 |
| 選擇退出電子郵件 | 取消訂閱 |
| 已刪除 | 已刪除SFDC |
| 姓氏 | 姓氏 |
| 銷售線索來源 | 來源 |
| 銷售線索分數 | 分數 |
| MailingCity | 城市 |
| MailingCountry | 國家／地區 |
| 郵遞區號 | 郵遞區號 |
| MailingState | 州 |
| MailingStreet | 地址 |
| 行動電話 | 行動電話號碼 |
| 商務電話 | 電話號碼 |
| 問候語 | 問候語 |
| 標題 | 職稱 |

## 帳戶欄位 {#account-fields}

| SFDC欄位 | Marketo欄位 |
|---|---|
| 年收入 | 年收入 |
| 帳單城市 | 帳單城市 |
| 帳單國家／地區 | 帳單國家／地區 |
| 帳單郵遞區號 | 帳單郵遞區號 |
| 帳單州／省 | 帳單狀態 |
| 帳單街 | 帳單地址 |
| 帳戶說明 | 公司說明 |
| 產業 | 產業 |
| 已刪除 | 已刪除SFDC |
| 帳戶名稱 | 公司名稱 |
| 員工 | 員工人數 |
| 帳戶電話 | 主手機 |
| SIC代碼 | SIC代碼 |
| 帳戶網站 | 網站 |
| 帳戶類型 | SFDC類型 |
| 網站 | 網站 |

## Marketo中與Salesforce相關的系統欄位（唯讀） {#salesforce-related-system-fields-in-marketo-read-only}

這些欄位是在Marketo中建立，但客戶無法調整。

| 欄位 | 說明 |
|---|---|
| SFDC ID | 18個字元的Salesforce Id |
| SFDC類型 | 潛在客戶或聯絡人。 如果空白，則銷售線索僅作為Marketto中的人員存在 |
| SFDC建立日期 | 在SFDC中建立的日期（可以與在Marketo中建立的日期不同） |
| 已刪除SFDC | 以前在SFDC的人員，但被刪除，現在只住在Marketo |
