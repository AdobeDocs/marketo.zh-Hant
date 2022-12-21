---
unique-page-id: 42762409
description: 適用於Marketo管理員的Sales Insight頁面 — Marketo檔案 — 產品檔案
title: 適用於Marketo管理員的Sales Insight頁面
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
source-git-commit: 5812f447fbe22bee13060afae8408de7ca7384e5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 適用於Marketo管理員的Sales Insight頁面 {#sales-insight-page-for-marketo-admins}

Marketo管理員在Sales Insight中擁有特定權限。 了解下面的內容。

## Soap API配置 {#soap-api-configuration}

這些憑證用於將Salesforce帳戶連接到Marketo實例，以便在Salesforce中使用MSI。

![](assets/one-1.png)

## 重設API設定 {#rest-api-configuration}

這些憑證用於將Salesforce帳戶連接到Marketo實例，以便在Salesforce中使用MSI Insights Dashboard。

![](assets/two-1.png)

## 人員分數設定 {#person-score-settings}

* **星**:星號代表相較於其他銷售機會的總銷售機會分數。
* **火焰**:火焰代表著緊迫性 — 最近鉛的分數發生了多大變化。

依預設，Marketo Sales Insight會使用Lead Score欄位來計算星形和火焰。 但是，如果你想選擇一個不同的領域，以下是方法：

1. 在 **管理** Marketo區域，按一下 **Sales Insight**.

   ![](assets/four.png)

1. 在「銷售機會計分設定」下，按一下 **編輯**.

   ![](assets/five.png)

1. 選擇要用於星的欄位。

   ![](assets/six.png)

1. 選擇要用於火焰的欄位。

   ![](assets/seven.png)

1. 按一下 **儲存**. 重新計算銷售分析需要一些時間。 您稍後可以檢查您的CRM，看到星光和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您尚未擁有自訂分數欄位，以下說明如何 [建立](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[星與火](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 設定 {#settings}

![](assets/nine.png)

**取消訂閱設定：**

您可以從下列取消訂閱設定中選擇：無範本、標準電子郵件和操作電子郵件

* 遵守取消訂閱設定
* 超過1個收件者時，請遵守「取消訂閱設定」
* 超過5個收件者時，請遵守「取消訂閱設定」
* 忽略取消訂閱設定

**啟用鎖定模板的功能：**

啟用後，MSI用戶將無法在從Salesforce發送電子郵件時編輯模板

**啟用RSS源：**

啟用後，MSI用戶可以在RSS源中查看其銷售機會饋送（除了Salesforce中的銷售機會饋送之外）。 RSS饋送只能在停用「代號過期」功能時運作。

**代號過期：**

權杖過期由功能管理員控制。 若要啟用/停用，請前往 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support). 啟用後，所有Marketo代號將在10分鐘內過期。 停用時，Marketo代號不會過期。

在啟用Token過期之前產生的Token沒有要驗證的到期時間，因此即使功能目前已啟用，它們也不會過期。

啟用Token過期後產生的Token過期時間將為10分鐘，因此即使停用功能，這些Token仍將在10分鐘後過期。

代號行為將根據其產生時間（代號過期功能啟用/停用時，而非其目前功能狀態）。
