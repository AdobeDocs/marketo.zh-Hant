---
description: 瞭解組織規則如何定義治理標準，並在方案建立、行銷活動規劃和驗證期間為Marketo Engage的同事提供指導。
title: 組織規則
source-git-commit: c1581e2b692dd50bf472756e4e6222ff75ae091c
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%
---
# 組織規則 {#organizational-rules}

組織規則會以單一檔案定義您的行銷作業標準和治理要求，引導Marketo Engage的同事完成方案建立、行銷活動規劃和驗證工作流程。

## 什麼是組織規則？ {#what-are-organizational-rules}

組織規則是以Markdown為基礎的設定檔案，可擷取您組織的行銷活動標準：

* 方案、電子郵件和智慧行銷活動的命名慣例
* 必要的資產和結構（資料夾、權杖、報表）
* 合規性要求（取消訂閱連結、UTM引數、排除篩選器）
* 最佳實務（電子郵件設計、智慧清單設定）

每個Marketo Engage環境都包含預設的組織規則。 您可以自訂這些規則，以反映組織的特定治理需求。

## 使用組織規則的位置 {#where-organizational-rules-are-used}

組織規則指南Marketo Engage同事的三項技能：

| 技能 | 規則的套用方式 |
| --- | --- |
| 建置計畫 | 規則可指導程式結構的建立、命名和初始設定。 Marketo Engage的同事會在建立方案之前，在您的簡報中標示任何法規遵循問題。 |
| 計畫行銷活動 | 規則會通知Marketo Engage的同事如何根據您的標準來建構智慧行銷活動、篩選器和流程步驟。 |
| 驗證程式 | 規則會定義在啟動前驗證程式時，Marketo Engage的同事要檢查哪些專案。 |

## 如何存取及自訂組織規則 {#how-to-access-and-customize-organizational-rules}

1. 在「我的Marketo」中，按一下「**Marketo Engage同事**」圖磚。
1. 按一下齒輪圖示。
1. 選取&#x200B;**組織規則**&#x200B;標籤。
1. 檢閱預設規則（這些規則已預先填入行銷操作最佳實務）。
1. 編輯規則以符合您組織的規則：

   * 命名慣例（方案、電子郵件、行銷活動）
   * 必要的檔案夾結構
   * 必要權杖和欄位
   * 法規遵循與排除標準

1. 進行變更時請更新版本號碼。
1. 儲存您的變更。 所有Marketo Engage技能的同事將立即使用您的自訂規則。

## 組織規則結構 {#organizational-rules-structure}

組織規則的格式為使用YAML frontmatter的Markdown：

```markdown
---
name: Your Organization Name - Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## Required Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## 組織規則的最佳實務 {#best-practices-for-organizational-rules}

* **以預設值開始**：在自訂之前先檢閱預設規則。 這些規則反映了行銷操作的業界最佳實務。
* **讓規則重點突出**：僅包含對貴組織重要的需求。 不必要的規則會產生雜訊，且會不必要地降低相容分數。
* **同時使用自動和手動檢查**：

  * 自動檢查：命名慣例、必要資料夾、權杖使用方式（Marketo Engage的同事可以確認）
  * 手動檢查：電子郵件視覺化設計、品牌法規遵循、行銷活動邏輯（Marketo Engage的同事會將這些標幟為手動檢閱步驟）

* **平衡嚴格性與彈性**：過於嚴格的規則可能會減慢程式建立的速度。 規則太鬆散，無法攔截重要的規範遵循問題。
* **將規則版本化**：進行重大變更時請更新版本號碼，讓您的團隊知道已更新治理標準。
* **溝通變更**：更新組織規則時，請讓您的行銷營運團隊知道變更內容及原因。

## 什麼是Marketo Engage的同事可以驗證和無法驗證 {#what-coworker-can-and-cannot-validate}

Marketo Engage CAN的同事驗證（自動檢查）：

* 命名慣例符合您的模式
* 必要的檔案夾結構已存在
* 已具備必要的權杖
* 電子郵件有取消訂閱連結和必要的頁尾元素
* 外部連結包含UTM引數
* 智慧型行銷活動名稱遵循慣例

Marketo Engage的同事無法驗證（需要手動檢閱）：

* 智慧清單篩選器邏輯（API限制：您必須手動設定篩選器）
* Smart Campaign流程步驟邏輯（API限制：您必須手動設定流程）
* 電子郵件視覺化呈現和回應能力（需要視覺化檢查）
* 品牌法規遵循與傳訊基調（需要人為判斷）
* 動態內容分段規則（API限制）

當Marketo Engage的同事遇到無法驗證的問題時，會在工作流程中將其標示為手動檢閱步驟。

## 合規性評分 {#compliance-scoring}

當您使用「驗證程式」時，適用於Marketo Engage的Co-worker會根據下列專案計算相容分數：

* **通過檢查**： Marketo Engage的同事已驗證合規性，未發現任何問題
* **失敗的檢查**： Marketo Engage的同事發現違反您的組織規則
* **手動檢閱步驟**：需要人為驗證的專案（這些不會計入您的分數）

一個計畫可以有100%的相容性，但仍需要手動複查步驟；這些步驟會排除在分數計算之外。

## 組織規則自訂範例 {#examples-of-organizational-rules-customization}

**範例1：嚴格的命名慣例**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

如果您的組織需要跨地區和業務部門的嚴格控管，請使用此選項。

**範例2：具有必要首碼的彈性命名**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

如果您想要地區代碼的一致性，但其他部分要有彈性，請使用此選項。

**範例3：最小規則（著重於規範）**

```markdown
# Email Compliance - REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

如果貴組織將法規遵循優先順序置於命名/結構一致性之上，請使用此選項。

## 疑難排解 {#troubleshooting}

**問：我已更新組織規則，但Marketo Engage的同事仍在使用舊規則。**

答：新程式和驗證的變更會立即生效。 如果您正在使用現有的程式，請重新整理瀏覽器或為Marketo Engage工作流程開始新的同事，以檢視更新的規則。

**問：我可以還原為預設規則嗎？**

答：是。 移至&#x200B;**設定** > **組織規則**，然後按一下&#x200B;**重設為預設值**。 您的自訂規則將會取代為預設規則。

**問：我的相容性分數很低，即使程式看起來不錯。**

答：檢查哪些檢查失敗。 請檢閱您的組織規則，以瞭解這些規則對您目前的工作流程是否過於嚴格，或者您是否需要調整方案以符合您的標準。
