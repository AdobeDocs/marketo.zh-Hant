---
description: 步驟3之1 — 將Marketo欄位新增至Salesforce (Enterprise/Unlimited) - Marketo檔案 — 產品檔案
title: 步驟3之1 — 將Marketo欄位新增至Salesforce (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 步驟3之1：將Marketo欄位新增至Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>您必須有權存取Salesforce API，才能在Marketo Engage與Salesforce之間同步。

Marketo使用一組欄位來擷取特定型別的行銷相關資訊。 如果您想在Salesforce中使用此資料，請遵循下列指示。

1. 在潛在客戶和聯絡物件的Salesforce中建立三個自訂欄位：分數、贏取方案和贏取日期。
1. 在潛在客戶與聯絡人之間對應這些自訂欄位，以便在Salesforce中進行轉換時值能延續。
1. 如有需要，您可以建立其他欄位（請參閱下表）。

所有這些自訂欄位都是選用欄位，不需要用來同步Marketo和Salesforce。 根據最佳實務，建議您建立「分數」、「贏取方案」和「贏取日期」欄位。

## 將Marketo欄位新增至Salesforce {#add-marketo-fields-to-salesforce}

在以上列出的Salesforce中的潛在客戶與聯絡人物件上，新增三個自訂欄位。 如果您想要新增更多欄位，請參閱本區段末尾的可用欄位表。

對三個自訂欄位中的每一個執行以下步驟以新增它們。 從分數開始。

1. 登入Salesforce並按一下「設定」。

   熒幕擷圖

1. 在「快速尋找」中，搜尋「物件」一詞

   熒幕擷圖

1. 按一下「物件管理員」並搜尋「銷售機會」

   熒幕擷圖

1. 按一下LABEL底下的Lead ，然後按一下左邊的Fields and Relationships。

   熒幕擷圖

1. 按一下「欄位和關係」頁面中名為「新增」的按鈕

   熒幕擷圖

1. 選擇適當的欄位型別（「分數 — 數字」、「贏取方案 — 文字」、「贏取日期 — 日期/時間」）。

   熒幕擷圖

1. 按一下「下一步」。

   熒幕擷圖

1. 輸入欄位的「欄位標籤」、「長度」和「欄位名稱」，如下表所示。

   表格

   >[!NOTE]
   >
   >Salesforce在用來建立API名稱時，會將__c附加至欄位名稱。

   熒幕擷圖

   >[!NOTE]
   >
   >文字和數字欄位需要長度，但日期/時間欄位不需要。說明為選用。

1. 按一下「下一步」。

   熒幕擷圖

1. 指定存取設定，然後按下一步：

   將所有角色設定為可見和唯讀

   清除同步使用者設定檔的「唯讀」核取方塊：

   如果您的使用者具有系統管理員的設定檔作為同步使用者，請清除系統管理員設定檔的唯讀核取方塊（如下所示）
如果您已建立同步處理使用者的自訂設定檔，請清除該自訂設定檔的「唯讀」核取方塊

   熒幕擷圖

1. 選擇應顯示欄位的頁面配置。

   熒幕擷圖

1. 按一下「儲存並新增」以返回並建立其他兩個自訂欄位。 按一下「儲存」 ，您已全部完成這三項。

   熒幕擷圖

* 在「物件管理員」中，搜尋「連絡人」。 按一下「欄位和關係」。
* 對連絡人物件的「分數」、「贏取日期」和「贏取方案」欄位，執行步驟5到12，就像您對潛在客戶物件所做的一樣。
* 或者，您可以將此程式用於此表格的任何其他自訂欄位。

  表格

  >[!NOTE]
  >
  >建立新欄位後，Marketo自動指派的欄位值將無法立即在Salesforce中使用。 下次更新任一系統上的記錄時(即更新任何在Salesforce和Marketo之間同步的欄位)，Marketo會將資料同步至Salesforce。

## 對應自訂欄位以進行轉換 {#map-custom-fields-for-conversions}

Salesforce中潛在客戶物件上的自訂欄位應對應至聯絡人物件上的聯絡人欄位，以便在轉換發生時保留資料。

1. 按一下右上角的「設定」。

   熒幕擷圖

1. 在「快速尋找」中，搜尋「物件」一詞

   熒幕擷圖

1. 前往「銷售機會自訂欄位和關係」區段，然後按一下「對應銷售機會欄位」

   熒幕擷圖

1. 按一下您要對應的欄位旁的下拉式清單，位於對應的索引標籤 — 帳戶、聯絡人或機會下方。

   熒幕擷圖

1. 選取對應的連絡人自訂欄位。

   熒幕擷圖

1. 對您已建立的任何其他欄位重複上述步驟。

1. 完成時，按一下「儲存」 。
