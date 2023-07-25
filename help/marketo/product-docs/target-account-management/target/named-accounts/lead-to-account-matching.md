---
unique-page-id: 11381156
description: 銷售線索帳戶比對 — Marketo檔案 — 產品檔案
title: 銷售線索與帳戶的比對
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# 銷售線索與帳戶的比對 {#lead-to-account-matching}

使用Marketo銷售線索與帳戶的比對，將右側銷售線索與右側具名帳戶進行比對。

>[!NOTE]
>
>**銷售線索與帳戶的比對** 是Marketo Target帳戶管理的內建功能。 它會使用模糊邏輯，以幾近即時的方式自動比對銷售線索與正確的具名帳戶。 這些具名帳戶可以是CRM帳戶或Marketo公司。

## 概觀 {#overview}

Marketo銷售線索與帳戶的比對會遵循4個步驟的程式：

**步驟1 -** 我們的比對程式從使用潛在客戶記錄上的關鍵資訊開始，例如：

* 電子郵件網域(例如，acme.com)
* 從IP位址推斷出的公司名稱
* 公司名稱 — 這可以是CRM帳戶名稱或潛在客戶公司名稱屬性（例如，來自表單填寫）

**步驟2 -** 我們根據各種潛在客戶屬性（例如Acme Inc.和Acme Corp會自動標準化為Acme），將找到的公司名稱標準化。 此步驟可確保在Marketo中擁有已命名帳戶的單一表示法，且可檢視單一已命名帳戶內的所有銷售機會。

**步驟3 -** 我們將相符的潛在客戶分割為2個貯體：強相符和弱相符的。

* 不相符的潛在客戶會出現在已命名的帳戶上，然後可以手動加以解析。

**步驟4 -** 我們提供一份強弱相符的建議公司清單。 當根據其中一家建議的公司建立具名帳戶時，我們會建立比對規則，以自動將新的銷售機會（例如，填寫表單的銷售機會）與正確的具名帳戶建立關聯。 這樣一來，您就不用再擔心銷售機會配對了，更不用擔心收入問題！

由於Marketo銷售線索與帳戶的比對是Marketo Target帳戶管理的一項內建功能，所以銷售線索與帳戶的比對幾乎是即時發生的(例如，當銷售線索填寫Marketo表單時，我們會將所述的銷售線索與正確的命名帳戶建立關聯)。 此事件可用來觸發警報，並通知帳戶擁有者有新的潛在客戶從他們指定的帳戶進入。

>[!NOTE]
>
>如果您使用Salesforce中的LeanData來執行銷售線索與帳戶的比對，Marketo已整合，可將符合的專案同步至您的Marketo執行個體。 若要啟用該功能，請聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support) 瞭解如何在下方設定LeanData。

## 使用LeanData進行銷售線索與帳戶的比對 {#using-leandata-for-lead-to-account-matching}

晚於 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support) 已為您的帳戶啟用LeanData，請依照下列步驟進行設定。

1. 在Salesforce中，按一下 **設定首頁** 左側導覽中找到。

1. 仍然在左側導覽中的「管理」下方，按一下 **使用者** 則 **設定檔**.

1. 找到並選取 **Marketo同步** 設定檔。

1. 向下捲動至「欄位層級安全性」區段，並找出Lead物件。 選取 **檢視**.

1. 對於欄位名稱「報表比對帳戶」，請確認 **讀取許可權** 欄已選取。

1. 在Marketo中，前往 **管理員** 區段。

   ![](assets/lead-to-account-matching-1.png)

1. 選取 **欄位管理**.

   ![](assets/lead-to-account-matching-2.png)

1. 透過搜尋「報表相符的帳戶」來確認欄位存在。

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[探索帳戶](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
