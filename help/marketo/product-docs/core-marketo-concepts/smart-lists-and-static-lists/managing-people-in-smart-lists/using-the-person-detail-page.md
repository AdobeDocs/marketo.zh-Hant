---
unique-page-id: 2953415
description: 使用人員詳細資料頁面——行銷人員檔案——產品檔案
title: 使用人員詳細資訊頁
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---


# 使用人員詳細資訊頁{#using-the-person-detail-page}

人員詳細資料頁面包含行銷人員瞭解的所有人員資訊。 您可以直接從此頁面編輯資料。

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

## CRM同步{#marketo-default-fields-prior-to-crm-sync}之前的Marketto預設欄位

|  |  |  |  |  |
|---|---|---|---|---|
| 地址 | 年收入 | 匿名IP | 帳單地址 | 帳單城市 |
| 帳單國家／地區 | 帳單郵遞區號 | 帳單狀態 | 城市 | 公司名稱 |
| 國家／地區 | 建立於 | 出生日期 | 部門 | 不要呼叫 |
| 不呼叫原因 | 不呼叫原因 | 電子郵件地址 | 電子郵件無效 | 電子郵件無效原因 |
| 外部公司ID | 外部銷售人員ID | 傳真號碼 | 名字 | 完整名稱 |
| 產業 | 推斷城市 | 推斷的公司 | 推斷國家 | 推斷的都市區 |
| 推斷的電話區號 | 推斷的郵遞區號 | 推斷的州區 | 匿名 | 是客戶 |
| 是合作夥伴 | 職稱 | 姓氏 | 評分 | 分數 |
| 人員來源 | 狀態 | 主手機 | Marketo Social Facebook顯示名稱 | Marketo Social FacebookID |
| Marketo Social Facebook像片URL | Marketo Social Facebook設定檔URL | Marketo Social Facebook觸及率 | Marketo Social Facebook反向連結註冊 | Marketo Social Facebook反向連結瀏覽 |
| 行銷社會性別 | Marketo Social上次反向連結註冊 | Marketo Social上次反向連結瀏覽 | Marketo Social LinkedIn顯示名稱 | Marketo Social LinkedIn Id |
| Marketo Social LinkedIn像片URL | Marketo Social LinkedIn設定檔URL | Marketo Social LinkedIn觸及面 | Marketo Social LinkedIn參考的註冊 | Marketo Social LinkedIn反向連結瀏覽 |
| Marketo Social協同內容ID | Marketo Social反向連結登記總數 | Marketo Social反向連結瀏覽總數 | Marketo Social Twitter顯示名稱 | Marketo Social TwitterID |
| Marketo Social Twitter像片URL | Marketo Social Twitter設定檔URL | Marketo Social Twitter觸及 | Marketo Social Twitter反向連結註冊 | Marketo Social Twitter反向連結瀏覽 |
| 中間名 | 行動電話號碼 | 員工人數 | 電話號碼 | 郵遞區號 |
| 優先順序 | 相對分數 | 角色 | 問候語 | SIC代碼 |
| 網站 | 州 | 取消訂閱 | 未訂閱原因 | 更新日期： |
| 緊急 | 網站 |  |  |  |

>[!NOTE]
>
>有些欄位為&#x200B;_not_&#x200B;可編輯：
>
>* 活動日誌
>* 公司資訊
>* SFDC聯繫人的機會
>* 特定行銷專用欄位，例如「建立日期」和「原始來源類型」。

>
>
進一步瞭解[系統管理欄位](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md)。

>[!MORELIKETHIS]
>
>[為「人員詳細資訊」頁建立自定義標籤](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
