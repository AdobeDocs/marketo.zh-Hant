---
description: 步驟3之2 — 建立Marketo的Salesforce使用者(Enterprise/Unlimited) - Marketo檔案 — 產品檔案
title: 步驟3之2 — 建立Marketo的Salesforce使用者(Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 1%

---

# 步驟2之3：建立Marketo的Salesforce使用者(Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>[步驟3之1：將Marketo欄位新增至Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

在本文中，您將會在Salesforce設定檔中設定使用者許可權，並建立Marketo-Salesforce整合帳戶。

## 建立設定檔 {#create-a-profile}

1. 按一下&#x200B;**[!UICONTROL 設定]**。

   熒幕擷圖

1. 在導覽搜尋列中輸入「設定檔」，然後按一下「設定檔」連結。

   熒幕擷圖

1. 按一下「新增設定檔」。

   熒幕擷圖

1. 選取「標準使用者」，將設定檔命名為「Marketo-Salesforce同步」，然後按一下「儲存」。

   熒幕擷圖

## 設定設定檔許可權 {#set-profile-permissions}

1. 按一下「編輯」以設定安全性許可權。

   熒幕擷圖

1. 在「管理許可權」區段下，確定已勾選下列方塊：

   * API已啟用
   * 編輯HTML範本
   * 管理公開檔案
   * 管理公開範本

   >[!TIP]
   >
   >請務必勾選「密碼永不過期」方塊。

1. 在「一般使用者許可權」區段下，確定已勾選下列方塊：

   * 轉換潛在客戶
   * 編輯事件
   * 編輯任務

1. 在「標準物件許可權」區段下，確定已勾選「讀取」、「建立」、「編輯」和「刪除」許可權：

   * 帳戶
   * 行銷活動
   * 連絡人
   * 銷售機會
   * 機會

   >[!NOTE]
   >
   >如果您打算使用Campaign Sync，請授與Campaigns的許可權。

   熒幕擷圖

1. 完成後，按一下頁面底部的「儲存」 。

   熒幕擷圖

## 設定欄位許可權 {#set-field-permissions}

1. 與您的行銷人員討論，找出同步所需的自訂欄位。

   >[!NOTE]
   >
   >此步驟將防止您不需要的欄位顯示在Marketo中，這將減少雜亂並加快同步速度。

1. 在設定檔詳細資訊頁面中，移至欄位層級安全性區段。 按一下檢視來編輯物件的協助工具：

   * 銷售機會
   * 連絡人
   * 帳戶
   * 機會

   >[!TIP]
   >
   >您可以根據組織的需求設定其他物件。

1. 對於每個物件，按一下「編輯」。

   熒幕擷圖

1. 找出不需要的欄位，確定未勾選「讀取存取權」和「編輯存取權」 。 完成時，按一下「儲存」 。

   >[!NOTE]
   >
   >僅編輯自訂欄位的協助工具。

   熒幕擷圖

1. 停用完所有不需要的欄位後，您必須核取下列物件欄位的「讀取存取權」和「編輯存取權」。 完成時，按一下「儲存」 。

   表格

   熒幕擷圖

## 建立Marketo-Salesforce同步帳戶 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>建立專用的Salesforce帳戶（例如`marketo@yourcompany.com`），以區分Marketo與其他Salesforce使用者所做的變更。

1. 在導覽搜尋列中輸入「管理使用者」，然後按一下「使用者」。 按一下「新增使用者」。

   熒幕擷圖

   熒幕擷圖

1. 填寫必填欄位。 接著，選取使用者授權： Salesforce和您先前建立的設定檔。 完成後，按一下「儲存」 。

   熒幕擷圖

步驟3之2已完成。
