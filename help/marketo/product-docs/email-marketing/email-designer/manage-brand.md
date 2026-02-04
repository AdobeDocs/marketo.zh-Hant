---
solution: Marketo Engage
product: Marketo
title: 管理品牌
description: 瞭解如何建立和管理您的品牌指引
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 8%

---

# 建立和管理您的品牌 {#brands}

品牌指引是一組詳細的規則和標準，可建立品牌的視覺和口頭識別。 這些可作為參考，以在所有行銷和通訊平台上維持一致的品牌代表性。

手動輸入及組織您的品牌詳細資料，或上傳品牌指引檔案，以便自動擷取資訊。

>[!AVAILABILITY]
>
>您必須同意[使用者合約](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}，才能在Adobe Marketo Engage中使用AI小幫手。 如需詳細資訊，請聯絡您的 Adobe 代表。

## 存取品牌 {#generative-access}

若要在&#x200B;**[!UICONTROL Brands]**&#x200B;中存取[!DNL Adobe Marketo Engage]功能表，使用者必須被授與&#x200B;**[!UICONTROL Manage brand kit]**&#x200B;或&#x200B;**[!UICONTROL Enable AI assistant]**&#x200B;許可權。

+++  瞭解如何指派品牌相關許可權

若要指派品牌的許可權，請遵循下列步驟：

1. 在&#x200B;**權限**&#x200B;產品中，前往&#x200B;**角色**&#x200B;標籤，然後選取所需的&#x200B;**角色**。

1. 按一下&#x200B;**編輯**&#x200B;以修改權限。

1. 新增&#x200B;**AI小幫手**&#x200B;資源，然後從下拉式功能表中選取&#x200B;**管理品牌套件**&#x200B;或&#x200B;**[!UICONTROL Enable Ai assistant]**。

   請注意，**[!UICONTROL Enable Ai assistant]**&#x200B;許可權僅提供&#x200B;**[!UICONTROL Brands]**&#x200B;功能表的唯讀存取權。

   熒幕擷圖

1. 按一下&#x200B;**儲存**，以套用所做的變更。

   任何已指派給此角色的使用者都會自動更新其權限。

1. 若要將此角色指派給新使用者，請瀏覽至&#x200B;**角色**&#x200B;儀表板中的&#x200B;**使用者**&#x200B;標籤，然後按一下&#x200B;**新增使用者**。

1. 輸入使用者的名稱、電子郵件地址，或從清單當中選擇，然後按一下&#x200B;**儲存**。

1. 如果之前未建立使用者，請參閱[此文件](https://experienceleague.adobe.com/zh-hant/docs/experience-platform/access-control/abac/permissions-ui/users)。

+++

## 建立和管理您的品牌 {#create-brand-kit}

若要建立和管理您的品牌指引，您可以自行輸入詳細資料，或上傳品牌指引檔案以自動擷取資訊：

1. 在&#x200B;**[!UICONTROL Brands]**&#x200B;功能表中，按一下&#x200B;**[!UICONTROL Create brand]**。

   熒幕擷圖

1. 為您的品牌輸入&#x200B;**[!UICONTROL Name]**。

1. 拖放或選取您的檔案，以上傳您的品牌指引，並自動擷取相關的品牌資訊。 按一下「**[!UICONTROL Create brand]**」。

   資訊擷取程式現在開始。 請注意，可能需要幾分鐘才能完成。

   熒幕擷圖

1. 系統現在會自動填入您的內容和視覺化建立標準。 瀏覽不同的標籤，視需要調整資訊。 [了解更多](#personalize)

1. 從每個區段或類別的進階功能表中，您可以新增參照以自動擷取相關品牌資訊。

   若要移除現有內容，請使用&#x200B;**[!UICONTROL Clear section]**&#x200B;或&#x200B;**[!UICONTROL Clear category]**&#x200B;選項。

   熒幕擷圖

1. 設定之後，按一下&#x200B;**[!UICONTROL Save]**，然後按&#x200B;**[!UICONTROL Publish]**，讓您的品牌指引可在AI助理中取得。

1. 若要修改您發佈的品牌，請按一下&#x200B;**[!UICONTROL Edit brand]**。

   >[!NOTE]
   >
   >這會在編輯模式中建立臨時副本，並在發佈後取代即時版本。

   熒幕擷圖

1. 在&#x200B;**[!UICONTROL Brands]**&#x200B;儀表板中，按一下三個點的圖示來開啟進階功能表：

   * 檢視品牌
   * 編輯
   * 重複
   * 發佈
   * 取消發佈
   * 刪除

   熒幕擷圖

您現在可以從AI Assistant功能表的&#x200B;**[!UICONTROL Brand]**&#x200B;下拉式清單存取品牌指南，使其產生符合您規格的內容和資產。

熒幕擷圖

### 設定預設品牌 {#default-brand}

您可以指定預設品牌，在建立行銷活動期間產生內容及計算一致性分數時自動套用。

若要設定預設品牌，請移至您的&#x200B;**[!UICONTROL Brands]**&#x200B;儀表板。 按一下三點圖示並選取&#x200B;**[!UICONTROL Mark as default brand]**，開啟進階功能表。

熒幕擷圖

## 個人化您的品牌 {#personalize}

### 關於品牌 {#about-brand}

使用&#x200B;**[!UICONTROL About the brand]**&#x200B;標籤來建立品牌的核心身分 — 概述其用途、個性、標語和其他定義屬性。

1. 首先，在&#x200B;**[!UICONTROL Key details]**&#x200B;類別中填寫品牌的基本資訊：

   * **[!UICONTROL Brand Kit Name]**：輸入您的品牌套件名稱。

   * **[!UICONTROL When to Use]**：指定應套用此品牌套件的案例或內容。

   * **[!UICONTROL Brand Name]**：輸入品牌的正式名稱。

   * **[!UICONTROL Brand Description]**：提供此品牌代表的概觀。

   * **[!UICONTROL Default Tagline]**：新增與品牌關聯的主要標語。

   熒幕擷圖

1. 在&#x200B;**[!UICONTROL Guiding principles]**&#x200B;類別中，釐清品牌的核心方向和理念：

   * **[!UICONTROL Mission]**：詳細說明您品牌的用途。

   * **[!UICONTROL Vision]**：說明您的長期目標或想要的未來狀態。

   * **[!UICONTROL Market Positioning]**：說明您的品牌在市場上的定位。

   熒幕擷圖

1. 從&#x200B;**[!UICONTROL Core brand values]**&#x200B;類別中，按一下「新增圖示」以新增品牌的核心值並填寫詳細資料：

   * **[!UICONTROL Value]**：為核心品牌值命名。

   * **[!UICONTROL Description]**：說明這個值對您的品牌有何意義。

   * **[!UICONTROL Behaviors]**：概述實際中反映此值的動作或態度。

   * **[!UICONTROL Manifestations]**：提供這個值在真實世界品牌中如何表示的範例。

   熒幕擷圖

1. 如有需要，請按一下「編輯」圖示以更新或刪除您的其中一個核心品牌價值。

   熒幕擷圖

您現在可以進一步個人化您的品牌，或[發佈您的品牌](#create-brand-kit)。

### 寫作風格 {#writing-style}

**[!UICONTROL Writing style]**&#x200B;區段概述撰寫內容的標準，詳述應如何使用語言、格式和結構來保持所有材料的清晰度、一致性和一致性。

+++ 可用的類別和範例

<table>
  <thead>
    <tr>
      <th>類別</th>
      <th>子類別</th>
      <th>指引範例</th>
      <th>排除專案範例</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">內容建立標準</td>
      <td>品牌訊息標準</td>
      <td>強調創新和客戶至上的訊息。</td>
      <td>請勿過度承諾產品功能。</td>
    </tr>
    <tr>
      <td>標語使用方式</td>
      <td>在所有數位行銷資產的標誌下方放置標語。</td>
      <td>請勿修改或翻譯標語。</td>
    </tr>
    <tr>
      <td>核心訊息</td>
      <td>強調主要優勢陳述，例如提高生產力。</td>
      <td>請勿使用不相關的值主張。</td>
    </tr>
    <tr>
      <td>命名標準</td>
      <td>使用簡單的描述性名稱，例如「ProScheduler」。</td>
      <td>請勿使用複雜字元或特殊字元。</td>
    </tr>
    <tr>
      <td rowspan="5">品牌溝通風格</td>
      <td>品牌人格特徵</td>
      <td>親切易懂。</td>
      <td>不要失敗。</td>
    </tr>
    <tr>
      <td>書寫力學</td>
      <td>讓句子儘量簡短並有影響力。</td>
      <td>不要使用過多的行話。</td>
    </tr>
    <tr>
      <td>情境色調</td>
      <td>維持危機溝通的專業語調。</td>
      <td>支援通訊時請勿不屑一顧。</td>
    </tr>
    <tr>
      <td>Word選擇指南</td>
      <td>使用「創新」和「智慧」等字眼。</td>
      <td>避免使用「便宜」或「駭客」等字眼。</td>
    </tr>
    <tr>
      <td>語言標準</td>
      <td>遵循美式英文慣例。</td>
      <td>請勿混合使用英式及美式拼字。</td>
    </tr>
    <tr>
      <td rowspan="3">法規遵循標準</td>
      <td>商標標準</td>
      <td>請一律使用™或®符號。</td>
      <td>必要時，請勿省略法定符號。</td>
    </tr>
    <tr>
      <td>版權標準</td>
      <td>在行銷資料中加入版權注意事項。</td>
      <td>未經許可請勿使用協力廠商內容。</td>
    </tr>
    <tr>
      <td>免責宣告標準</td>
      <td>在數位資產上清楚顯示免責宣告。</td>
      <td>請勿隱藏隱藏隱藏隱藏隱藏區域的免責宣告。</td>
    </tr>
</table>

+++

</br>

個人化您的&#x200B;**[!UICONTROL Writing Style]**：

1. 在&#x200B;**[!UICONTROL Writing Style]**&#x200B;標籤中，按一下&#x200B;**+**&#x200B;圖示以新增指引、例外或排除。

1. 輸入您的指引、例外或排除。 您也可以加入&#x200B;**[!UICONTROL Examples]**，以更清楚說明應如何套用它。

   熒幕擷圖

1. 指定您指引、例外或排除的「使用」內容：

   * **[!UICONTROL Channel type]**：選擇此指引、例外或排除的適用位置。 例如，您可能希望特定的書寫樣式僅顯示在電子郵件、行動裝置、列印或其他通訊通道中。

   * **[!UICONTROL Element type]**：指定套用規則的內容元素。 這可能包括標題、按鈕、連結或內容中的其他元件等元素。

   熒幕擷圖

1. 一旦您的指引、例外或排除設定完成後，請按一下&#x200B;**[!UICONTROL Add]**。

1. 如有需要，請選取其中一個准則或排除專案來更新或刪除。

1. 按一下「編輯」以編輯您的範例，或按一下「刪除」圖示以刪除範例。

   熒幕擷圖

您現在可以進一步個人化您的品牌，或[發佈您的品牌](#create-brand-kit)。

### 視覺內容 {#visual-content}

**[!UICONTROL Visual Content]**&#x200B;區段定義影像和設計的標準，詳細說明維持統一一致的品牌外觀所需的規格。

+++ 可用的類別和範例

<table>
  <thead>
    <tr>
      <th>類別</th>
      <th>指引範例</th>
      <th>排除專案範例</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>攝影標準</td>
      <td>戶外鏡頭使用自然光線。</td>
      <td>避免過度編輯或畫素化的影像。</td>
    </tr>
    <tr>
      <td>插圖示準</td>
      <td>使用簡潔的極簡風格。</td>
      <td>避免過於複雜。</td>
    </tr>
    <tr>
      <td>圖示標準</td>
      <td>使用一致的24px格線系統。</td>
      <td>請勿混合圖示尺寸、使用不一致的線條粗細，或偏離格線規則。</td>
    </tr>
    <tr>
      <td>使用指南</td>
      <td>選擇反映真實客戶在專業環境中使用該產品的生活方式影像。</td>
      <td>請勿使用與品牌色調相抵觸或看起來與內容不符的影像。</td>
    </tr>
</table>

+++

</br>

個人化您的&#x200B;**[!UICONTROL Visual content]**：

1. 從&#x200B;**[!UICONTROL Visual content]**&#x200B;索引標籤中，按一下三個點的圖示以新增指引、排除專案或範例。

1. 輸入您的指引、排除專案或範例。

   熒幕擷圖

1. 指定指引或排除專案的使用內容：

   * **[!UICONTROL Channel type]**：選擇此指引、例外或排除的適用位置。 例如，您可能希望特定的書寫樣式僅顯示在電子郵件、行動裝置、列印或其他通訊通道中。

   * **[!UICONTROL Element type]**：指定套用規則的內容元素。 這可能包括標題、按鈕、連結或內容中的其他元件等元素。

   熒幕擷圖

1. 一旦您的指引、例外或排除設定完成後，請按一下&#x200B;**[!UICONTROL Add]**。

1. 若要新增顯示正確使用方式的影像，請選取&#x200B;**[!UICONTROL Example]**&#x200B;並按一下&#x200B;**[!UICONTROL Select image]**。 您也可以新增使用方式不正確的影像，作為排除範例。

   熒幕擷圖

1. 如有需要，請選取其中一個准則或排除專案來更新或刪除。

1. 選取您的指引或排除專案以更新它。 按一下「刪除」圖示以將其刪除。

   熒幕擷圖

您現在可以進一步個人化您的品牌，或[發佈您的品牌](#create-brand-kit)。
