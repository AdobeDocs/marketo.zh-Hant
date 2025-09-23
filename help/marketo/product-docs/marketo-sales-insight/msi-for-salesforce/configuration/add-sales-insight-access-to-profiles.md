---
description: 將銷售Insight存取權新增至設定檔 — Marketo檔案 — 產品檔案
title: 新增銷售洞察存取權至設定檔
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 1%

---

# 新增[!DNL Sales Insight]設定檔的存取權 {#add-sales-insight-access-to-profiles}

以下說明如何建立可存取[!DNL Sales Insight]的設定檔，同時移除其他設定檔的存取權。 適用於已安裝[[!DNL Sales Insight] AppExchange套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}的使用者。

>[!IMPORTANT]
>
>如果您先前已授予[!DNL Sales Insight]所有設定檔的存取權，您必須[移除設定檔層級的存取權](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"}才能使用此許可權集。

## 為[!DNL Sales Insight]建立新的設定檔 {#create-a-new-profile-for-sales-insight}

如果您有[!DNL Sales Insight]位使用者的專屬設定檔，則可略過此步驟。

1. 在[!DNL Salesforce]中，移至[設定]頁面。

1. 在快速尋找中搜尋設定檔，並選取&#x200B;**[!UICONTROL Profile]**&#x200B;選項。

1. 按一下頁面頂端的&#x200B;**[!UICONTROL New Profile]**&#x200B;按鈕。

1. 挑選要複製的設定檔並賦予其名稱(例如：Sales Insight User)。

1. 完成時，按一下&#x200B;**[!UICONTROL Save]**。

## 新增[!DNL Sales Insight]許可權 {#add-sales-insight-permissions}

1. 返回「設定檔」清單。

1. 按一下您剛建立之新設定檔的&#x200B;**[!UICONTROL Edit]**&#x200B;連結（或您要授予[!DNL Sales Insight]存取權的任何其他現有設定檔）。

1. 在編輯頁面上，您需要變更一些設定。

   **對於允許存取[!DNL Sales Insight]**&#x200B;的設定檔：

   * 在索引標籤設定中，將Marketo索引標籤變更為預設開啟
   * 在自訂物件許可權中，檢查[!DNL Marketo Sales Insight]設定上的讀取、建立、編輯和刪除（如果使用者應該擁有設定設定的存取權 — 通常用於管理員）

   **對於不允許存取[!DNL Sales Insight]**&#x200B;的設定檔：

   * 在索引標籤設定中，將Marketo索引標籤變更為隱藏索引標籤
   * 在自訂物件許可權中，取消核取[!DNL Marketo Sales Insight]設定上的讀取、建立、編輯和刪除

1. 完成時，按一下&#x200B;**[!UICONTROL Save]**。

## 建立[!DNL Sales Insight]的配置 {#create-layout-for-sales-insight}

1. 前往設定頁面，然後按一下&#x200B;**[!UICONTROL App Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Leads]** > **[!UICONTROL Page Layouts]**。 然後按一下&#x200B;**[!UICONTROL New]**&#x200B;按鈕。

1. 複製您選擇的版面，並為版面指定適當的名稱(例如： Sales Insight Layout)。

1. 完成時，按一下&#x200B;**[!UICONTROL Save]**。

1. 對您的[!UICONTROL Contacts]、[!UICONTROL Opportunities]和[!UICONTROL Accounts]版面配置重複這些步驟。

## 將設定檔指派給配置 {#assign-profile-to-layout}

1. 返回「頁面配置」區段，然後按一下「**[!UICONTROL Page Layout Assignment]**」按鈕。

1. 選取「**[!UICONTROL Edit Assignment]**」。

1. 從清單中選取您的[!DNL Sales Insight]設定檔，然後從&quot;[!DNL Sales insight]&quot;下拉式清單中選取您的[!UICONTROL Select Page Layout]配置。

1. 完成時，按一下&#x200B;**[!UICONTROL Save]**。

1. 對您的[!UICONTROL Contacts]、[!UICONTROL Opportunities]和[!UICONTROL Accounts]版面配置重複這些步驟。

## 其他變更 {#other-changes}

以下是可能出現[!DNL Sales Insight]個專案的其他地方。 您必須將其完全移除，因為您無法使用設定檔來限制其存取權：

* 從[!DNL Sales Insight]、[!UICONTROL Contacts]和[!UICONTROL Leads]的搜尋配置中移除[!UICONTROL Accounts]按鈕
* 從連絡人和潛在客戶清單移除[!DNL Sales Insight]欄
