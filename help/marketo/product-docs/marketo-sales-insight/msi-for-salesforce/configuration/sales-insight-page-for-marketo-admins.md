---
unique-page-id: 42762409
description: Marketo管理員的銷售分析頁面 — Marketo檔案 — 產品檔案
title: Marketo管理員的銷售分析頁面
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Marketo管理員的銷售分析頁面 {#sales-insight-page-for-marketo-admins}

Marketo管理員在Sales Insight中有特定的許可權。 瞭解以下內容。

## Soap API設定 {#soap-api-configuration}

這些憑證可用來將您的Salesforce帳戶連線到您的Marketo執行個體，以便在Salesforce中使用MSI。

![](assets/one-1.png)

## Rest API設定 {#rest-api-configuration}

這些憑證可用來將您的Salesforce帳戶連結至您的Marketo執行個體，以便在Salesforce中使用MSI前瞻分析控制面板。

![](assets/two-1.png)

## 個人分數設定 {#person-score-settings}

* **星級**：星星代表和其他潛在客戶相較之下的總潛在客戶分數。
* **火焰**：火焰代表急迫性 — 潛在客戶分數最近已變更多少。

依預設，Marketo Sales Insight會使用「銷售機會分數」欄位來計算星星和火焰。 但如果您想挑選不同的欄位，請依照以下方式：

1. 在 **管理員** Marketo區域，按一下 **銷售分析**.

   ![](assets/four.png)

1. 在「潛在客戶評分設定」底下，按一下 **編輯**.

   ![](assets/five.png)

1. 選取您要用於星星的欄位。

   ![](assets/six.png)

1. 選取您要用於火焰的欄位。

   ![](assets/seven.png)

1. 按一下 **儲存**. 重新計算銷售分析需要一些時間。 您可以稍後檢視CRM，檢視星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您還沒有自訂分數欄位，以下說明如何 [建立它們](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[星星與火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 設定 {#settings}

![](assets/nine.png)

**取消訂閱設定：**

您可以從以下取消訂閱設定中選擇「無範本」、「標準電子郵件」和「營運電子郵件」

* 遵守取消訂閱設定
* 超過1位收件者時，請遵循取消訂閱設定
* 超過5位收件者時遵循取消訂閱設定
* 忽略取消訂閱設定

**啟用鎖定範本的功能：**

啟用後，MSI使用者將無法從Salesforce傳送電子郵件時編輯範本

**啟用RSS摘要：**

啟用後，MSI使用者可以在RSS摘要中檢視其銷售機會摘要（除了Salesforce中的銷售機會摘要之外）。 RSS摘要只有在「權杖有效期」功能停用時才能運作。

**權杖有效期：**

權杖到期在「功能管理員」中控制。 若要啟用/停用此功能，請聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support). 啟用後，所有Marketo Token都會在10分鐘內過期。 停用時，Marketo Token不會過期。

在啟用權杖過期之前產生的Token不會有可驗證的有效期，因此即使目前啟用了功能，也不會過期。

在啟用權杖過期之後產生的Token有10分鐘的過期時間，因此即使停用該功能，它們仍將在10分鐘後過期。

權杖行為將以其產生時間為基礎（當權杖到期功能已啟用/停用時，而不是其目前的功能狀態）。
