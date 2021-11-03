---
description: 隱私權要求 — Marketo檔案 — 產品檔案
title: 隱私權要求
source-git-commit: fd4becf77135be7fc80156c8fde56f29a0aa38d0
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# 隱私權要求 {#privacy-requests}

本檔案概述如何管理個別資料隱私權請求，您可透過Privacy ServiceUI和 **Privacy ServiceAPI**.

您可以透過兩種方式提交個別請求，以從Marketo Engage中存取和刪除消費者資料：

* 透過 [Privacy ServiceUI](https://privacyui.cloud.adobe.io/). 請參閱本檔案 [此處](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_ui_tutorial.md).
* 透過 **Privacy ServiceAPI**. 請參閱本檔案 [此處](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_api_tutorial.md) 和API參考 [此處](https://www.adobe.io/apis/experiencecloud/gdpr/api-reference.html#!acpdr/swagger-specs/privacy-service.yaml).

此 [Privacy Service](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html) 支援兩種請求：資料存取和資料刪除。

注意：透過Privacy ServiceUI或API提交的Marketo Engage請求，僅適用於擁有Marketo Engage+ RT-CDP、B2B和B2P版本的客戶。

讓我們來看看您如何建立存取和刪除請求。

## 傳送請求以進行Marketo Engage的必要設定 {#required-setup-to-send-requests-for-marketo-engage}

若要請求存取和刪除Marketo Engage資料，您必須：

1. 識別下列項目：

   a.IMS組織ID<br/>
b.您要行事之人員的電子郵件地址

   IMS組織ID是24個字元的英數字串，並附加@AdobeOrg。 如果您的行銷團隊或內部Adobe系統管理員不知道您組織的IMS組織ID，請透過gdprsupport@adobe.com聯絡Adobe客戶服務。 您需要IMS組織ID才能將請求提交至隱私權API。

1. 在Privacy Service中，您可以提交存取和刪除請求以Marketo Engage，並檢查現有請求的狀態。

## Marketo EngageJSON請求中的必填欄位值 {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: <Your IMS Org ID Value>

&quot;users&quot;:

* &quot;key&quot;: <Your Request Tracking Key>   （可選）
* &quot;action&quot;:heer **存取** 或 **刪除**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **電子郵件**
   * &quot;type&quot;: **標準**
   * &quot;value&quot;: &lt;data subject=&quot;&quot; s=&quot;&quot; email=&quot;&quot; address=&quot;&quot;>

&quot;include&quot;:

* **marketo** (適用於請求的Adobe產品)

&quot;regulation&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd**，或 **nzpa**  （適用於請求的隱私權法規）

## 範例一：GDPR刪除請求 {#gdpr-delete-request}

JSON要求

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
      "key": "AAGDPRO1", 
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

JSON回應

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "key": "AAGDPRO1",
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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

## 範例二：CCPA存取要求 {#ccpa-access-request}

JSON要求

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
      "key": "AAGDPRO1",
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

JSON回應

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": " 3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "key": "AAGDPRO1",
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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
