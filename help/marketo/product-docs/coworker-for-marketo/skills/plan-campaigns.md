---
description: 使用適用於Marketo Engage的CX Enterprise Coworker ，將行銷活動簡報轉換為涵蓋對象邏輯、電子郵件、權杖和QA檢查的結構化方案計畫。
title: 計畫行銷活動
source-git-commit: e72db83a5f1f3c58a29da7c4b4b1bbb79a61b596
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%
---
# 計畫行銷活動 {#plan-campaigns}

將行銷活動簡報轉換為Marketo Engage的結構化實作計畫。 計畫行銷活動技能概述方案結構、對象邏輯、電子郵件、智慧行銷活動、代號、報告和預先啟用檢查。 輸出為出現在工作區面板中的可下載報表。

>[!NOTE]
>
>- 此技能會產生Marketo Engage計畫的實施計畫（結構化檔案，告訴人員或自動化系統確切如何建立行銷活動）。 它不會在Marketo Engage中建立任何內容。 [建置計畫](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md){target="_blank"}有單獨的技能。
>- 此技能以[組織規則](/help/marketo/product-docs/coworker-for-marketo/organizational-rules.md){target="_blank"}為指引。

## 先決條件 {#prerequisites}

- 若為方案計畫，請提供可用的資訊給行銷活動簡報，例如行銷活動目標、目標對象、訊息、時間表和成功量度。
- 若要改善現有的簡介或計畫，請提供檔案並描述您想要的變更。
- 若要在不做簡訊的情況下開始使用，請要求範例簡訊或根據常見行銷活動情境請求計畫。

## 使用方式 {#how-to-use}

1. 在「我的Marketo」中，按一下「**[!UICONTROL CX Enterprise Coworker for Marketo Engage]**」圖磚。

1. 選取&#x200B;**[!UICONTROL Plan campaigns]**&#x200B;技能並按一下&#x200B;**[!UICONTROL Use this skill]**。

1. 選擇您要執行的動作：
   - 從行銷活動簡介規劃方案。
   - 產生範例行銷活動簡報。
   - 改善現有摘要。
   - 修訂現有的設定計畫。

1. 提供簡報或檔案。 包含任何特定變更、行銷活動要求或組織慣例。

1. 在Workspace面板中檢閱產生的報告。 開啟它以檢閱詳細資料或下載報告。

1. 在Marketo Engage中建立方案之前，請先檢閱並核准設定計畫。

## 技能選項 {#skill-options}

### 計畫方案 {#plan-a-program}

方案計畫會將行銷活動需求轉換為建立方案的指示。 根據摘要，其中可能包括：

- **方案總覽：**&#x200B;行銷活動名稱、目標、目標對象和時間表。
- **資料夾結構：**&#x200B;電子郵件、智慧行銷活動和報表的建議本機資料夾。
- **智慧列示：**&#x200B;分段邏輯、篩選器定義和必要的排除。
- **電子郵件設定：**&#x200B;主旨列、前置文字、內容結構、寄件者詳細資訊和規範元素。
- **智慧行銷活動：**&#x200B;行銷活動名稱、觸發或批次指定、流程步驟和排程建議。
- **權杖和欄位：**&#x200B;我的權杖、必要和自訂權杖，以及任何需要的自訂欄位及其型別和值。
- **歷程流程：**&#x200B;行銷活動順序、等待步驟和決定邏輯。
- **報告與QA：**&#x200B;成功量度、建議的報表，以及預先啟用驗證檢查。

### 建立範例簡報 {#create-a-sample-brief}

當您想要調整範例時，請要求範例簡報。 您可以指定主題或促銷活動型別，例如產品上市或網路研討會。 如果您要求計畫但不提供簡報，則技能可以使用範例情境（例如產品上市網路研討會）作為計畫的基礎。

### 修剪摘要或修訂計畫 {#polish-a-brief-or-revise-a-plan}

此技能會從檔案內容中識別檔案型別，而非僅依賴您請求的措辭。

**行銷活動簡報**&#x200B;通常會說明目標、對象、傳訊策略、時間表和成功量度。 **安裝計畫**&#x200B;通常包含實作詳細資料，例如智慧列示組態、智慧行銷活動流程步驟、權杖定義、電子郵件規格和技術需求。

提供檔案和您要求的變更。 例如，如果您要求改善計畫但提供行銷活動簡報，此技能會將檔案視為簡報。 如果您提供設定計畫並要求修訂簡報，則會將檔案視為計畫。

## 組織規則整合 {#organizational-rules-integration}

設定檔案應從系統前後關聯中合併您組織的規則。

### 命名慣例 {#naming-conventions}

- 程式： `{{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}`
- 電子郵件： `{{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}`
- 智慧行銷活動： `{{NUMBER}}_{{TRIGGER_OR_BATCH}}_{{ACTION}}`

### 必要元素 {#required-elements}

- 三個本機資料夾（01封電子郵件、02個智慧行銷活動、03個報告）
- 四個必要權杖(eventDate、eventTime、replyToEmail、senderName)
- 排除篩選器（已取消訂閱、電子郵件無效、行銷活動已暫停、已列入封鎖名單）
- 電子郵件規範遵循（取消訂閱連結、實體地址）

### 啟動前QA {#pre-activation-qa}

- 名稱模式驗證
- 檔案夾結構確認
- 排除篩選器驗證
- 合規性元素檢查

## 使用案例 {#use-cases}

**規劃網路研討會計畫：**&#x200B;提供網路研討會目標、對象、活動時間表及傳訊需求。 設定計畫可概述方案結構、電子郵件規格、行銷活動順序、代號及QA檢查。

**產生範例簡報：**&#x200B;要求行銷活動型別的範例簡報，然後將其與行銷活動詳細資料一起調整，再要求方案計畫。

**更新現有的設定計畫：**&#x200B;提供計畫並指定變更，例如更新時間表、新增行銷活動步驟或修訂對象邏輯。

## 後續步驟 {#next-steps}

計畫作業完成後，適當的後續提示可能包括：

- 「修訂此設定計畫」
- 「取得範例行銷活動簡報」
- 「在Marketo中建立此程式」（若要建立程式，您必須使用[建立程式](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md)技能）。
