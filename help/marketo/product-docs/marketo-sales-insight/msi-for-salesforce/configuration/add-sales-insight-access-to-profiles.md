---
description: 將Sales Insight存取新增至設定檔 — Marketo檔案 — 產品檔案
title: 將Sales Insight存取權新增至設定檔
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 將Sales Insight存取權新增至設定檔 {#add-sales-insight-access-to-profiles}

以下說明如何在移除其他設定檔的存取權時，建立具有Sales Insight存取權的設定檔。 這適用於已安裝 [Sales InsightAppExchange套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}。

>[!IMPORTANT]
>
>如果您先前已授予Sales Insight所有設定檔的存取權，則您必須 [移除設定檔層級存取權](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;}使用此權限集。

## 建立Sales Insight的新設定檔 {#create-a-new-profile-for-sales-insight}

如果您有專屬的Sales Insight使用者設定檔，則可略過此步驟。

1. 在Salesforce中，轉至「設定」頁面。

1. 在快速查找中搜索配置檔案，並選擇 **設定檔** 選項。

1. 按一下 **新設定檔** 按鈕。

1. 選擇要克隆的配置檔案並為其命名(例如：銷售分析用戶)。

1. 按一下 **儲存** 時才能使用。

## 添加Sales Insight權限 {#add-sales-insight-permissions}

1. 返回您的設定檔清單。

1. 按一下 **編輯** 您剛建立的新設定檔的連結（或您要授予Sales Insight存取權的任何其他現有設定檔）。

1. 在編輯頁面上，您需要變更一些設定。

   **對於允許訪問Sales Insight的配置檔案**:

   * 在「標籤設定」中，將Marketo標籤變更為「預設開啟」
   * 在「自訂物件權限」中，勾選「Marketo銷售分析設定」的「讀取」、「建立」、「編輯」和「刪除」（如果使用者應有權存取設定設定，則通常用於管理員）

   **對於不能訪問Sales Insight的配置檔案**:

   * 在「標籤設定」中，將Marketo標籤變更為「標籤隱藏」
   * 在「自訂物件權限」中，取消勾選「Marketo Sales Insight設定」上的「讀取」、「建立」、「編輯」和「刪除」


1. 按一下 **儲存** 時才能使用。

## 建立Sales Insight的佈局 {#create-layout-for-sales-insight}

1. 前往「設定」頁面，然後按一下 **應用程式設定** > **自訂** > **銷售機會** > **頁面配置**. 然後按一下 **新增** 按鈕。

1. 複製您選擇的版面，並為版面命名適當的名稱(例如：銷售分析配置)。

1. 按一下 **儲存** 時才能使用。

1. 對您的「聯繫人」、「業務機會」和「帳戶」的頁面佈局重複這些步驟。

## 將設定檔指派給配置 {#assign-profile-to-layout}

1. 返回「頁面配置」區段，然後按一下 **頁面佈局分配** 按鈕。

1. 選擇 **編輯分配**.

1. 從清單中選擇您的Sales Insight配置檔案，然後從「選擇頁面配置」下拉式清單中選擇您的Sales Insight配置。

1. 按一下 **儲存** 時才能使用。

1. 對您的「聯繫人」、「業務機會」和「帳戶」的頁面佈局重複這些步驟。

## 其他變更 {#other-changes}

以下是「銷售分析」項目可能出現的其他位置。 您必須直接移除這些設定檔，因為您無法使用設定檔來限制其存取權：

* 從「搜索聯繫人」、「銷售機會」和「帳戶」的「佈局」中刪除「銷售分析」按鈕
* 從聯繫人和潛在客戶清單中刪除Sales Insight列
