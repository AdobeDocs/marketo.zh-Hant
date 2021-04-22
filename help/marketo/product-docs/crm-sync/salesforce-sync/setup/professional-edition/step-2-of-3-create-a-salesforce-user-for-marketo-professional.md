---
unique-page-id: 3571797
description: 第2步（共3步）-為Marketo（專業）建立Salesforce用戶-Marketo文檔——產品文檔
title: 第2步（共3步）-為Marketo（專業）建立Salesforce使用者
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---

# 步驟2（共3步）:為Marketo（專業）{#step-of-create-a-salesforce-user-for-marketo-professional}建立Salesforce使用者

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>[步驟1（共3步）:將Marketo欄位新增至Salesforce（專業版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

在本文中，您將使用「Salesforce頁面配置」自訂欄位權限，並建立Marketo-Salesforce同步使用者。

## 設定頁面版面{#set-page-layouts}

Salesforce Professional會使用「頁面版面」來設定欄位層級的協助工具，而非Salesforce Enterprise/Unlimited的「設定檔」。 依照這些步驟，Marketo同步使用者可以更新自訂欄位。

1. 在Nav搜索欄中鍵入&#x200B;**頁面佈局**&#x200B;而不按&#x200B;**Enter**&#x200B;鍵，然後按一下&#x200B;**Leads**&#x200B;下的&#x200B;**頁面佈局**。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 按一下「Lead Layout（銷售線索佈局）」旁邊的「Edit ****」。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 按一下並拖曳新的&#x200B;**Section**&#x200B;至頁面版面。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 為&#x200B;**節名**&#x200B;輸入&quot;Marketo&quot;，然後按一下&#x200B;**確定**。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 按一下並拖曳欄位&#x200B;**贏取日期**&#x200B;至&#x200B;**Marketo**&#x200B;區段。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 對下列欄位重複上述步驟：

   * 贏取計畫
   * 贏取計畫ID
   * 選擇退出電子郵件
   * 推斷城市
   * 推斷公司
   * 推斷國家
   * 推斷的都市區
   * 推斷的電話區號
   * 推斷的郵遞區號
   * 推斷的州區
   * 潛在客戶分數
   * 原始反向連結
   * 原始搜尋引擎
   * 原始搜尋片語
   * 原始來源資訊
   * 原始來源類型

   >[!NOTE]
   >
   >這些欄位必須位於頁面版面中，以便Marketo能夠讀／寫。

   >[!TIP]
   >
   >拖曳至頁面右側，為欄位建立兩欄。 您可以將欄位從一側移至另一側，以平衡欄長。

1. 添加完欄位後，按一下&#x200B;**保存**。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 對Salesforce **連絡人頁面配置**&#x200B;重複上述所有步驟。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 完成&#x200B;**連絡頁面配置**&#x200B;操作後，請記得按一下&#x200B;**保存**。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >請確定&#x200B;**全天事件**&#x200B;欄位已新增至&#x200B;**事件頁面配置**。

## 建立同步用戶{#create-sync-user}

Marketo需要具備存取Salesforce的認證。 使用以下步驟建立的專用使用者，最好能完成此作業。

>[!NOTE]
>
>如果您的組織沒有額外的Salesforce授權，您可以使用現有的&#x200B;**行銷使用者**&#x200B;搭配&#x200B;**系統管理員**&#x200B;設定檔。

1. 在導航搜索欄中輸入&quot;users&quot;，然後按一下&#x200B;**管理用戶**&#x200B;下的&#x200B;**用戶**。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 按一下「**新用戶**」。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填寫必填欄位，選擇&#x200B;**使用者授權：Salesforce**，設定&#x200B;**設定檔：系統管理員**，勾選&#x200B;**行銷使用者**，然後按一下&#x200B;**儲存**。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >請確定您輸入的電子郵件地址有效。 您必須以同步使用者身分登入，才能重設密碼。

太棒了！ 現在，您有一個帳戶可讓Marketo用來連線至Salesforce。 我們來吧。

>[!MORELIKETHIS]
>
>[步驟3（共3步）:連接Marketo和Salesforce（專業版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
