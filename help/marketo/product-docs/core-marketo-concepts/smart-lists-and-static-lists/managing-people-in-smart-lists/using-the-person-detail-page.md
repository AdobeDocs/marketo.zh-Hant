---
unique-page-id: 2953415
description: 使用人員詳細資料頁面 — Marketo檔案 — 產品檔案
title: 使用人員詳細資訊頁面
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 19%

---

# 使用人員詳細資訊頁面 {#using-the-person-detail-page}

人員詳細資訊頁面包含Marketo所知的關於人員的所有資訊。 您可以直接從此頁面編輯資料。

## 人員詳細資訊頁面 {#getting-to-person-detail-page}

有很多方法可以開啟特定的人。 例如：

* 從 **資料庫**，您可以在「快速尋找」中搜尋
* 任何智慧 **清單** 或清單
* **成員** 方案的標籤
* **檢視促銷活動成員** 在智慧型行銷活動中
* 部分 **報告**

   <br> 

1. 連按兩下任何人員，或按一下左側的ID。

   ![](assets/one-1.png)

1. 這會開啟人員詳細資料畫面。

   ![](assets/two-5.png)

## 頁面組織 — Salesforce {#page-organization-salesforce}

人員資訊分為下列標籤：

| 標籤 | 說明 |
|---|---|
| 資訊 | 人員的聯絡資訊和自訂欄位。 |
| 公司資訊 | 人員的公司資訊和地址。 |
| 機會資訊 | 從Salesforce同步的機會資訊。 |
| SFDC銷售機會欄位 | 內建的Salesforce欄位。 |
| SFDC自定義欄位 | 自訂Salesforce欄位。 |
| 活動記錄 | 與人員相關的所有活動。 |

## 頁面組織 — Microsoft Dynamics {#page-organization-microsoft-dynamics}

| 標籤 | 說明 |
|---|---|
| 資訊 | 人員的聯絡資訊和自訂欄位。 |
| 公司資訊 | 人員的公司資訊和地址。 |
| 機會資訊 | 從Microsoft同步的機會資訊。 |
| Microsoft自訂欄位 | 自訂Microsoft欄位。 |
| Microsoft主導欄位 | 內建Microsoft欄位。 |
| 活動記錄 | 與人員相關的所有活動。 |

>[!NOTE]
>
>您還可以看到Opportunity資訊 [透過API插入](https://developers.marketo.com/rest-api/lead-database/opportunities/) 適用於未與CRM同步的執行個體。

## 編輯欄位 {#editing-a-field}

許多欄位都可編輯。 若要更新人員的資訊，請輸入新值，然後按一下欄位外部以儲存。

![](assets/image2015-2-27-11-3a14-3a2.png)

## Marketo CRM同步前的預設欄位 {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| 地址 | 年營業額 | 匿名IP | 帳單寄送地址 | 帳單寄送城市 |
| 帳單國家 | 帳單郵遞區號 | 帳單州別 | 城市 | 公司名稱 |
| 國家 | 建立時間 | 出生日期 | 部門 | 請勿來電 |
| 不調用原因 | 請勿來電的理由 | 電子郵件地址 | 電子郵件無效 | 電子郵件無效原因 |
| 外部公司Id | 外部銷售人員 ID | 傳真號碼 | 名字 | 全名 |
| 產業 | 推斷的城市 | 推斷公司 | 推斷國家 | 推斷的大都會區 |
| 推斷的電話區碼 | 推斷的郵遞區號 | 推斷的州別地區 | 是匿名的 | 是客戶 |
| 是合作夥伴 | 職稱 | 姓氏 | 評等 | 分數 |
| 人員來源 | 狀態 | 主要電話 | Marketo Social Facebook顯示名稱 | Marketo Social Facebook Id |
| Marketo Social Facebook照片URL | Marketo Social Facebook設定檔URL | Marketo Social Facebook觸及 | Marketo Social Facebook反向註冊 | Marketo Social Facebook反向連結的造訪 |
| Marketo社會性別 | Marketo社交上次轉介的註冊 | Marketo Social上次轉介的造訪 | Marketo Social LinkedIn顯示名稱 | Marketo Social LinkedIn Id |
| Marketo Social LinkedIn照片URL | Marketo Social LinkedIn設定檔URL | Marketo Social LinkedIn觸及 | Marketo Social LinkedIn反向註冊 | Marketo Social LinkedIn反向連結的造訪 |
| Marketo Social整合ID | Marketo Social轉介登記總數 | Marketo社交反向連結瀏覽總數 | Marketo Social Twitter顯示名稱 | Marketo Social Twitter Id |
| Marketo Social Twitter照片URL | Marketo Social Twitter設定檔URL | Marketo Social Twitter觸及 | Marketo Social Twitter反向註冊 | Marketo Social Twitter反向連結的造訪 |
| 中間名 | 手機號碼 | 員工數 | 電話號碼 | 郵遞區號 |
| 優先順序 | 相對分數 | 角色 | 稱謂 | 標準產業分類（SIC）代碼 |
| 現場 | 州別 | 退訂 | 退訂原因 | 更新日期： |
| 緊急 | 網站 |  |  |  |

>[!NOTE]
>
>部分欄位包括 _not_ 可編輯：
>
>* 活動記錄
>* 公司資訊
>* SFDC聯繫人的機會
>* 特定於Marketo的欄位，例如「建立日期」和「原始來源類型」。
>
>深入了解 [系統管理欄位](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[為「人員詳細資訊」頁建立自定義頁簽](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
