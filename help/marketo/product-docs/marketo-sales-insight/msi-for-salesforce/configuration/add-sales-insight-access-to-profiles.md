---
description: 添加Sales Insight訪問配置檔案 — Marketo文檔 — 產品文檔
title: 將Sales Insight訪問權添加到配置檔案
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 將Sales Insight訪問權添加到配置檔案 {#add-sales-insight-access-to-profiles}

下面是如何在刪除對其他配置檔案的訪問權限時建立具有Sales Insight訪問權限的配置檔案。 這適用於已安裝 [Sales InsightAppExchange包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}。

>[!IMPORTANT]
>
>如果您以前已授予Sales Insight對所有配置檔案的訪問權限，則必須 [刪除配置檔案級別訪問](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;}可使用此權限集。

## 為Sales Insight建立新配置檔案 {#create-a-new-profile-for-sales-insight}

如果您的Sales Insight用戶有專用的配置檔案，則可以跳過此步驟。

1. 在Salesforce中，轉到「設定」頁。

1. 在「快速查找」中搜索配置檔案，然後選擇 **配置檔案** 的雙曲餘切值。

1. 按一下 **新建配置檔案** 按鈕。

1. 選擇要克隆的配置檔案並為其指定名稱(例如：Sales Insight用戶)。

1. 按一下 **保存** 完成。

## 添加Sales Insight權限 {#add-sales-insight-permissions}

1. 返回到您的配置式清單。

1. 按一下 **編輯** 連結，用於您剛建立的新配置檔案（或您希望為Sales Insight授予訪問權限的任何其他現有配置檔案）。

1. 在編輯頁面上，您需要更改一些設定。

   **對於允許訪問Sales Insight的配置檔案**:

   * 在頁籤設定中，將Marketo頁籤更改為預設開啟
   * 在自定義對象權限中，選中MarketoSales Insight配置上的讀取、建立、編輯和刪除（如果用戶應有權訪問配置設定 — 通常用於管理員）

   **對於不允許訪問Sales Insight的配置檔案**:

   * 在頁籤設定中，將Marketo頁籤更改為頁籤隱藏
   * 在自定義對象權限中，取消選中MarketoSales Insight配置上的讀取、建立、編輯和刪除


1. 按一下 **保存** 完成。

## 為Sales Insight建立佈局 {#create-layout-for-sales-insight}

1. 轉到「設定」頁，然後按一下 **應用程式設定** > **自定義** > **銷售線索** > **頁面佈局**。 然後按一下 **新建** 按鈕

1. 克隆所選佈局並為佈局指定適當的名稱(例如：Sales Insight佈局)。

1. 按一下 **保存** 完成。

1. 對Contacts 、 Opportunity和Accounts的頁面佈局重複這些步驟。

## 將配置檔案分配給佈局 {#assign-profile-to-layout}

1. 返回「頁面佈局」部分，然後按一下 **頁面佈局分配** 按鈕

1. 選擇 **編輯分配**。

1. 從清單中選擇您的Sales Insight配置檔案，然後從「選擇頁面佈局」下拉清單中選擇您的Sales Insight佈局。

1. 按一下 **保存** 完成。

1. 對Contacts 、 Opportunity和Accounts的頁面佈局重複這些步驟。

## 其他更改 {#other-changes}

下面是Sales Insight項目可能出現的其他位置。 您必須直接刪除它們，因為您不能使用配置檔案來限制其訪問：

* 從聯繫人、銷售線索和帳戶的搜索佈局中刪除Sales Insight按鈕
* 從聯繫人和潛在客戶清單中刪除Sales Insight列
