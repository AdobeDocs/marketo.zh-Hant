---
solution: Marketo Engage
product: marketo
title: 可自訂的片段
description: 瞭解如何透過讓一些欄位可編輯來自訂片段。 在電子郵件Designer中建立靈活的可重複使用片段。
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: fdc003d7aed05d85687427d9455bb806eb33d0b2
workflow-type: tm+mt
source-wordcount: 1398
ht-degree: 0%

---

# 可自訂的片段 {#customizable-fragments}

在電子郵件或電子郵件範本中使用片段時，依預設會因繼承而鎖定，這表示對片段所做的任何變更都會自動傳播至使用它的所有資產。 有了可自訂的片段，當片段新增到電子郵件或電子郵件範本時，片段中的特定欄位可以定義為可編輯。 例如，如果您的片段具有橫幅、某些文字和按鈕，您可以將某些欄位（例如影像或按鈕目標URL）指定為可編輯。

可自訂的片段可讓您管理和個人化內容，而不會建立全新的內容區塊或中斷片段繼承。 在片段層級進行的變更仍會傳播，同時允許在電子郵件或電子郵件範本層級自訂。

視覺效果和運算式片段都可以標示為可自訂。

## 在視覺片段中新增可編輯欄位 {#visual}

若要讓視覺化片段的某些部分可編輯，請遵循下列步驟：

>[!NOTE]
>
>可編輯的欄位可新增至&#x200B;**影像**、**文字**&#x200B;和&#x200B;**按鈕**&#x200B;元件。 針對&#x200B;**HTML**&#x200B;元件，使用個人化編輯器新增可編輯的欄位，類似於運算式片段。 [瞭解片段HTML元件中可編輯的欄位](#editable-html)

1. 開啟片段內容版本畫面。

1. 選取片段中要設定可編輯欄位的元件。

1. 元件屬性窗格會在右側開啟。 選取「**[!UICONTROL Editable fields]**」標籤，然後切換「**[!UICONTROL Enable edition]**」選項。

1. 窗格中會列出所有可編輯所選元件的欄位。 可編輯的欄位取決於所選的元件型別。

   在以下範例中，「按一下這裡」按鈕URL已設定為可編輯。

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL Overview]**&#x200B;以檢查所有可編輯的欄位及其預設值。

   在此範例中，按鈕URL欄位會以元件中定義的預設值顯示。 將片段新增至使用者內容後，使用者可以自訂此值。

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. 完成時儲存變更。

將片段新增到電子郵件後，使用者可以自訂片段中設定的所有可編輯欄位。

## 片段中的可編輯HTML元件 {#editable-html}

在HTML元件中，下列型別的元素可以變成可編輯：

* **文字內容**&#x200B;的一部分（例如，標題或CTA標籤）。
* 完整的&#x200B;**URL**，用作連結目標或影像來源。 不支援部分URL；變數必須代表整個URL值。
* 完整的&#x200B;**CSS屬性值** （例如，全色值、全邊框間距值或全寬度值）。 不支援部分CSS屬性值。

每個引數化CSS屬性值必須剛好是`{{{varName}}}`：沒有尾碼、沒有額外的文字、沒有多個變數，以及單一屬性內沒有串連。

若要將多側屬性（例如內距）引數化，請執行下列其中一項操作：

* 將每一方宣告為個別屬性&#x200B;_（建議使用）_，或
* 宣告包含完整速記值的單一變數。

## HTML元件中可編輯欄位的運作方式 {#components}

HTML元件中的可編輯欄位是透過直接在元件的原始程式碼中宣告內嵌變數來建立。 每個變數都有唯一的ID和預設值。 接著會參考變數，指出可編輯值在標籤中出現的位置。

儲存並發佈片段後，在將片段新增至電子郵件時，HTML元件中宣告的每個變數都會自動顯示為可編輯的引數。

電子郵件作者接著可以覆寫電子郵件Designer中任何變數的預設值（例如，變更背景顏色、交換CTA URL或更新標題），而不需修改基礎的HTML。

## 語法參考 {#syntax}

可編輯欄位會使用兩種模式來定義和參照：

### 宣告變數 {#declaring}

使用內嵌宣告來定義具有唯一ID和預設值的變數：

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

將`variableID`取代為可編輯欄位的唯一識別碼。 ID在元件中必須是唯一的，且不得包含空格。

以電子郵件作者未覆寫時應使用的值取代`default_value`。

### 參考變數 {#referencing}

使用三大括弧來參照變數，無論其值在標籤中出現的位置：

```handlebars
{{{variableID}}}
```

在HTML中，可多次參照相同的變數ID。 所有參考都將解析為電子郵件作者設定的任何值（如果未提供覆寫，則解析為預設值）。

### 選用引數 {#optional}

內嵌宣告支援可變更可編輯欄位呈現或處理方式的選用引數：

| 動作 | 參數 | 範例 |
|---|---|---|
| 宣告具有&#x200B;**預設值**&#x200B;的可編輯欄位。 將片段新增至電子郵件時，除非作者覆寫該片段，否則會使用此預設值。 | 在內嵌標籤之間新增預設值。 | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| 為可編輯欄位定義&#x200B;**標籤**。 當電子郵件作者編輯片段的欄位時，此標籤會顯示在電子郵件Designer中。 | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| 宣告包含&#x200B;**影像來源**&#x200B;的可編輯欄位。 | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| 宣告包含需要追蹤之&#x200B;**URL**&#x200B;的可編輯欄位。 | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## 將可編輯欄位新增至HTML元件 {#adding-editable-fields}

若要讓視覺片段中HTML元件的某些部分可供編輯，請遵循下列步驟：

1. 開啟視覺化片段，以便在電子郵件Designer中編輯。
1. 從「元件」面板新增&#x200B;**HTML元件**&#x200B;至片段，或選取現有的HTML元件。
1. 選取HTML元件後，按一下&#x200B;**顯示原始程式碼**&#x200B;以在個人化編輯器中開啟HTML原始程式碼檢視。
1. 在個人化編輯器中，使用內嵌宣告語法來宣告每個可編輯的變數。 將所有變數宣告放在元件的頂端以提高可讀性，並為每個變數指派唯一的ID。
1. 在可編輯值出現的任何地方，使用`{{{variableID}}}`語法參考HTML標籤中的每個變數。 同一變數可在同一元件中參照多次。
1. 儲存HTML元件，然後儲存片段。
1. 發佈片段以使其可用於電子郵件。

## 在電子郵件中使用片段 {#using-fragment}

片段發佈後，在其HTML元件中宣告的所有變數，都會在電子郵件Designer中顯示為可編輯的引數。

若要在電子郵件中使用片段時自訂這些專案：

1. 在Marketo Engage電子郵件Designer中開啟或建立電子郵件。
1. 將發佈的片段新增至電子郵件畫布。
1. 選取片段以開啟其屬性窗格。 可編輯欄位清單會顯示在&#x200B;**可編輯欄位**&#x200B;區段下，每個欄位均以變數ID （或透過`name`引數指定的易記標籤）標示。
1. 直接從屬性窗格更新任何可編輯欄位的值。 此變更僅套用至目前的電子郵件；已發佈的片段和參照該片段的其他電子郵件不受影響。
1. 儲存電子郵件。

片段會以自訂值呈現，同時仍會繼承對已發佈片段所做的任何未來結構更新。

### 範例：具有可編輯文字、顏色和URL的簡單片段 {#example}

下列範例會建立包含四個可編輯欄位的小型促銷橫幅：

* 背景顏色
* 標題文字
* CTA標籤
* CTA URL

發佈片段後，電子郵件作者可以在將片段新增至電子郵件時覆寫這些值。

**簡單可編輯的橫幅**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

在此範例中，

* `bgColor`參考了兩次：一次為表格背景顏色，另一次為CTA文字顏色。 兩個參照會解析為相同的值，因此單一編輯會傳播至兩個位置。
* `ctaUrl`是以`assetType="url"`宣告，這表示值應該作為追蹤的URL處理。

## 最佳做法 {#best-practices}

* 在變數的預設值中包含單位(`px`、`em`、`%`)，讓變數代表完整的CSS值。 這樣可避免不支援的串連。
* 可能需要單獨編輯每一方時，偏好使用每方longhand CSS屬性(`padding-top`、`padding-right`、`padding-bottom`、`padding-left`)而非簡寫。
* 當需要追蹤URL時，請使用`assetType="url"`宣告URL。
* 當可編輯欄位包含影像來源時，請使用`assetType="image"`宣告它。
* 將片段新增至草稿電子郵件，然後驗證所有可編輯的欄位是否出現在屬性窗格中，並在覆寫時正確解析，以測試片段。

## 注意事項 {#things-to-know}

* HTML元件中的可編輯欄位支援完整文字內容、完整URL和完整CSS屬性值。 部分URL和部分CSS屬性值無法引數化。
* 單一CSS屬性值不能將變數與其他靜態文字或其他變數結合。 每個引數化的屬性值必須剛好是一個變數參考。
* 變數ID在HTML元件中必須是唯一的，且不得包含空格。
* 現成可用的系統連結（例如取消訂閱連結和映象頁面URL）無法轉換為可編輯的欄位。

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[片段](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
