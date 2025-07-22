---
unique-page-id: 42762409
description: Marketo管理員銷售Insight頁面 — Marketo檔案 — 產品檔案
title: Marketo管理員專用的Insight銷售頁面
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Marketo管理員的[!DNL Sales Insight]頁面 {#sales-insight-page-for-marketo-admins}

Marketo管理員在[!DNL Sales Insight]中擁有特定許可權。 瞭解以下內容。

## Soap API設定 {#soap-api-configuration}

這些認證可用來將您的[!DNL Salesforce]帳戶連線至您的Marketo執行個體，以便在[!DNL Salesforce]中使用MSI。

![](assets/one-1.png)

## Rest API設定 {#rest-api-configuration}

這些認證可用來將您的[!DNL Salesforce]帳戶連線至您的Marketo執行個體，以便在[!DNL Salesforce]中使用MSI深入分析儀表板。

![](assets/two-1.png)

## 個人分數設定 {#person-score-settings}

* **[!UICONTROL Stars]**：星星代表和其他潛在客戶相較之下的潛在客戶總分。
* **[!UICONTROL Flames]**：火焰代表急迫性 — 潛在客戶的分數最近已變更多少。

根據預設，[!DNL Marketo Sales Insight]會使用「潛在客戶分數」欄位來計算星星和火焰。 但如果您想挑選不同的欄位，選擇方法如下：

1. 在Marketo的&#x200B;**[!UICONTROL Admin]**&#x200B;區域中，按一下&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/four.png)

1. 在[!UICONTROL Lead Scoring Settings]底下，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/five.png)

1. 選取您要用於星星的欄位。

   ![](assets/six.png)

1. 選取您要用於火焰的欄位。

   ![](assets/seven.png)

1. 按一下&#x200B;**[!UICONTROL Save]**。 銷售insight將需要一些時間重新計算。 您可以稍後檢視您的CRM，以檢視星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您還沒有自訂分數欄位，以下說明如何[建立它們](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

   >[!MORELIKETHIS]
   >
   >[星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 設定 {#settings}

![](assets/nine.png)

**取消訂閱設定：**

您可以從下列[!UICONTROL No Template]、[!UICONTROL Standard Emails]與[!UICONTROL Operational emails]的取消訂閱設定中選擇

* [!UICONTROL Respect Unsubscribe Setting]
* [!UICONTROL Respect Unsubscribe Settings when more than 1 recipient]
* [!UICONTROL Respect Unsubscribe Settings when more than 5 recipients]
* [!UICONTROL Ignore Unsubscribe Settings]

**啟用鎖定範本的功能：**

啟用後，MSI使用者將無法從[!DNL Salesforce]傳送電子郵件時編輯範本

**啟用RSS摘要：**

啟用後，MSI使用者可以在RSS摘要中檢視他們的銷售機會摘要（除了[!DNL Salesforce]中的銷售機會摘要之外）。 RSS摘要只有在停用&quot;[!UICONTROL Token Expiration]&quot;功能時才能運作。

**權杖到期日：**

權杖有效期限可在「功能管理員」中控制。 若要啟用/停用此功能，請連絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。 啟用後，所有Marketo Token都會在10分鐘內過期。 停用後，Marketo代號將不會過期。

在啟用權杖到期之前產生的Token沒有可驗證的到期時間，因此即使目前啟用該功能，也不會到期。

在啟用權杖過期之後產生的Token有10分鐘的過期時間，因此即使停用該功能，它們仍將在10分鐘後過期。

權杖行為將以其產生時間為基礎（當權杖到期功能已啟用/停用時，而不是其目前的功能狀態）。
