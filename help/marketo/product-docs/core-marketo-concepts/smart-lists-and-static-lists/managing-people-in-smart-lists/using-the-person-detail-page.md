---
unique-page-id: 2953415
description: 使用人員詳細資料頁面 — Marketo檔案 — 產品檔案
title: 使用人員詳細資料頁面
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 22%

---

# 使用人員詳細資料頁面 {#using-the-person-detail-page}

個人詳細資訊頁面包含Marketo知道的所有個人資訊。 您可以直接從此頁面編輯資料。

## 前往個人詳細資料頁面 {#getting-to-person-detail-page}

有許多方式可開啟特定人員。 以下是一些範例：

* 從 **資料庫**，您可以在「快速尋找」中搜尋
* 任何 **智慧清單** 或清單
* **成員** 方案的索引標籤
* **檢視行銷活動成員** 在智慧行銷活動中
* 部分 **報表**
  <br> 

1. 連按兩下任何人員或按一下左側的ID。

   ![](assets/one-1.png)

1. 這會開啟人員詳細資訊畫面。

   ![](assets/two-5.png)

## 頁面組織 — Salesforce {#page-organization-salesforce}

人員資訊會分類為下列標籤：

| 標籤 | 說明 |
|---|---|
| 資訊 | 聯絡資訊和個人相關自訂欄位。 |
| 公司資訊 | 個人的公司資訊和地址。 |
| 機會資訊 | 已從Salesforce同步機會資訊。 |
| SFDC銷售機會欄位 | 內建Salesforce欄位。 |
| SFDC自訂欄位 | 自訂Salesforce欄位。 |
| 活動記錄 | 與個人相關的所有活動。 |

## 頁面組織 — Microsoft Dynamics {#page-organization-microsoft-dynamics}

| 標籤 | 說明 |
|---|---|
| 資訊 | 聯絡資訊和個人相關自訂欄位。 |
| 公司資訊 | 個人的公司資訊和地址。 |
| 機會資訊 | 已從Microsoft同步機會資訊。 |
| Microsoft自訂欄位 | 自訂Microsoft欄位。 |
| Microsoft潛在客戶欄位 | 內建Microsoft欄位。 |
| 活動記錄 | 與個人相關的所有活動。 |

>[!NOTE]
>
>您也可以看到商機資訊 [透過API插入](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities) 用於未與CRM同步的執行個體。

## 編輯欄位 {#editing-a-field}

許多欄位都是可編輯的。 若要更新人員資訊，請輸入新值，然後按一下欄位外部以儲存。

![](assets/image2015-2-27-11-3a14-3a2.png)

## CRM同步之前的Marketo預設欄位 {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| 地址 | 年營業額 | 匿名IP | 帳單寄送地址 | 帳單寄送城市 |
| 帳單國家 | 帳單郵遞區號 | 帳單州別 | 城市 | 公司名稱 |
| 國家 | 建立時間 | 出生日期 | 部門 | 請勿來電 |
| 不要呼叫原因 | 請勿來電的理由 | 電子郵件地址 | 電子郵件無效 | 電子郵件無效原因 |
| 外部公司 ID | 外部銷售人員 ID | 傳真號碼 | 名字 | 全名 |
| 產業 | 推斷的城市 | 推斷公司 | 推斷國家 | 推斷的大都會區 |
| 推斷的電話區碼 | 推斷的郵遞區號 | 推斷的州別區域 | 匿名 | 是客戶 |
| 是合作夥伴 | 職稱 | 姓氏 | 評等 | 分數 |
| 個人來源 | 狀態 | 主要電話 | Marketo Social Facebook顯示名稱 | Marketo Social Facebook Id |
| Marketo Social Facebook像片URL | Marketo社交Facebook設定檔URL | Marketo Social Facebook觸及 | Marketo Social Facebook轉介註冊 | Marketo Social Facebook轉介造訪 |
| Marketo社交性別 | Marketo社交上次反向連結註冊 | Marketo Social上次轉介的造訪 | Marketo Social LinkedIn顯示名稱 | Marketo Social LinkedIn Id |
| Marketo Social LinkedIn像片URL | Marketo社交LinkedIn設定檔URL | Marketo Social LinkedIn觸及 | Marketo Social LinkedIn轉介註冊 | Marketo Social LinkedIn轉介造訪 |
| Marketo社交整合ID | Marketo 社交轉介註冊總次數 | Marketo 社交轉介造訪總次數 | Marketo社交Twitter顯示名稱 | Marketo社交TwitterID |
| Marketo社交Twitter像片URL | Marketo社交Twitter設定檔URL | Marketo社交Twitter觸及 | Marketo社交Twitter反向註冊 | Marketo社交Twitter轉介造訪 |
| 中間名 | 手機號碼 | 員工數 | 電話號碼 | 郵遞區號 |
| 優先順序 | 相對分數 | 角色 | 稱謂 | 標準產業分類（SIC）代碼 |
| 現場 | 州別 | 退訂 | 退訂原因 | 更新時間 |
| 急迫性 | 網站 |  |  |  |

>[!NOTE]
>
>部分欄位為 _非_ 可編輯：
>
>* 活動記錄
>* 公司資訊
>* SFDC連絡人的機會
>* 特定Marketo欄位，例如「建立日期」和「原始來源型別」。
>
>進一步瞭解 [系統管理的欄位](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[建立人員詳細資料頁面的自訂標籤](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
