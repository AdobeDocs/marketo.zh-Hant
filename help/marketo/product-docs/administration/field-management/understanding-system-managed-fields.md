---
unique-page-id: 5472615
description: 瞭解系統管理欄位——行銷檔案——產品檔案
title: 瞭解系統管理欄位
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# 瞭解系統管理欄位{#understanding-system-managed-fields}

您可能注意到，[person detail page](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)包含由Marketo建立的一系列不可編輯欄位。 這些資料來自各種來源，有無數的值可以顯示。

## 欄位類型{#field-types}

| **欄位名稱** | **定義** |
|---|---|
| 原始來源類型 | 首次發現訪客或網站訪客的位置(範例：清單匯入、網頁瀏覽) |
| 原始來源資訊 | 該位置的具體資訊(範例：清單名稱，網頁的URL) |
| 原始搜尋引擎 | 如果適用，將人員引薦至原始登入來源的搜尋引擎 |
| 原始搜尋片語 | 如果適用，則使用的搜尋詞會將人員引薦至原始登入來源 |
| 原始反向連結 | 代管原始登入來源的URL |
| 註冊源類型 | 活動最初成為人員的位置(例如：清單匯入、網頁瀏覽) |
| 註冊來源資訊 | 該位置的具體資訊(範例：清單名稱，網頁的URL) |
| 匿名IP | 指出人員的IP位址 |
| 推斷的公司 | Marketo對個人公司的最佳猜測（基於IP） |
| 推斷城市 | Marketto對個人城市的最佳猜測 |
| 推斷的州區 | Marketo對個人所在州或地區的最佳猜測（依據IP） |
| 推斷的郵遞區號 | Marketo對個人郵遞區號的最佳猜測（以IP為基礎） |
| 推斷國家 | Marketo對個人國家的最佳猜測 |
| 推斷的都市區 | Marketo對人口大都市區的最佳猜測 |
| 推斷的電話區號 | Marketo對個人區號的最佳猜測（以IP為基礎） |

## 原始源類型和註冊源類型的可能值{#possible-values-for-original-and-registration-source-type}

以下是一些可能的價值及其含義。

| **原始來源類型** | **定義** |
|---|---|
| Salesforce.com | 從Salesforce同步中發現人員 |
| 網頁瀏覽 | 從網頁中發現人 |
| Web表單篩選 | 填妥表格後發現了 |
| 清單匯入 | 從清單匯入中發現人員 |
| 新人 | 人員已手動輸入資料庫 |
| Web連結點按 | 在點按連結後發現人員 |
| 銷售電子郵件 | Person是透過Sales Insight電子郵件增益集傳送電子郵件給 |
| 人物 | Person是以個人身分從Salesforce同步 |
| 聯絡人 | 人員與Salesforce同步為聯絡人 |
| Munchkin API | Marketo的Munchkin API發現了Porsen |
| 社交應用程式 | 人被社交小工具發現 |
| 網站服務API | Person是由web service API發現的 |
| 活動合作夥伴 | 透過同步的網路研討會服務發現此人 |
| 關聯銷售線索 | 透過Associate Lead API呼叫合併的人員 |

| **註冊源類型** | **定義** |
|---|---|
| 清單匯入 | 透過清單匯入成為人 |
| Salesforce.com | 透過Salesforce同步化成為人 |
| Web表單篩選 | 填妥表格後成為人 |
| 銷售電子郵件 | Person是透過Sales Insight電子郵件增益集傳送電子郵件給 |
| 網站服務API | 人員是透過SOAP/REST API建立的 |
| 新人 | 人員已手動輸入資料庫 |
| Munchkin API | 透過Marketo的Munchkin API成為人 |
| 社交應用程式 | 透過社交小工具成為人 |
| 活動合作夥伴 | 透過連結的網路研討會服務成為個人 |
