---
unique-page-id: 5472615
description: 瞭解系統管理的欄位 — Marketo檔案 — 產品檔案
title: 瞭解系統管理的欄位
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 8%

---

# 瞭解系統管理的欄位 {#understanding-system-managed-fields}

您可能已注意到 [個人詳細資料頁面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} 有一系列Marketo建立的不可編輯欄位。 這些資料來自各種來源，而且可以顯示無數值。

## 欄位型別 {#field-types}

| **欄位名稱** | **定義** |
|---|---|
| 原始來源類型 | 首次發現個人或網站訪客的位置（範例：清單匯入、網頁造訪） |
| 原始來源資訊 | 該位置的詳細資訊（範例：清單名稱、網頁URL） |
| 原始搜尋引擎 | 將人員轉至原始專案來源的搜尋引擎（如適用） |
| 原始搜尋片語 | 如果適用，會使用將人員轉至原始專案來源的搜尋字詞 |
| 原始反向連結 | 託管原始登入來源的URL |
| 註冊來源型別 | 活動首次成為個人的位置（例如：清單匯入、網頁造訪） |
| 註冊來源資訊 | 該位置的詳細資訊（範例：清單名稱、網頁URL） |
| 匿名 IP | 表示個人的IP位址 |
| 推斷的公司 | Marketo對個人公司的最佳猜測（根據IP） |
| 推斷的城市 | Marketo對個人城市的最佳猜測（根據IP） |
| 推斷的州別區域 | Marketo對個人所在州或地區的最佳猜測（根據IP） |
| 推斷的郵遞區號 | Marketo對個人郵遞區號的最佳猜測（根據IP） |
| 推斷的國家 | Marketo對個人所在國家/地區的最佳猜測（根據IP） |
| 推斷的大都會區 | Marketo對個人大都會區域的最佳猜測（根據IP） |
| 推斷的電話區碼 | Marketo對個人區碼的最佳猜測（根據IP） |

## 原始與註冊來源型態的可能值 {#possible-values-for-original-and-registration-source-type}

以下是一些可能的值及其含義。

| **原始來源類型** | **定義** |
|---|---|
| Salesforce.com | 人員是從 [!DNL Webhook] 同步 |
| 網頁瀏覽次數 | 從網頁發現人員 |
| 網頁表單轉出 | 填寫表單後發現人員 |
| 清單匯入 | 從清單匯入中發現人員 |
| 新人員 | 已將人員手動輸入資料庫 |
| Web連結點按 | 按一下連結後發現人員 |
| 銷售電子郵件 | 已透過向某人傳送電子郵件 [!DNL Sales Insight] 電子郵件增益集 |
| 個人 | 人員已同步處理來源 [!DNL Salesforce] 作為個人 |
| 連絡人 | 人員已同步處理來源 [!DNL Webhook] 作為連絡人 |
| [!DNL Munchkin] API | Marketo Engage發現人員 [!DNL Munchkin] API |
| 社交應用程式 | 由社交Widget探索人員 |
| 網站服務API | 透過網站服務API發現人員 |
| 活動合作夥伴 | 透過同步網路研討會服務發現人員 |
| 關聯銷售機會 | 透過「關聯銷售機會API」呼叫合併的人員 |

| **註冊來源型別** | **定義** |
|---|---|
| 清單匯入 | 透過清單匯入成為個人 |
| Salesforce.com | 透過 [!DNL Webhook] 同步 |
| 網頁表單轉出 | 填寫表單後成為人員 |
| 銷售電子郵件 | 已透過向某人傳送電子郵件 [!DNL Webhook] 電子郵件增益集 |
| 網站服務API | 已透過SOAP/REST API建立人員 |
| 新人員 | 已將人員手動輸入資料庫 |
| [!DNL Munchkin] API | 透過Marketo成為一個人 [!DNL Munchkin] API |
| 社交應用程式 | 透過社交Widget變成人 |
| 活動合作夥伴 | 透過連結的網路研討會服務成為個人 |
