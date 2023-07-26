---
unique-page-id: 14352475
description: 在活動歷程記錄上安裝Sales Connect事件欄位 — Marketo檔案 — 產品檔案
title: 在活動歷史記錄上安裝Sales Connect事件欄位
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 在活動歷史記錄上安裝Sales Connect事件欄位 {#install-sales-connect-event-fields-on-activity-history}

將Enterprise套件安裝到Salesforce中後，您就可以將Sales Connect事件欄位安裝到活動歷史記錄區段中。 Sales Connect事件欄位包含檢視、點按和促銷活動等資訊。 這可讓您擁有直接匯入Salesforce之電子郵件的相關資訊。

執行這些步驟時，請務必與Salesforce管理員組成團隊。 在此範例中，我們會將欄位安裝至 **潛在客戶頁面配置**. 您也可以將欄位安裝到Contact、Account和Opportunity頁面配置中。 請記住，將電子郵件記錄至帳戶和機會時，您將需要您正在以電子郵件傳送的連絡人角色關聯。

1. 按一下 **設定**.
1. 按一下 **自訂**.
1. 按一下 **銷售機會**.
1. 按一下 **頁面配置**.
1. 按一下 **編輯** 在您要變更的頁面配置旁邊。

   >[!NOTE]
   >
   >Sales Connect會為您安裝一些版面配置，但如果您已有預設版面配置供您的團隊使用，您會想要在那裡安裝。 如果您不想使用Sales Connect頁面配置，可以將其刪除。

1. 向下捲動至「活動歷史記錄」區段。
1. 按一下扳手以進行編輯。
1. 選取您要包含在Activity History區段中的Sales Connect欄位。 如果您未在此處看到Sales Connect欄位，表示您可能安裝了錯誤的Salesforce套件。
1. 按一下 **新增** 以移動所需欄位。
1. 按一下 **確定**.
1. 按一下 **儲存**.

   您的使用者現在可以在Salesforce中檢視有關其電子郵件的重要資訊和更新！
