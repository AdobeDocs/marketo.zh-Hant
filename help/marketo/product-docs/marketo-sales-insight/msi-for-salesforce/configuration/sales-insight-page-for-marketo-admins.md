---
unique-page-id: 42762409
description: Marketo管理員的Sales Insight頁面 — Marketo文檔 — 產品文檔
title: Marketo管理員的Sales Insight頁
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
source-git-commit: 5812f447fbe22bee13060afae8408de7ca7384e5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Marketo管理員的Sales Insight頁 {#sales-insight-page-for-marketo-admins}

Marketo管理員在Sales Insight中具有特定權限。 瞭解下面的內容。

## SOAP API配置 {#soap-api-configuration}

這些憑據用於將您的Salesforce帳戶連接到您的Marketo實例，以便在Salesforce中使用MSI。

![](assets/one-1.png)

## REST API配置 {#rest-api-configuration}

這些憑據用於將您的Salesforce帳戶連接到您的Marketo實例，以便在Salesforce中使用MSI Insights Dashboard。

![](assets/two-1.png)

## 人員分數設定 {#person-score-settings}

* **星**:星表表示與其他線索相比的匯流排索得分。
* **火焰**:火焰代表著緊迫性 — 最近一個領先者的得分發生了多大變化。

預設情況下，Marketo銷售洞察器使用「銷售線索得分」欄位計算星形和火焰。 但如果你想選擇一個不同的領域，下面是方法：

1. 在 **管理** Marketo區域，按一下 **銷售洞察**。

   ![](assets/four.png)

1. 在「銷售線索評級設定」下，按一下 **編輯**。

   ![](assets/five.png)

1. 選擇要用於星號的欄位。

   ![](assets/six.png)

1. 選擇要用於火焰的欄位。

   ![](assets/seven.png)

1. 按一下 **保存**。 重新計算銷售洞察力需要一些時間。 您可以稍後查看您的CRM，以查看星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果尚沒有自定義分數欄位，請參見 [建立](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

   >[!MORELIKETHIS]
   >
   >[星與火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 設定 {#settings}

![](assets/nine.png)

**取消訂閱設定：**

您可以從以下取消訂閱設定中選擇：無模板、標準電子郵件和操作電子郵件

* 尊重取消訂閱設定
* 當超過1個收件人時，請遵守取消訂閱設定
* 當超過5個收件人時，請尊重取消訂閱設定
* 忽略取消訂閱設定

**啟用鎖定模板的功能：**

啟用後，MSI用戶將無法在從Salesforce發送電子郵件時編輯模板

**啟用RSS源：**

啟用後，MSI用戶可以在RSS源中查看其Lead Feed（除Salesforce中的Lead Feed外）。 RSS源僅在禁用「令牌過期」功能時才能運行。

**令牌到期：**

令牌到期在功能管理器中控制。 要啟用/禁用它，請聯繫 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。 啟用後，所有Marketo令牌將在10分鐘內過期。 禁用後，Marketo令牌將不會過期。

啟用令牌過期之前生成的令牌將沒有要驗證的過期時間，因此即使當前啟用了該功能，它們也不會過期。

啟用令牌過期後生成的令牌的過期時間為10分鐘，因此即使禁用了該功能，這些令牌仍將在10分鐘內過期。

令牌行為將基於其生成時間（啟用/禁用令牌過期功能時，而不是其當前功能狀態）。
