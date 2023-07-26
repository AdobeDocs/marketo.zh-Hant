---
description: 將銷售分析存取權新增至設定檔 — Marketo檔案 — 產品檔案
title: 將銷售分析存取權新增至設定檔
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 將銷售分析存取權新增至設定檔 {#add-sales-insight-access-to-profiles}

以下說明如何建立可存取Sales Insight的設定檔，同時移除其他設定檔的存取權。 適用於已安裝 [銷售分析AppExchange套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>如果您先前已授予Sales Insight存取所有設定檔的許可權，則必須 [移除設定檔層級的存取權](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} 以使用此許可權集。

## 建立Sales Insight的新設定檔 {#create-a-new-profile-for-sales-insight}

如果您的Sales Insight使用者有專屬的設定檔，則可略過此步驟。

1. 在Salesforce中，前往「設定」頁面。

1. 在「快速尋找」中搜尋設定檔，並選取 **個人資料** 選項。

1. 按一下 **新設定檔** 按鈕來切換頁面。

1. 挑選要複製的設定檔並賦予其名稱（例如：銷售分析使用者）。

1. 按一下 **儲存** 完成時。

## 新增Sales Insight許可權 {#add-sales-insight-permissions}

1. 返回「設定檔」清單。

1. 按一下 **編輯** 連結至您剛建立的新設定檔（或您要授與Sales Insight存取權的任何其他現有設定檔）。

1. 在編輯頁面上，您需要變更一些設定。

   **針對允許存取銷售分析的個人檔案**：

   * 在索引標籤設定中，將Marketo索引標籤變更為預設開啟
   * 在「自訂物件許可權」中，勾選Marketo Sales Insight Config上的「讀取」、「建立」、「編輯」和「刪除」 （如果使用者應具有組態設定的存取權 — 通常用於管理員）

   **針對不允許存取Sales Insight的設定檔**：

   * 在索引標籤設定中，將Marketo索引標籤變更為隱藏索引標籤
   * 在「自訂物件許可權」中，取消勾選「Marketo銷售分析設定」的「讀取」、「建立」、「編輯」和「刪除」

1. 按一下 **儲存** 完成時。

## 建立Sales Insight的版面 {#create-layout-for-sales-insight}

1. 前往「設定」頁面，然後按一下 **應用程式設定** > **自訂** > **銷售機會** > **頁面配置**. 然後按一下 **新增** 按鈕。

1. 複製您選擇的版面，並為版面提供適當的名稱（例如： Sales Insight Layout）。

1. 按一下 **儲存** 完成時。

1. 對您的「連絡人」、「商機」和「帳戶」的頁面配置重複這些步驟。

## 將設定檔指派給配置 {#assign-profile-to-layout}

1. 返回「頁面配置」區段，然後按一下 **頁面配置指派** 按鈕。

1. 選取 **編輯指派**.

1. 從清單中選取您的銷售分析設定檔，然後從「選取頁面配置」下拉式清單中選取您的銷售分析配置。

1. 按一下 **儲存** 完成時。

1. 對您的「連絡人」、「商機」和「帳戶」的頁面配置重複這些步驟。

## 其他變更 {#other-changes}

以下是其他可能出現銷售分析專案的位置。 您必須將其完全移除，因為您無法使用設定檔來限制其存取權：

* 從連絡人、潛在客戶及帳戶的搜尋配置中移除銷售分析按鈕
* 從連絡人和潛在客戶清單中移除Sales Insight欄
