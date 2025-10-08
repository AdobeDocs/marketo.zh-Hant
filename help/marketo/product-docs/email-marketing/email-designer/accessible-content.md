---
title: 設計無障礙內容
description: 瞭解如何在Marketo Engage中為您的電子郵件設計無障礙內容。
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: 電子郵件、設計、協助工具
source-git-commit: 753455b40ead039a56c595fa61ab9a95b7936382
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 0%

---

# 設計無障礙內容 {#accessible-content}

[歐洲無障礙法](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882){target="_blank"}是一項指令，旨在透過消除因各成員國的不同國家規則所造成的障礙，來增強無障礙產品和服務的內部市場。

這項法規規定，所有數位通訊，包括電子郵件、電子報、PDF和可下載的內容，都應可供存取。 因此，在為收件者建立內容時，您必須遵循特定准則，例如使用無障礙字型和可讀格式，以及為影像提供替代文字。

Marketo Engage電子郵件Designer可讓您根據網頁內容可及性指引(WCAG) 2.1 （AA級），輕鬆遵循此指示。 以下列出使用Marketo Engage設計無障礙內容的最佳實務。

>[!NOTE]
>
>此頁面主要說明如何讓所有收件者都能存取您的內容，讓身心障礙人士能夠閱讀、瞭解您在Marketo Engage中設計的電子郵件，並與之互動。

## 確保文字可讀性 {#text-readability}

運用&#x200B;**[!UICONTROL Styles]**&#x200B;元件的&#x200B;**[!UICONTROL Text]**&#x200B;標籤，確保文字可讀，例如使用適當的色彩對比和簡單字型。

<!--![](assets/accessible-text-styles.png){width="80%"}-->

針對字型和文字，請務必遵循下列准則：

**字型選擇**

* 使用Arial、Verdana、Tahoma、Helvetica或Open Sans等無襯線字型。
* 避免在正文內容中使用襯線、草稿或裝飾字型。
* 保留至有限的字型集以取得一致性和遞補（例如： `font-family: Arial, Helvetica, sans-serif;`）。

**字型大小**

* 確定內文字型大小下限為16px。
* 請使用適當的標題階層。

**色彩對比**

* 維持文字與背景之間的對比率至少為4.5:1。
* 對於大型文字(≥24px或粗體18px)，請確定至少3:1對比度。
* 避免白色背景上的淺灰色或淡色文字。
* 不要只依賴顏色來傳達意義。 使用底線、圖示等

**文字協助工具**

* 避免影像中的文字。
* 請勿在正文中使用全部大寫字。
* 確保文字可以縮放至200%而不中斷版面。

## 確保視覺化協助工具 {#visual-accessibility}

* 避免使用僅限顏色的指標來取得重要資訊。
* 請使用文字標籤或圖示來清楚說明。
* 針對行動裝置和回應式版面配置最佳化您的設計，確保按鈕較大且間距適當。
* 定期測試裝置和熒幕大小，以維持協助工具。

在Marketo Engage中，您可以使用「電子郵件Designer **[!UICONTROL Styles]**」窗格的樣式引數和屬性，進一步調整內容中不同元素的大小和間距。

例如，您可以更新背景或變更邊界、邊框間距和對齊方式，以改善視覺協助工具。

<!--![](assets/accessible-styles.png){width="80%"}-->

Marketo Engage電子郵件Designer可讓您預覽並最佳化不同裝置和熒幕大小的設計。 您隨時可以&#x200B;**[!UICONTROL Switch to live view]**&#x200B;檢查您的內容在各種裝置大小上可能呈現的方式。

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>即時檢視是通用的預覽，用來比較內容在各種裝置大小中可能呈現的方式。 最終呈現內容可能會因收件者的電子郵件使用者端而異。

## 使用影像的替代文字 {#alt-text}

使用&#x200B;**[!UICONTROL Image]**&#x200B;元件提供影像的替代文字。

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* 簡潔且情境化地描述影像用途。
* 請避免「影像……」等多餘的片語，並使用裝飾性影像的空白替代文字。
* 對於具有意義的圖示，提供有意義的標籤；對於複雜的影像，請使用簡短替代文字，並在其他位置使用較長的說明。

## 使用可讀格式 {#readable-format}

使用電子郵件Designer的相關結構和內容元件，以及&#x200B;**[!UICONTROL Styles]**&#x200B;窗格中的選項，以清晰、邏輯且簡潔的方式組織您的內容，讓所有人都能存取。

<!--![](assets/accessible-components.png){width="100%"}-->

* 使用結構化、語意化的HTML，搭配適當的標題、段落、清單和表格。
* 確保內容遵循由左至右、由上至下的邏輯流程。
* 使用簡潔明瞭的語言。
* 為PDF和Infographics提供替代格式。
* 允許調整文字大小及重排，並確保印刷樣式在所有格式中都能以足夠的色彩對比讀取。

## 確保內容可讀性 {#readability}

若要閱讀，您的內容必須清晰、結構良好，且可供所有人使用，包括視覺、認知或閱讀困難的人士以及使用輔助技術的人。 建立無障礙內容時，請考量以下幾點：

* 將句子限制在20字以內。
* 編輯您的復本，使其簡明扼要。
* 使用主動語態讓句子結構更簡單。
* 避免使用某些人可能不熟悉的俚語、行話或地區性用語。

若要評估您的電子郵件可讀性，您可以使用熱門的[Flesch Reading Easy測試](https://support.microsoft.com/en-us/office/get-your-document-s-readability-and-level-statistics-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"}，此測試可在Microsoft Word中找到，並以0至100的級數計算內容的閱讀容易程度。

## 測試您的內容 {#test}

若要驗證內容的協助工具，您可以使用Marketo Engage提供的測試功能。 它們不是特別設計來檢查您的內容是否完全可存取，但是它們可以提供第一級的驗證。

* 使用測試設定檔預覽您的內容。

* 使用[電子郵件呈現](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"}選項，利用Litmus模擬您跨主要電子郵件使用者端(Apple Mail、Gmail、Outlook)的設計，並檢視文字、色彩和影像是否可讓您存取內容。<!--Litmus includes accessibility testing-->

* 傳送校樣以測試內容的轉譯，然後再傳送給真正的對象。

<!--![](assets/accessible-simulate.png){width="90%"}-->

如果能以可靠的方式存取內容，若要以更一致的方式簽入，請前往特定的外部工具，例如：

* [WebAim對比檢查程式](https://webaim.org/resources/contrastchecker/){target="_blank"}和[WAVE網頁協助工具評估工具](https://wave.webaim.org/){target="_blank"}，以評估對比和相容性；

* 熒幕助讀程式之類的輔助技術(例如： [NVDA](https://www.nvaccess.org/download/){target="_blank"}，或iPhone上的[VoiceOver](https://support.apple.com/en-ie/guide/iphone/iph3e2e415f/ios){target="_blank"})，可從視障使用者的角度體驗電子郵件。

## 使用深色模式 {#dark-mode}

[深色模式](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"}可增強對光線敏感度或視覺障礙的使用者的視覺協助工具，以改善檢視體驗。

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

在深色模式中設計內容的一些最佳實務包括：

* 使用透明PNG或SVG
* 設定適當的中繼標籤和CSS
* 如果深色模式不受支援，則提供可存取的遞補樣式。

透過在淺色和深色模式下測試所有電子郵件內容和UI元素，確保您的電子郵件在深色模式下正確呈現。

## 針對協助工具使用特定屬性 {#attributes}

### 語言屬性 {#language}

建立設計時，請在內容本文中包含`lang` （語言）和`dir` （文字方向）屬性。 這些屬性可協助輔助技術（例如熒幕閱讀程式）以適當的方式解譯和呈現您的內容。

* `lang`屬性指出輔助技術所使用之電子郵件的語言，確保正確發音單字。

  +++範例

  英文範例：

  ```
  <body lang="en">
  ```

  法文範例：

  ```
  <body lang="fr">
  ```

  +++

* `dir`屬性指定文字方向。 大部分的語言，包括英文和法文，都是由左至右(ltr)閱讀，而阿拉伯文和希伯來文等語言則是由右至左(rtl)閱讀。

  +++範例

  英文範例（由左至右）：

  ```html
  <body lang="en" dir="ltr">
  ```

  阿拉伯文範例（由右至左）：

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

熒幕朗讀程式依賴`lang`屬性來套用正確的發音規則，而文字方向可確保內容從左至右或從右至左的語言自然流暢。 如果沒有這些屬性，使用者可能會遇到閱讀順序混亂或發音錯誤的情況。 請一律使用適當的`lang`和`dir`屬性包住您的電子郵件內文。

>[!TIP]
>
>如果您的電子郵件包含多種語言，請將適當的語言屬性指派給特定區段（例如`<table>`或`<td>`區塊），以確保每個部分都可正確讀取。

### 表格 {#tables}

在HTML內容中，表格通常用於版面配置。 依預設，熒幕助讀程式會將每個`<table>`視為資料表，宣告列、欄和結構。 如果表格僅用於格式設定，這可能會造成混淆。

將`role="presentation"` （或`role="none"`）新增至配置表格，以確保輔助技術會略過其結構並僅專注於實際內容。

+++範例 — 配置表格（含`role="presentation"`）

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

熒幕助讀程式顯示：
「你好。 歡迎使用我們的電子報。」 _（未提及列、欄或資料表）_

+++

+++範例 — 資料表（不含`role="presentation"`）

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

熒幕助讀程式顯示：
「2欄3列的表格。」

「姓名，Peter。 分數，19。」

「姓名，帕克。 分數， 62。」

+++

>[!TIP]
>
>僅使用`role="presentation"`配置表格。 對於資料表，請保留語意`<table>`結構，讓熒幕朗讀程式可以正確宣告標題和關聯性。

### 連結文字 {#links}

熒幕助讀程式會使用文字朗讀連結。 如果連結僅標籤為「按一下這裡」或「閱讀更多」，則輔助技術的使用者將無法知道目的地。 為了確保協助工具，這些檔案需要清楚指出目標或動作的描述性文字。

使用電子郵件Designer為您的內容新增連結，並編輯標籤，使其可區分（可見）並具描述性（清除用途）。 避免使用模糊的標籤，如「這裡」或「更多」。

<!--![](assets/accessible-link.png){width="70%"}-->

+++範例 — 良好連結（描述性）： 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

熒幕助讀程式顯示：
「連結，8月發行說明。」

+++

+++範例 — 錯誤連結（非描述性）

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

熒幕助讀程式顯示：
「連結，按一下這裡。」 *（未提供讀取順序錯亂的內容）*

+++

<!--for Landing Pages-->

<!--## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.-->
