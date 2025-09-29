---
solution: Marketo Engage
product: marketo
title: 使用 AI 助理
description: 善用 Adobe 的生成式 AI 技術為您的電子郵件新增實用的文字和/或影像。
level: Beginner, Intermediate
feature: Email Designer
exl-id: e07ed645-d8a3-483f-aa1f-f82bc9cb8634
source-git-commit: 38a35f2c6b2abfca6c200fa6d8e53452dcfaeff6
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 9%

---

# 使用 AI 助理 {#use-ai-assistant}

Marketo Engage Email Designer中的AI Assistant可幫助您建立當代、高效能且直覺式的電子郵件。 透過 Adobe 的生成式 AI 技術和提示資料庫，並搭配 Firefly 來產生影像，協助針對特定的人物誌/購買群組、行銷歷程階段、溝通策略、語調等建立適當的內容，便能打造出這樣的電子郵件。也可以使用特定品牌資產來建立內容。

>[!PREREQUISITES]
>
>AI助理預設為未啟用。 您必須先同意[核心Gen-AI條款與補充條款](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}，才能在電子郵件Designer中使用Gen-AI功能。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

## 設定許可權 {#set-up-permissions}

_依照上述必要條件，_&#x200B;之後，Marketo管理員必須先套用存取權給特定使用者/角色，使用者才能看到GenAI按鈕。

1. 在Marketo Engage中，按一下&#x200B;**管理員**&#x200B;並選取&#x200B;**使用者和角色**。

   ![](assets/use-the-ai-assistant-0a.png)

1. 在&#x200B;**角色**&#x200B;標籤中，按兩下所需的角色。

   ![](assets/use-the-ai-assistant-0b.png)

1. 在&#x200B;_Access Design Studio_&#x200B;下，選取&#x200B;**Access AI小幫手**&#x200B;核取方塊，然後按一下&#x200B;**儲存**。

   ![](assets/use-the-ai-assistant-0c.png)

1. 按一下使用者索引標籤，然後選取您要提供存取權的使用者。

   ![](assets/use-the-ai-assistant-0d.png)

1. 選取您在步驟3中選擇的角色以及所需的工作區（如果適用）。 按一下&#x200B;**儲存**。

   ![](assets/use-the-ai-assistant-0e.png)

## 使用案例 {#use-cases}

AI Assistant有三個主要使用案例：

* [為您的電子郵件建立主旨列](#create-a-subject-line)
* [為電子郵件的特定區段](#create-content-for-a-specific-section)建立內容
* [從選取的範本建立整封電子郵件](#create-an-entire-email)

## 建立主旨列 {#create-a-subject-line}

使用新電子郵件Designer建立電子郵件時，輸入暫時性主旨列。

![](assets/use-the-ai-assistant-1.png)

建立電子郵件之後，主旨列在右側的&#x200B;_詳細資料_&#x200B;欄中。 按一下旁邊的AI助理按鈕（ ![篩選圖示](assets/icon-ai-assistant.png) ）以取得協助，使用Gen AI功能建立新的主旨列。

![](assets/use-the-ai-assistant-2.png)

啟用AI助理的&#x200B;**使用參考內容**&#x200B;選項，以根據選取的內容個人化新內容。

輸入提示來自訂主旨列。 輸入相關文字設定，然後上傳您要用來作為參照的任何品牌資產，以建立適當的主旨行。

![](assets/use-the-ai-assistant-3.png)

文字設定包括：

<table><tbody>
  <tr>
    <td style="width:25%"><b>購買群組</b></td>
    <td>您鎖定目標的特定購買群組（例如，從業人員、影響者、決策者）。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>行銷歷程階段</b></td>
    <td>特定行銷歷程階段的收件者（例如，探索、評估、認可）。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>溝通策略</b></td>
    <td>通訊的目標（例如，緊急、社交證明、資訊）。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>語言</b></td>
    <td>您要產生主旨行的語言。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>色調</b></td>
    <td>您希望產生內容的語調（例如，勵志、興奮、幽默）。</td>
  </tr>
  <tr>
    <td style="width:25%"><b>表情符號</b></td>
    <td>允許在產生的內容中包含表情符號。</td>
  </tr>
</tbody>
</table>

按一下&#x200B;**產生**&#x200B;後，會出現範例供您選擇：

![](assets/use-the-ai-assistant-4.png)

您也可以上傳品牌資產，以使用資產內的內容作為建立主旨行的參考。

![](assets/use-the-ai-assistant-5.png)

若要選擇變數，請選取其核取方塊，然後按一下&#x200B;**選取**。 您也可以按一下「調整&#x200B;**&#x200B;**」來調整它。 此外，您可以按一下向上或向下縮圖示提供意見回饋，讓Gen-AI技術學習您的偏好設定。

做出選擇後，主旨列會填入您的電子郵件詳細資訊中。

![](assets/use-the-ai-assistant-6.png)

## 為您的電子郵件特定區段建立內容 {#create-content-for-a-specific-section}

建立電子郵件後，您可以選擇修改某些區段、影像或文字。

![](assets/use-the-ai-assistant-7.png)

在此範例中，我們使用醫療保健範本。 如果現有的醫療保健專家影像不符合您的需求，您可以指示AI助理建立自己的醫療保健專家影像。 只需選取影像內容，然後按一下AI助理。

![](assets/use-the-ai-assistant-8.png)

在提示中輸入相關詳細資訊，例如「產生醫療保健專家的影像」，並新增任何需要的自訂。 如果您不確定要輸入什麼，也可以使用提示程式庫（在提示的右側）。

按一下&#x200B;**產生**&#x200B;之後，會建立多個變體供您選擇。

![](assets/use-the-ai-assistant-9.png)

與影像類似，也可以修改電子郵件的文字部分。

![](assets/use-the-ai-assistant-10.png)

## 從選取的範本建立整個電子郵件 {#create-an-entire-email}

僅當使用現有範本建立電子郵件時，才可使用此選項。 可以是電子郵件Designer提供的標準範本、您已建立的已儲存範本，或使用「匯入HTML」選項匯入的範本。 如果您為電子郵件選擇[從草稿開始設計](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#design-from-scratch)，則無法使用此選項。

選取範本，不選取範本中的任何元件，然後按一下「電子郵件Designer」中的AI助理按鈕。

![](assets/use-the-ai-assistant-11.png)

輸入相關提示，然後選擇文字設定、品牌資產，以及您想要用於電子郵件的任何影像設定。

![](assets/use-the-ai-assistant-12.png)

如果您想要使用Firefly產生影像，請選取「影像設定」並選取&#x200B;**使用AI產生影像**&#x200B;的切換按鈕。

![](assets/use-the-ai-assistant-13.png)

選取所需的&#x200B;_內容型別_、_色彩和色調_、_光源_&#x200B;和&#x200B;_構成_，為您的電子郵件建立Gen-AI影像。 完成時，按一下&#x200B;**產生**。

![](assets/use-the-ai-assistant-14.png)

按一下&#x200B;**預覽**，檢視變數在電子郵件中的外觀。 按一下&#x200B;**套用**&#x200B;以選擇變數。
