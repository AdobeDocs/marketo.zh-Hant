---
unique-page-id: 5472615
description: 了解系統管理欄位 — Marketo檔案 — 產品檔案
title: 了解系統管理欄位
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 5%

---

# 了解系統管理欄位 {#understanding-system-managed-fields}

你可能注意到 [人員詳細資訊頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) 有Marketo建立的一系列不可編輯欄位。 這些資料來自各種來源，有無數的值可以顯示。

## 欄位類型 {#field-types}

| **欄位名稱** | **定義** |
|---|---|
| 原始源類型 | 首次發現人員或網站訪客的位置(範例：清單匯入、網頁瀏覽) |
| 原始源資訊 | 該位置的詳細資訊(範例：清單名稱，網頁URL) |
| 原始搜尋引擎 | 如果適用，將人員引薦至原始登入來源的搜尋引擎 |
| 原始搜索片語 | 如果適用，將人員引入原始錄入源所使用的搜索詞 |
| 原始反向連結 | 托管原始登入來源的URL |
| 註冊源類型 | 活動最初變成人員的位置(範例：清單匯入、網頁瀏覽) |
| 註冊源資訊 | 該位置的詳細資訊(範例：清單名稱，網頁URL) |
| 匿名 IP | 指示人員的IP地址 |
| 推斷的公司 | Marketo最佳猜測（以IP為基礎） |
| 推斷的城市 | Marketo對個人城市的最佳猜測（基於IP） |
| 推斷的州別地區 | Marketo對個人所在州或地區的最佳猜測（根據IP） |
| 推斷的郵遞區號 | Marketo最佳猜測（根據IP）人員郵遞區號 |
| 推斷的國家/地區 | Marketo最佳猜測（根據IP） |
| 推斷的大都會區 | Marketo對人口大都市區的最佳猜測（基於IP） |
| 推斷的電話區碼 | Marketo對人員區號的最佳猜測（根據IP） |

## 原始和註冊源類型的可能值 {#possible-values-for-original-and-registration-source-type}

以下是一些可能的值及其含義。

| **原始源類型** | **定義** |
|---|---|
| Salesforce.com | 從Salesforce同步中發現 |
| 網頁瀏覽次數 | 從網頁中發現人 |
| 網路表單篩選 | 填完表格後，人被發現 |
| 清單匯入 | 從清單匯入中發現人員 |
| 新人員 | 已將人員手動輸入資料庫 |
| 網頁連結點按 | 在按一下連結後發現人員 |
| 銷售電子郵件 | 人員已透過Sales Insight Email增益集傳送電子郵件 |
| 個人 | 人員是以人員身分從Salesforce同步 |
| 連絡人 | 人員已從Salesforce同步為連絡人 |
| 蒙奇金API | Marketo的Munchkin API發現了此人 |
| 社交應用程式 | 人被一個社交小工具發現 |
| 網站服務API | 網站服務API發現了人員 |
| 活動合作夥伴 | 透過同步的網路研討會服務發現人員 |
| 關聯銷售機會 | 透過關聯銷售機會API呼叫合併的人員 |

| **註冊源類型** | **定義** |
|---|---|
| 清單匯入 | 通過匯入清單成為人 |
| Salesforce.com | 通過Salesforce同步成為人 |
| 網路表單篩選 | 填完表格後變成人 |
| 銷售電子郵件 | 人員已透過Sales Insight Email增益集傳送電子郵件 |
| 網站服務API | 人員是透過SOAP/REST API建立 |
| 新人員 | 已將人員手動輸入資料庫 |
| 蒙奇金API | 透過Marketo的Munchkin API成為人 |
| 社交應用程式 | 通過社交小工具成為人 |
| 活動合作夥伴 | 透過連結的網路研討會服務成為個人 |
