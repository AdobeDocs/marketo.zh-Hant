---
unique-page-id: 6848747
description: 角色許可權說明 — Marketo檔案 — 產品檔案
title: 角色許可權說明
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
feature: Users and Roles
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# 角色許可權說明 {#descriptions-of-role-permissions}

以下是您可以指派給角色的所有可用許可權清單。 許可權通常與Marketo內的特定功能區域相關聯，並可協助您控制不同使用者可存取的區域和功能。

關於許可權的其他資訊：

* 「存取」許可權可授予角色檢視和編輯應用程式該部分的許可權。
* 若要讓角色擁有子許可權（「建立」、「刪除」等）的存取權，該角色必須擁有該部分應用程式的「存取權」。 例如，如果您想要授與某人「編輯促銷活動」的許可權，該人員必須擁有存取行銷活動的整體許可權。
* 您可能會看到您沒有許可權使用的動作或資產。 但是，如果您嘗試存取這些檔案，將會看到一則訊息，警告您存取許可權受限。

## 可用許可權 {#available-permissions}

當您 [建立或編輯角色](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)，您可以核取適當的方塊，選取下列哪個許可權可允許該角色。

![](assets/descriptions-of-role-permissions-1.png)

## 存取管理員  {#access-admin}

在「管理員」的「我的帳戶」區段中檢視設定並進行變更。

* 存取稽核軌跡 — 可讓使用者存取資產稽核軌跡和管理稽核軌跡
* 存取頻道 — 僅授予使用者修改頻道標籤的存取權，不授予其他自訂標籤
* 存取通訊限制 — 提供使用者存取權，以便在「管理員」中啟用通訊限制
* 存取CRM — 提供使用者對CRM的存取權，例如 [!DNL Salesforce] 或 [!DNL Microsoft Dynamics]，在管理員中
* 存取 [[!DNL Data.com]](https://Data.com)  — 提供使用者存取Data.com流程動作的許可權
* 存取電子郵件管理員 — 提供使用者電子郵件管理員以變更預設設定，例如取消訂閱和品牌化網域
* 存取事件合作夥伴 — 讓使用者在管理員中存取LaunchPoint
* 存取欄位管理 — 提供使用者存取管理員欄位管理的許可權
* 存取檔案上傳 — 讓使用者能夠將影像和檔案上傳到Design Studio
* 存取登陸頁面 — 提供使用者在Admin中存取登陸頁面的許可權
* 存取位置 — 可讓使用者存取管理員中的位置，以設定預設語言、地區設定、時區和貨幣
* 存取登入歷史記錄 — 可讓使用者存取稽核軌跡中的使用者登入歷史記錄
* 存取登入設定 — 讓使用者可存取管理員中的登入設定，包括安全性、IP限制和智慧列示報表設定
* 存取Marketo自訂活動 — 讓使用者能在「管理員」中存取Marketo自訂活動
* 存取Marketo自訂物件 — 讓使用者能夠在「管理員」中存取Marketo自訂物件
* 存取 [!DNL Munchkin]  — 使用者存取許可權： [!DNL Munchkin] 在管理員中，用於設定追蹤代碼、人員追蹤及啟用API設定
* 存取Revenue Cycle Analytics — 讓使用者能夠存取Admin中的Revenue Cycle Analytics，以設定同步摘要和歸因
* 存取角色 — 提供使用者管理和編輯角色的存取權，但不提供使用者
* 存取銷售分析 — 可讓使用者存取管理中的銷售分析，用於設定狀態、API設定、人員評分和其他設定
* 存取單一登入 — 提供使用者在Admin中管理單一登入的存取權，可啟用SAML並使用SAML設定和重新導向頁面URL
* 存取Smart Campaign — 讓使用者可存取Admin中的Smart Campaign，以限制合格人員的限制
* 存取SOAP API — 讓使用者能夠在Admin中管理網站服務中的SOAP API
* 存取標籤 — 讓使用者可存取所有自訂標籤，但通道標籤除外
* 存取Treasure Check — 讓使用者在Admin中存取Treasure Check的實驗功能
* 存取使用者 — 提供使用者在管理員中編輯和管理使用者（而非角色）的存取權
* 存取Webhook — 為使用者提供Admin中的Webhook，用於設定詳細資料和回應對應
* 存取工作區和分割區 — 提供使用者在Admin中建立、編輯和刪除工作區和分割區的存取權

## Access API  {#access-api}

為使用者提供 **僅限API** **角色** 存取下列個別API。

* 核准資產
* 執行行銷活動
* 唯讀活動
* 唯讀活動中繼資料
* 唯讀資產
* 唯讀行銷活動
* 唯讀公司
* 唯讀自訂物件
* 唯讀人員
* 唯讀具名帳戶
* 唯讀機會
* 唯讀銷售人員
* 讀寫活動
* 讀寫活動中繼資料
* 讀寫資產
* 讀寫行銷活動
* 讀寫公司
* 讀寫自訂物件
* 讀寫人員
* 讀寫具名帳戶
* 讀寫機會
* 讀寫銷售人員

## 存取Analytics {#access-analytics}

讓使用者能存取Analytics標籤、電子郵件分析、報表及以下三個專案（未勾選者除外）。

* 存取Revenue Explorer — 取消核取將移除使用者對Revenue Explorer的存取權
* 刪除報告 — 取消核取將移除使用者刪除報告的能力
* 匯出Analytics資料 — 取消勾選會移除使用者匯出Analytics資料的能力

## 存取行事曆Presentations {#access-calendar-presentations}

讓使用者能存取行事曆簡報 — 在底部顯示Presentations按鈕。

* 編輯行事曆Presentations — 讓使用者能在行事曆中編輯簡報

## 存取Design Studio {#access-design-studio}

可讓使用者存取Design Studio標籤和樹狀檢視，但無法存取詳細資訊。

* 存取電子郵件
   * 編輯電子郵件 — 提供使用者編輯、建立和複製電子郵件的許可權
      * 讓電子郵件運作 — 授予使用者讓電子郵件運作的許可權。 請參閱： [讓電子郵件運作正常](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * 核准電子郵件 — 讓使用者可核准電子郵件。
      * 刪除電子郵件 — 讓使用者可以刪除電子郵件。
      * 設定品牌領域 — 讓使用者能夠使用品牌領域。 請參閱： [新增其他品牌網域](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* 存取電子郵件範本

   * 核准電子郵件範本
   * 刪除電子郵件範本
   * 編輯電子郵件範本 — 編輯、建立和複製電子郵件範本

* 存取表單

   * 核准表單
   * 刪除表單
   * 編輯表單 — 編輯、建立和複製表單

* 存取影像

   * 刪除影像
   * 上傳影像

* 存取登陸頁面

   * 核准登陸頁面
   * 刪除登陸頁面
   * 編輯登陸頁面 — 編輯、建立和複製登陸頁面

* 存取登入頁面範本

   * 核准登陸頁面範本
   * 刪除登入頁面範本
   * 編輯登入頁面範本 — 編輯、建立和複製登入頁面範本

* 存取代碼片段

   * 核准程式碼片段
   * 刪除程式碼片段
   * 編輯代碼片段

* 存取社交應用程式

   * 核准社交應用程式
   * 刪除社交應用程式
   * 編輯社交應用程式

## Access資料庫 {#access-database}

檢視資料庫，以及檢視和編輯智慧/靜態清單。

* 存取區段

   * 核准分段
   * 刪除分段
   * 編輯分段

* 刪除人員
* 刪除清單
* 編輯人員 — 防止手動編輯和執行單一流程步驟；您仍然可以透過執行行銷活動來編輯人員
* Export Person — 從您的資料庫清單匯出試算表與
* 匯入自訂物件
* 匯入清單
* 合併人員
* 執行單一流程動作 — 讓使用者能夠執行 **變更資料值** 對資料庫中的人員執行流程步驟

* 檢視機會資料 — 隱藏個人詳細資訊頁面上的機會資訊

## 存取行銷活動 {#access-marketing-activities}

檢視行銷活動標籤、行銷活動和行銷活動資料夾。

* 存取簡訊訊息

   * 核准簡訊訊息
   * 刪除簡訊訊息
   * 編輯SMS訊息

* 存取推播通知

   * 核准推播通知
   * 刪除推播通知
   * 編輯推播通知

* 存取獎勵
* 啟動觸發程式行銷活動
* 核准電子郵件方案
* 原地複製行銷資產
* 刪除行銷資產
* 編輯行銷活動限制
* 編輯行銷資產
* 匯入計畫
* 清單匯入
* 排程批次行銷活動

存取SEO

* 管理SEO
* 標準SEO

## 目標定位和個人化 {#targeting-and-personalization}

* 管理Web個人化
* CRE行銷活動編輯器
* CRE Campaign啟動器
* 網站行銷活動編輯器
* 網頁行銷活動啟動器

工作區管理

* 特定工作區的管理員存取權（前提是您已啟用工作區）
* 在工作區之間移動資產（前提是您已啟用工作區）
