---
description: 隱私權請求 — Marketo檔案 — 產品檔案
title: 隱私權請求
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# 隱私權請求 {#privacy-requests}

本檔案概述如何管理您可透過Marketo Engage UI和Privacy Service API傳送給Privacy Service的個別資料隱私權請求。

>[!NOTE]
>
>透過Privacy Service UI或用於Marketo Engage的API提交的隱私權請求僅適用於以下專案：
>
>* Marketo Engage已上線到AdobeIdentity Management系統的使用者
>
>**或 —**
>
>* Marketo Engage使用AdobeIdentity Management系統上已存在的其他Experience Cloud產品的使用者(例如RT-CDP、B2B和B2P版本、Audience Manager)。

您可以透過兩種方式提交存取和刪除Marketo Engage中消費者資料的個別請求：

* 透過[Privacy ServiceUI](https://privacyui.cloud.adobe.io/)。 請參閱檔案[這裡](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=zh-Hant){target="_blank"}。
* 透過Privacy Service API。 請參閱檔案[這裡](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"}和API資訊[這裡](https://developer.adobe.com/experience-platform-apis/){target="_blank"}。

[Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=zh-Hant){target="_blank"}支援兩種型別的請求：資料存取和資料刪除。

讓我們看看如何建立存取和刪除請求。

## 傳送Marketo Engage請求的必要設定 {#required-setup-to-send-requests-for-marketo-engage}

若要請求存取和刪除Marketo Engage資料，您必須：

1. 識別下列專案：

   a. IMS組織ID<br/>
b.您要對其採取動作之人員的電子郵件地址

   IMS組織ID是24個字元的英數字串，通常會加上@AdobeOrg。 如果您的行銷團隊或內部Adobe系統管理員不知道您組織的IMS組織ID，請透過`gdprsupport@adobe.com`聯絡Adobe客戶服務。 您需先取得IMS組織ID，才能向隱私權API提交請求。

1. 在Privacy Service中，您可以提交存取和刪除請求以Marketo Engage，並檢查現有請求的狀態。

## Marketo EngageJSON請求中的必填欄位值 {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;：

* &quot;namespace&quot;： **imsOrgID**
* &quot;value&quot;： `<Your IMS Org ID Value>`

&quot;users&quot;：

* &quot;action&quot;： **存取**&#x200B;或&#x200B;**刪除**
* &quot;userIDs&quot;：
   * &quot;namespace&quot;： **電子郵件**
   * &quot;type&quot;： **standard**
   * &quot;value&quot;： `<Data Subject's Email Address>`

&quot;include&quot;：

* **marketo** (適用於此請求的Adobe產品)

&quot;regulation&quot;：

* **gdpr**、**ccpa**、**pdpa**、**lgpd_bra**&#x200B;或&#x200B;**nzpa_nzl** （適用於此要求的隱私權法規）

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
>[隱私權管理](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
