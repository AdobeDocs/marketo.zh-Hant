---
unique-page-id: 7511512
description: 在Salesforce1中安裝及設定Marketo Sales Insight - Marketo檔案 — 產品檔案
title: 在Salesforce1中安裝和設定Marketo Sales Insight
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# 在Salesforce1中安裝和設定Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>現有客戶，請[升級您的MSI封裝](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)，然後再繼續！

>[!PREREQUISITES]
>
>如果您有Salesforce Enterprise/Unlimited：
>
>* [步驟3之1：將Marketo欄位新增至Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [步驟2之3：建立Marketo (Enterprise/Unlimited)的Salesforce使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [步驟3之3：連線Marketo與Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>如果您有Salesforce Professional：
>
>* [在Salesforce Professional Edition中設定Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>Salesforce1中的Marketo Sales Insight包括：首選、銷售機會摘要、有趣的時刻，以及「新增至Marketo促銷活動」。

## 啟用Salesforce1行動應用程式 {#enable-the-salesforce1-mobile-app}

1. 按一下&#x200B;**設定**，然後按一下&#x200B;**行動系統管理**。

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. 按一下&#x200B;**Salesforce1**。

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. 按一下&#x200B;**Salesforce1設定**。

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. 按一下&#x200B;**啟用Salesforce1行動瀏覽器應用程式**。

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. 選取&#x200B;**行動管理**。

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. 按一下&#x200B;**管理行動導覽功能表**。

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. 選取&#x200B;**Marketo**&#x200B;並&#x200B;**將它新增至**&#x200B;選取的&#x200B;**功能表專案**。

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. 選取&#x200B;**Marketo**，將其&#x200B;**向上**&#x200B;移至所需區域，然後按一下&#x200B;**儲存**。

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## 隱藏過時的Marketo自訂物件 {#hide-outdated-marketo-custom-object}

1. 按一下&#x200B;**設定**。

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. 選取&#x200B;**管理使用者**。

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. 選取&#x200B;**設定檔**。

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. 按一下以&#x200B;**編輯**&#x200B;任何需要的設定檔。

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. 在&#x200B;**索引標籤設定**&#x200B;下，選取&#x200B;_第一個_ **Marketo**。

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. 選取&#x200B;**隱藏的索引標籤**。

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >請務必隱藏所有所需設定檔的Marketo標籤！

## 自訂標籤 {#customize-tabs}

1. 按一下&#x200B;**+**。

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. 按一下&#x200B;**自訂我的標籤**。

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. 選取&#x200B;**Marketo**&#x200B;和&#x200B;**將它新增至選取的索引標籤**。

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. 選取&#x200B;**Marketo**，將其&#x200B;**向上**&#x200B;移至所需區域，然後按一下&#x200B;**儲存**。

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## 自訂頁面配置 {#customize-page-layouts}

1. 按一下&#x200B;**設定**。

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. 按一下[銷售機會]下的[設定]****，輸入&#x200B;**頁面配置**，然後按一下[版面配置]****。

   >[!NOTE]
   >
   >對貴組織使用的每個「頁面配置」（行銷、銷售等）重複步驟 連絡人、帳戶和機會物件。

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. 按一下&#x200B;**編輯**&#x200B;以變更銷售機會配置。

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. 按一下&#x200B;**Visualforce頁面**，然後將&#x200B;**潛在行動裝置**&#x200B;拖曳至行動卡區段。

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. 將高度變更為66並按一下[確定]。****

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. 按一下「**欄位**」，然後將「**新增至Marketo行銷活動**」拖曳至「**Marketo銷售分析**」區段。

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >在快速尋找中輸入「新增至」，以方便尋找新增至Marketo Campaign。

1. 按一下&#x200B;**保存**。

   ![](assets/image2015-4-22-18-3a1-3a56.png)

噢！ 您終於可以安裝Marketo Sales Insight for Salesforce1了！ 繼續操作，輕輕拍一下自己的後背。

>[!MORELIKETHIS]
>
>* [Salesforce中的首選1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* Salesforce中的[有趣時刻1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [在Salesforce中傳送Marketo電子郵件和行銷活動及監看清單動作1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
