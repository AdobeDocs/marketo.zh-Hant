---
solution: Marketo Engage
product: marketo
title: 標題
description: 瞭解如何使用可重複使用的主題和模組來簡化電子郵件建立，確保設計一致性和效率。
feature: Email Designer
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: 1cfb28f47ba3c168292b298e1fc7ab2ff638b412
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# 對您的電子郵件內容套用主題 {#apply-email-themes}

>[!AVAILABILITY]
>
>此功能目前為 Beta 版本，僅供 Beta 版客戶使用。若要加入 Beta 版計畫，請聯絡 Adobe 代表。

透過主題，非技術使用者能藉由在標準範本<!-- to achieve brand specific results-->上新增自訂樣式，建立符合特定品牌和設計語言的可重複使用內容。

此功能可讓行銷人員更快且更輕鬆地運用視覺上吸引人、品牌一致的電子郵件，同時提供進階自訂選項以滿足獨特的設計需求。

<!--What is the Enhanced Email Authoring Experience?

This feature introduces two key components to simplify and enhance email creation:

* **Theme Management System**: A centralized system for creating, customizing, and applying reusable themes to emails. Themes ensure consistent styling across campaigns and eliminate the need for repetitive manual styling.

* **Modules**: Pre-designed, reusable content blocks that abstract common email elements (e.g., titles, descriptions, images, and links). Modules are built using customizable low-level components, offering flexibility while maintaining design standards.

Key Benefits:

- **Consistency**: Ensure all emails align with your brand's design guidelines.
- **Efficiency**: Save time by reusing themes and modules across campaigns.
- **Customization**: Add custom CSS and mobile-specific styles for advanced designs.
- **Scalability**: Eliminate repetitive styling tasks, enabling faster email creation.-->

## 護欄與限制 {#themes-guardrails}

* 從頭開始建立電子郵件時，您可以選擇使用主題開始建立內容，以快速套用符合您的品牌和設計的特定樣式。

  如果您選擇&#x200B;_手動樣式_&#x200B;模式，除非重設電子郵件，否則您將無法套用任何主題。

* [片段](/help/marketo/product-docs/email-marketing/email-designer/fragments.md)在&#x200B;_使用主題_&#x200B;和&#x200B;_手動樣式化_&#x200B;模式之間不相容。

  若要能夠在套用了主題的內容中使用片段，此片段必須以&#x200B;_使用主題_&#x200B;模式建立。

* 如果使用HTML中建立的內容，您將會處於[相容性模式](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html)，且無法將主題套用至此內容。

  若要充分利用Email Designer的所有功能，包括主題，您必須在&#x200B;_使用主題_&#x200B;模式中建立新內容，或轉換您的[匯入的HTML內容](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html)。

<!--If using a content created in Manual Styling mode or HTML, you cannot apply themes to this content. You must create a new content in Use Themes mode.

If you apply a theme to a content using a [fragment](../content-management/fragments.md) created in Manual Styling mode, the rendering may not be optimal.-->

## 建立主題 {#create-and-edit-themes}

若要定義您可在未來電子郵件內容中運用的主題，請遵循下列步驟。

1. 若要開始，請建立新的[電子郵件範本](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)。

1. 選取&#x200B;**[!UICONTROL Create or edit themes]**&#x200B;選項。

   `![](assets/theme-create.png)`

1. 您可以選取預設主題，或使用Adobe或自訂範本。 在此範例中，選取預設主題並按一下&#x200B;**[!UICONTROL Create]**。

   `![](assets/theme-select.png)`

1. 在&#x200B;**[!UICONTROL General settings]**&#x200B;索引標籤中，為您的品牌指定特定名稱，以開始定義您的主題。 您可以調整電子郵件的預設寬度，也可以匯出目前的佈景主題以在沙箱之間共用。

   `<!--![](assets/theme-general-settings.png)-->`

1. 使用右側的邊欄瀏覽不同的標籤並更新您的設計設定。

   `![](assets/theme-right-pane.png)`

1. 從&#x200B;**[!UICONTROL Colors]**&#x200B;索引標籤：

   * 使用&#x200B;**[!UICONTROL Edit]**&#x200B;按鈕為您的品牌設定預設顏色的&#x200B;**[!UICONTROL Color palette]**。 選取&#x200B;**[!UICONTROL Preset]**&#x200B;以快速建立色彩配置，或個別調整佈景主題的每種顏色。 您也可以使用兩者的組合。

     `![](assets/theme-colors.gif)`

   * 按一下&#x200B;**[!UICONTROL Add variant]**&#x200B;建立多種顏色變體，例如淺色和深色模式，每個變體都有自己的調色盤和細微控制項。

     `![](assets/theme-colors-variant.png)`

   * 對於每個變體，按一下「編輯」圖示以編輯任何個別元素。 您可以使用已建立的預設調色盤或任何自訂顏色。

     `![](assets/theme-colors-edit-variant.gif)`

1. 在&#x200B;**[!UICONTROL Text settings]**&#x200B;中，您可以設定要用於整個佈景主題的全域字型。 如需更細微的控制項，您也可以編輯每個標題和段落型別，以調整字型、大小、樣式等。

   `![](assets/theme-text.png)`

1. 在&#x200B;**[!UICONTROL Spacing]**&#x200B;索引標籤中，從清單中選取個別元素，以便在不同元件之間適當地間隔該元素。

   `<!--![](assets/theme-spacing.png)-->`

1. 使用右側的其他索引標籤，您可以分別管理此主題的每個按鈕元素、分隔線、其他影像格式和格線版面間距。

   `<!--![](assets/theme-buttons.png)-->`

1. 按一下&#x200B;**[!UICONTROL Save]**&#x200B;儲存此主題以供日後使用。

## 套用主題至電子郵件 {#apply-themes}

若要套用預設或自訂樣式主題至電子郵件，請遵循下列步驟。

1. `In [!DNL Marketo Engage], [add an email](create-email.md) action to a journey or campaign, and [edit your email body](get-started-email-design.md#key-steps).`

1. 您可以選取下列其中一個動作：

   * `Select a built-in [email template](use-email-templates.md) to open the Email Designer. A default theme specific to each template is automatically applied.`

   * `Design a [new content from scratch](content-from-scratch.md) and select **[!UICONTROL Use Themes]** to start with a predefined styling theme.`

     `![](assets/theme-from-scratch.png)`

     >[!CAUTION]
     >
     >如果您選擇&#x200B;_手動樣式_&#x200B;模式，除非重設電子郵件，否則您將無法套用任何主題。
     >
     >若要在[使用佈景主題](/help/marketo/product-docs/email-marketing/email-designer/fragments.md)模式中使用&#x200B;_片段_，此片段必須已使用&#x200B;_使用佈景主題_&#x200B;模式自行建立。

1. 在電子郵件Designer中，按一下右側邊欄上的&#x200B;**[!UICONTROL Themes]**&#x200B;按鈕。 預設主題或範本主題隨即顯示。 您可以在此佈景主題的兩個顏色變體之間切換。

   `![](assets/theme-default-hero.png)`

1. 按一下目前使用之主題旁的箭頭。 可用的自訂和Adobe主題清單隨即顯示。

   `![](assets/theme-hero-change.png)`

1. 按一下&#x200B;**[!UICONTROL Custom themes]**&#x200B;並選取您建立的主題。

   `![](assets/theme-select-custom.png)`

1. 按一下下拉式清單外部。 新選取的自訂主題會自動將其樣式套用至所有電子郵件元件。 您可以在兩種顏色變體之間切換。

1. 選取元件時，您仍可使用專用圖示來解除鎖定其樣式。

   `![](assets/theme-unlock-style.png)`

您可以隨時切換主題。 電子郵件內容保持不變，但樣式會更新以反映新主題。

<!--
>[!NOTE]
> - Themes apply styles globally. Ensure your theme is finalized before applying it to multiple emails.
> - Switching themes may override custom styles applied to individual components.

>[!CAUTION]
> - When using fragments, the email's theme will override the fragment's styles. A warning will be displayed in the editor if there is a conflict.

## Example Use Cases {#example-use-cases}

### 1. Creating a New Theme
- A marketer creates a theme with their brand's colors, fonts, and button styles.
- The theme is saved and reused across multiple email campaigns.

### 2. Switching Themes
- A marketer applies a holiday-themed design to an existing email by switching to a pre-designed holiday theme.-->
