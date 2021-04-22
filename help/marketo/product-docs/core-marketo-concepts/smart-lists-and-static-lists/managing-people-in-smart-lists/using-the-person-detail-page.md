---
unique-page-id: 2953415
description: 使用人員詳細資訊頁-Marketo文檔——產品文檔
title: 使用人員詳細資訊頁
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 13%

---

# 使用人員詳細資訊頁{#using-the-person-detail-page}

人員詳細資訊頁面包含Marketo所知的關於人員的所有資訊。 您可以直接從此頁面編輯資料。

## Getting to Person Detail Page {#getting-to-person-detail-page}

有許多方式可以開放特定的人。 例如：

* 從&#x200B;**Database**&#x200B;中，可以在「快速查找」中搜索
* 任何智慧型&#x200B;**list**&#x200B;或list
* **方** 案會員表
* **在智慧型促銷** 活動中檢視促銷活動會籍
* 部分&#x200B;**報告**

   <br> 

1. 按兩下任何人，或按一下左側的ID。

   ![](assets/one-1.png)

1. 這會開啟人員詳細資料畫面。

   ![](assets/two-5.png)

## 頁面組織- Salesforce {#page-organization-salesforce}

人員資訊分為以下頁籤：

| 頁籤 | 說明 |
|---|---|
| 資訊 | 連絡資訊和人員的自訂欄位。 |
| 公司資訊 | 人員的公司資訊和地址。 |
| 機會資訊 | 與Salesforce同步的機會資訊。 |
| SFDC銷售線索欄位 | 內建的Salesforce欄位。 |
| SFDC自定義欄位 | 自訂Salesforce欄位。 |
| 活動日誌 | 與該人相關的所有活動。 |

## 頁面組織- Microsoft Dynamics {#page-organization-microsoft-dynamics}

| 頁籤 | 說明 |
|---|---|
| 資訊 | 連絡資訊和人員的自訂欄位。 |
| 公司資訊 | 人員的公司資訊和地址。 |
| 機會資訊 | 與Microsoft同步的機會資訊。 |
| Microsoft自訂欄位 | 自訂Microsoft欄位。 |
| Microsoft銷售線索欄位 | 內建Microsoft欄位。 |
| 活動日誌 | 與該人相關的所有活動。 |

>[!NOTE]
>
>您還可以看到通過API](http://developers.marketo.com/rest-api/lead-database/opportunities/)插入的與CRM不同步的實例的機會資訊[。

## 編輯欄位{#editing-a-field}

許多欄位都可編輯。 若要更新人員的資訊，請輸入新值，然後按一下欄位外的以儲存。

![](assets/image2015-2-27-11-3a14-3a2.png)

## MarketoCRM同步{#marketo-default-fields-prior-to-crm-sync}之前的預設欄位

|  |  |  |  |  |
|---|---|---|---|---|
| 地址 | 年營業額 | 匿名IP | 帳單寄送地址 | 帳單寄送城市 |
| 帳單寄送國家 | 帳單郵遞區號 | 帳單寄送州 | 城市 | 公司名稱 |
| 國家 | 建立於 | 出生日期 | 部門 | 請勿來電 |
| 不呼叫原因 | 請勿來電的理由 | 電子郵件地址 | 電子郵件無效 | 電子郵件無效原因 |
| 外部公司ID | 外部銷售人員ID | 傳真號碼 | 名字 | 全名 |
| 行業 | 推斷城市 | 推斷公司 | 推斷國家 | 推斷的都市區 |
| 推斷的電話區號 | 推斷的郵遞區號 | 推斷的州區 | 匿名 | 是客戶 |
| 是合作夥伴 | 職稱 | 姓氏 | 評分 | 分數 |
| 人員來源 | 狀態 | 主要電話 | Marketo社會Facebook顯示名稱 | Marketo社會FacebookID |
| Marketo社會Facebook照片URL | Marketo社會Facebook個人檔案URL | Marketo社會Facebook | Marketo社會Facebook參考註冊 | Marketo社會Facebook反向訪問 |
| Marketo社會性別 | Marketo社交上次引薦註冊 | Marketo社交上次反向連結瀏覽 | Marketo社會LinkedIn顯示名稱 | Marketo社會LinkedInID |
| Marketo社會LinkedIn照片URL | Marketo社會LinkedIn個人檔案URL | Marketo社會LinkedIn | Marketo社會LinkedIn參考註冊 | Marketo社會LinkedIn反向訪問 |
| Marketo社社交協同內容ID | Marketo社會轉介登記總數 | Marketo社交反向連結瀏覽總數 | Marketo社會Twitter顯示名稱 | Marketo社會TwitterID |
| Marketo社會Twitter照片URL | Marketo社會Twitter個人檔案URL | Marketo社會Twitter | Marketo社會Twitter參考註冊 | Marketo社會Twitter反向訪問 |
| 中間名 | 手機號碼 | 員工數 | 電話號碼 | 郵遞區號 |
| 優先順序 | 相對分數 | 職位 | 稱謂 | 標準產業分類（SIC）代碼 |
| 現場 | 州 | 退訂 | 退訂原因 | 更新日期： |
| 緊急 | 網站 |  |  |  |

>[!NOTE]
>
>有些欄位為&#x200B;_not_&#x200B;可編輯：
>
>* 活動日誌
>* 公司資訊
>* SFDC聯繫人的機會
>* 特定於Marketo的欄位，如建立日期和原始源類型。

>
>
進一步瞭解[系統管理欄位](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md)。

>[!MORELIKETHIS]
>
>[為「人員詳細資訊」頁建立自定義標籤](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
