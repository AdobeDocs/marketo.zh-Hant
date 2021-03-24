---
description: 為您的團隊設定銷售分析——行銷檔案——產品檔案
title: 為您的團隊設定銷售分析
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# 為您的團隊設定{#setting-up-sales-insight-for-your-team}的銷售分析

以下說明如何在移除其他個人檔案的存取權時，建立具有Sales Insight存取權的個人檔案。 這適用於已安裝[Sales InsightAppExchange套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)的使用者。

## 為Sales Insight {#create-a-new-profile-for-sales-insight}建立新的設定檔

如果您有專屬的Sales Insight使用者設定檔，則可略過此步驟。

1. 在Salesforce中，前往「設定」頁面。

1. 在「快速查找」中搜索配置檔案，然後選擇&#x200B;**Profile**&#x200B;選項。

1. 按一下頁面頂部的&#x200B;**New Profile**&#x200B;按鈕。

1. 選擇要克隆的配置檔案並為其命名(例如：Sales Insight使用者)。

1. 完成時，按一下「保存」。****

## 新增Sales Insight權限{#add-sales-insight-permissions}

1. 返回您的個人檔案清單。

1. 按一下您剛建立之新描述檔（或您想要讓Sales Insight存取的任何其他現有描述檔）的&#x200B;**編輯**&#x200B;連結。

1. 在編輯頁面上，您需要變更一些設定。

   **對於允許訪問Sales Insight的配置檔案**:

   * 在「自訂應用程式設定」中，勾選Marketto讓Marketo應用程式可見
   * 在「標籤設定」中，將「行銷人員」標籤變更為「預設開啟」
   * 在「自訂物件權限」中，勾選「在Marketo Sales Insight設定上讀取、建立、編輯和刪除」（如果使用者應擁有設定設定的存取權——通常用於管理員）

   **對於不允許存取Sales Insight的設定檔**:

   * 在「自訂應用程式設定」中，取消勾選「行銷人員」以隱藏Marketo應用程式
   * 在「標籤設定」中，將「行銷人員」標籤變更為「標籤隱藏」
   * 在「自訂物件權限」中，取消勾選「在Marketo Sales Insight設定上讀取、建立、編輯和刪除」


1. 完成時，按一下「保存」。****

## 建立Sales Insight {#create-layout-for-sales-insight}的版面

1. 前往「設定」頁面，然後按一下「應用程式設定」**>>「**&#x200B;自訂&#x200B;**>**&#x200B;銷售機會&#x200B;**>**&#x200B;頁面佈局」**。**&#x200B;然後，按一下&#x200B;**新建**&#x200B;按鈕。

1. 仿製您選擇的版面，並為版面指定適當的名稱(例如：銷售分析配置)。

1. 完成時，按一下「保存」。****

1. 對您的Contacts 、 Opportunity和Accounts的頁面佈局重複這些步驟。

## 將配置檔案分配給佈局{#assign-profile-to-layout}

1. 返回「頁面佈局」部分，然後按一下&#x200B;**「頁面佈局分配」按鈕。**

1. 選擇&#x200B;**編輯分配**。

1. 從清單中選取您的Sales Insight描述檔，然後從「選取頁面配置」下拉式清單中選取您的Sales Insight配置。

1. 完成時，按一下「保存」。****

1. 對您的Contacts 、 Opportunity和Accounts的頁面佈局重複這些步驟。

## 其他更改{#other-changes}

以下是Sales Insight項目可能出現的其他位置。 您必須直接移除這些檔案，因為您無法使用描述檔來限制其存取權：

* 從「搜尋連絡人」、「銷售線索」和「帳戶」的「版面」中移除「銷售分析」按鈕
* 從「聯繫人」和「銷售線索」清單中刪除Sales Insight列
