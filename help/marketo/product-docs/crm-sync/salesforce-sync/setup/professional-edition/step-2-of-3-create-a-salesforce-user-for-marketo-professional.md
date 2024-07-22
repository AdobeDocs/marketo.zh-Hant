---
unique-page-id: 3571797
description: 步驟3之2 — 建立Marketo （專業）的Salesforce使用者 — Marketo檔案 — 產品檔案
title: 步驟3之2 — 建立Marketo的Salesforce使用者（專業）
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 8%

---

# 步驟3之2：建立Marketo的Salesforce使用者（專業） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成。

>[!PREREQUISITES]
>
>[步驟3之1：將Marketo欄位新增至Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

在本文中，您將使用「Salesforce頁面配置」來自訂欄位許可權，並建立Marketo-Salesforce同步使用者。

## 設定頁面配置 {#set-page-layouts}

Salesforce Professional會以頁面配置設定欄位層級協助工具，而非Salesforce Enterprise/Unlimited的設定檔。 按照以下步驟操作將允許Marketo同步使用者更新自訂欄位。

1. 在導覽搜尋列中輸入&#39;&#39;[!UICONTROL &#39;&#39;頁面配置]&#39;&#39;，不按&#x200B;**[!UICONTROL Enter]**，然後按一下&#x200B;**[!UICONTROL 銷售機會]**&#x200B;下的&#x200B;**[!UICONTROL &#39;頁面配置]**。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 按一下潛在客戶配置旁的&#x200B;**[!UICONTROL 編輯]**。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 按一下並將新的&#x200B;**[!UICONTROL 區段]**&#x200B;拖曳到版面配置中。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 輸入&#x200B;**[!UICONTROL 區段名稱]**&#x200B;的「Marketo」並按一下&#x200B;**[!UICONTROL 確定]**。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 按一下並拖曳欄位&#x200B;**[!UICONTROL 贏取日期]**&#x200B;至&#x200B;**Marketo**&#x200B;區段。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 對下列欄位重複上述步驟：

   * 贏取方案
   * 贏取方案ID
   * 電子郵件選擇退出
   * 推斷的城市
   * 推斷公司
   * 推斷國家
   * 推斷的大都會區
   * 推斷的電話區碼
   * 推斷的郵遞區號
   * 推斷的州別區域
   * 銷售機會分數
   * 原始反向連結
   * 原始搜尋引擎
   * 原始搜尋片語
   * 原始來源資訊
   * 原始來源類型

   >[!NOTE]
   >
   >這些欄位必須位於頁面配置中，Marketo才能讀取/寫入這些欄位。

   >[!TIP]
   >
   >向下拖曳至頁面右側，為欄位建立兩欄。 您可以將欄位從一側移動到另一側，以平衡欄長度。

1. 完成新增欄位時，按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 對Salesforce **[!UICONTROL 連絡人頁面配置]**&#x200B;重複上述所有步驟。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 完成&#x200B;**[!UICONTROL 連絡人頁面配置]**&#x200B;時，請記得按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >確定已將&#x200B;**[!UICONTROL 全天事件]**&#x200B;欄位新增至&#x200B;**[!UICONTROL 事件頁面配置]**。

## 建立同步使用者 {#create-sync-user}

Marketo需要認證才能存取Salesforce。 建議您先透過下列步驟建立專屬使用者，再完成這項工作。

>[!NOTE]
>
>如果您的組織沒有其他Salesforce授權，您可以使用具有系統管理員設定檔的現有行銷使用者。

1. 在導覽搜尋列中輸入「使用者」，然後按一下&#x200B;**[!UICONTROL 管理使用者]**&#x200B;底下的&#x200B;**[!UICONTROL 使用者]**。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 按一下&#x200B;**[!UICONTROL 新增使用者]**。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填寫必填欄位，選取&#x200B;**[!UICONTROL 使用者授權： Salesforce]**，設定&#x200B;**[!UICONTROL 設定檔：系統管理員]**，勾選&#x200B;**[!UICONTROL 行銷使用者]**，然後按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >請確定您輸入的電子郵件地址有效。 您必須以同步處理使用者身分登入，才能重設密碼。

太好了！ 現在您已擁有Marketo可用來連線至Salesforce的帳戶。 開始吧。

>[!MORELIKETHIS]
>
>[步驟3之3：連線Marketo與Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
