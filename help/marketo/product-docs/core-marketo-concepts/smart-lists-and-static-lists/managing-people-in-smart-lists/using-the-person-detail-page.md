---
unique-page-id: 2953415
description: 使用人員詳細資料頁面 — Marketo檔案 — 產品檔案
title: 使用人員詳細資料頁面
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 23%

---

# 使用人員詳細資料頁面 {#using-the-person-detail-page}

個人詳細資訊頁面包含Marketo知道的所有個人資訊。 您可以直接從此頁面編輯資料。

## 前往個人詳細資料頁面 {#getting-to-person-detail-page}

有許多方式可開啟特定人員。 以下是一些範例：

* 您可以從&#x200B;**資料庫**&#x200B;中搜尋快速尋找
* 任何&#x200B;**智慧清單**&#x200B;或清單
* 方案的&#x200B;**成員**&#x200B;標籤
* 在Smart Campaign中&#x200B;**檢視行銷活動成員**
* 某些&#x200B;**報告**
  <br> 

1. 連按兩下任何人員或按一下左側的ID。

   ![](assets/one-1.png)

1. 這會開啟人員詳細資訊畫面。

   ![](assets/two-5.png)

## 頁面組織 — Salesforce {#page-organization-salesforce}

人員資訊會分類為下列標籤：

| 標記 | 說明 |
|---|---|
| 資訊 | 聯絡資訊和個人相關自訂欄位。 |
| 公司資訊 | 個人的公司資訊和地址。 |
| 機會資訊 | 已從Salesforce同步機會資訊。 |
| SFDC潛在客戶欄位 | 內建Salesforce欄位。 |
| SFDC自訂欄位 | 自訂Salesforce欄位。 |
| 活動記錄 | 與個人相關的所有活動。 |

## 頁面組織 — Microsoft Dynamics {#page-organization-microsoft-dynamics}

| 標記 | 說明 |
|---|---|
| 資訊 | 聯絡資訊和個人相關自訂欄位。 |
| 公司資訊 | 個人的公司資訊和地址。 |
| 機會資訊 | 已從Microsoft同步機會資訊。 |
| Microsoft自訂欄位 | 自訂Microsoft欄位。 |
| Microsoft潛在客戶欄位 | 內建Microsoft欄位。 |
| 活動記錄 | 與個人相關的所有活動。 |

>[!NOTE]
>
>您也可以看到透過API[插入的商機資訊](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/opportunities)，瞭解未與CRM同步的執行個體。

## 編輯欄位 {#editing-a-field}

許多欄位都是可編輯的。 若要更新人員資訊，請輸入新值，然後按一下欄位外部以儲存。

![](assets/image2015-2-27-11-3a14-3a2.png)

## CRM同步之前的Marketo預設欄位 {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| 地址 | 年營業額 | 匿名IP | 帳單寄送地址 | 帳單寄送城市 |
| 帳單國家 | 帳單郵遞區號 | 帳單州別 | 城市 | 公司名稱 |
| 國家/地區 | 建立時間 | 出生日期 | 部門 | 請勿來電 |
| 不要呼叫原因 | 請勿來電的理由 | 電子郵件地址 | 電子郵件無效 | 電子郵件無效原因 |
| 外部公司 ID | 外部銷售人員 ID | 傳真號碼 | 名字 | 全名 |
| 行業 | 推斷的城市 | 推斷公司 | 推斷國家 | 推斷的大都會區 |
| 推斷的電話區碼 | 推斷的郵遞區號 | 推斷的州別區域 | 匿名 | 是客戶 |
| 是合作夥伴 | 職稱 | 姓氏 | 評等 | 分數 |
| Source人員 | 狀態 | 主要電話 | Marketo社交[!DNL Facebook]顯示名稱 | Marketo社交[!DNL Facebook] Id |
| Marketo社交[!DNL Facebook]像片URL | Marketo社交[!DNL Facebook]設定檔URL | Marketo社交[!DNL Facebook]觸及 | Marketo社交[!DNL Facebook]反向註冊 | Marketo社交[!DNL Facebook]轉介的造訪 |
| Marketo社交性別 | Marketo社交上次反向連結註冊 | Marketo Social上次轉介的造訪 | Marketo社交[!DNL LinkedIn]顯示名稱 | Marketo社交[!DNL LinkedIn] Id |
| Marketo社交[!DNL LinkedIn]像片URL | Marketo社交[!DNL LinkedIn]設定檔URL | Marketo社交[!DNL LinkedIn]觸及 | Marketo社交[!DNL LinkedIn]反向註冊 | Marketo社交[!DNL LinkedIn]轉介的造訪 |
| Marketo社交整合ID | Marketo 社交轉介註冊總次數 | Marketo 社交轉介造訪總次數 | Marketo社交[!DNL Twitter]顯示名稱 | Marketo社交[!DNL Twitter] Id |
| Marketo社交[!DNL Twitter]像片URL | Marketo社交[!DNL Twitter]設定檔URL | Marketo社交[!DNL Twitter]觸及 | Marketo社交[!DNL Twitter]反向註冊 | Marketo社交[!DNL Twitter]轉介的造訪 |
| 中間名 | 手機號碼 | 員工數 | 電話號碼 | 郵遞區號 |
| 優先順序 | 相對分數 | 角色 | 稱謂 | 標準產業分類（SIC）代碼 |
| 現場 | 狀態 | 退訂 | 退訂原因 | 更新時間 |
| 急迫性 | 網站 |  |  |  |

>[!NOTE]
>
>部分欄位&#x200B;_無_&#x200B;可編輯：
>
>* 活動記錄
>* 公司資訊
>* SFDC聯絡人的機會
>* 特定Marketo欄位，例如「建立日期」和「原始Source型別」。
>
>深入瞭解[系統管理的欄位](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}。

>[!MORELIKETHIS]
>
>[建立個人詳細資料頁面的自訂標籤](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
