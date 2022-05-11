---
description: 隱私請求 — Marketo文檔 — 產品文檔
title: 隱私請求
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# 隱私請求 {#privacy-requests}

本文檔概述了如何管理可通過Privacy ServiceUI和 **Privacy ServiceAPI**。

>[!NOTE]
>
>通過Privacy ServiceUI或API提交的隱私請求用於Marketo Engage，僅適用於具有Marketo Engage+ RT-CDP、B2B和B2P版本的用戶。

您可以通過兩種方式提交單個請求，以從Marketo Engage中訪問和刪除使用者資料：

* 通過 [Privacy ServiceUI](https://privacyui.cloud.adobe.io/)。 請參閱文檔 [這裡](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target=&quot;_blank&quot;}。
* 通過 **Privacy ServiceAPI**。 請參閱文檔 [這裡](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target=&quot;_blank&quot;}和API資訊 [這裡](https://developer.adobe.com/experience-platform-apis/){target=&quot;_blank&quot;}。

的 [Privacy Service](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target=&quot;_blank&quot;支援兩種類型的請求：資料存取和資料刪除。

讓我們看看如何建立訪問和刪除請求。

## 發送請求以進行Marketo Engage所需的設定 {#required-setup-to-send-requests-for-marketo-engage}

要請求訪問和刪除資料以進行Marketo Engage，您必須：

1. 確定以下內容：

   a.IMS組織ID<br/>
b.要執行操作的人員的電子郵件地址

   IMS組織ID是附加有@AdobeOrg的24個字元的字母數字字串。 如果您的營銷團隊或內部Adobe系統管理員不知道您組織的IMS組織ID，請通過gdprsupport@adobe.com聯繫Adobe客戶服務。 您需要IMS組織ID將請求提交到隱私API。

1. 在Privacy Service中，您可以將訪問和刪除請求提交到Marketo Engage，並檢查現有請求的狀態。

## Marketo EngageJSON請求中的必需欄位值 {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;命名空間&quot;: **ims組織ID**
* &quot;值&quot;: `<Your IMS Org ID Value>`

&quot;用戶&quot;:

* &quot;操作&quot;:或 **訪問** 或 **刪除**
* &quot;userIDs&quot;:
   * &quot;命名空間&quot;: **電子郵件**
   * &quot;類型&quot;: **標準**
   * &quot;值&quot;: `<Data Subject’s Email Address>`

&quot;包括&quot;:

* **市場** (即適用於請求的Adobe產品)

&quot;規章&quot;:

* **日當**。 **ccpa**。 **PDPA**。 **lgpd_bra**&#x200B;或 **nzpa_nzl**  （即適用於請求的隱私法規）

## 示例一：GDPR刪除請求 {#gdpr-delete-request}

JSON請求

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

JSON響應

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## 示例二：CCPA訪問請求 {#ccpa-access-request}

JSON請求

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

JSON響應

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[隱私管理](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
