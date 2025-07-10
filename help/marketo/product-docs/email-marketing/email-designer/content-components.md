---
solution: Marketo Engage
product: marketo
title: 內容元件
description: 說明。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: ca8644c43cfbdbaf7be9f21c5e440949b796cfdb
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 0%

---

# 內容元件 {#content-components}

建立電子郵件內容時，**[!UICONTROL Content components]**&#x200B;可讓您使用原始元件進一步個人化電子郵件，這些元件一旦放入電子郵件中即可編輯。

您可以視需要在一個或多個結構元件中新增任意數量的內容元件，這些元件定義電子郵件的版面。

## 新增內容元件 {#add-content-components}

若要新增內容元件至您的電子郵件，並根據您的需求進行調整，請遵循下列步驟。

1. 在電子郵件Designer中，使用現有內容或將&#x200B;**[!UICONTROL Structure components]**&#x200B;拖放至您的空白內容中，以定義電子郵件的配置。`[Learn how](content-from-scratch.md)`

1. 若要存取&#x200B;**[!UICONTROL Content components]**&#x200B;區段，請從[電子郵件Designer]左窗格中選取對應的按鈕。

   熒幕擷圖

1. 將您選擇的內容元件拖放到相關結構元件內。

   熒幕擷圖

   >[!NOTE]
   >
   >您可以將數個元件加入單一結構元件中，並加入結構元件的每個欄中。

1. 使用右側的&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Style]**&#x200B;索引標籤，調整每個元件的屬性和樣式。 例如，您可以變更文字樣式、每個元件的邊框間距或邊界。`[Learn more about alignment and padding](alignment-and-padding.md)`

   熒幕擷圖

1. 從&#x200B;**[!UICONTROL Content component]**&#x200B;的進階功能表，您可以視需要輕鬆刪除或複製任何內容元件。

   熒幕擷圖

## 容器 {#container}

若要將特定樣式套用至一組內容元件，您可以新增&#x200B;**[!UICONTROL Container]**&#x200B;元件，然後在其中新增您想要的內容元件。 這可讓您將不同的樣式套用至容器，這會與套用至內部內容元件的樣式不同。

例如，新增&#x200B;**[!UICONTROL Container]**&#x200B;元件，然後在該容器中新增[Button](#button)元件。 您可以將特定背景用於容器，並將另一個背景用於按鈕。

熒幕擷圖

## 按鈕 {#button}

使用&#x200B;**[!UICONTROL Button]**&#x200B;元件將一或多個按鈕插入您的電子郵件，並將您的電子郵件對象重新導向至其他頁面。

1. 從&#x200B;**[!UICONTROL Content components]**，將&#x200B;**[!UICONTROL Button]**&#x200B;元件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 按一下您新新增的按鈕以個人化文字，並存取電子郵件Designer右窗格中的&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Styles]**&#x200B;索引標籤。

   熒幕擷圖

1. 從&#x200B;**[!UICONTROL Link]**&#x200B;功能表，新增您要在按一下按鈕時重新導向的URL。

1. 透過&#x200B;**[!UICONTROL Target]**&#x200B;下拉式清單選擇將您的對象重新導向的方式：

   * **[!UICONTROL None]**：在按一下連結的相同框架中開啟連結（預設）。
   * **[!UICONTROL Blank]**：在新視窗或索引標籤中開啟連結。
   * **[!UICONTROL Self]**：在同一個框架中開啟連結（與按一下連結時相同）。
   * **[!UICONTROL Parent]**：在父框架中開啟連結。
   * **[!UICONTROL Top]**：在視窗的完整內文中開啟連結。

   熒幕擷圖

1. 您可以變更樣式屬性（例如&#x200B;**[!UICONTROL Border]**、**[!UICONTROL Size]**、**[!UICONTROL Margin]**&#x200B;等），進一步個人化您的按鈕。 從&#x200B;**[!UICONTROL Component settings]**&#x200B;窗格。

## 文字 {#text}

使用&#x200B;**[!UICONTROL Text]**&#x200B;元件將文字插入您的電子郵件，並使用&#x200B;**[!UICONTROL Styles]**&#x200B;索引標籤調整樣式（邊框、大小、邊框間距等）。

熒幕擷圖

1. 從&#x200B;**[!UICONTROL Content components]**，將&#x200B;**[!UICONTROL Text]**&#x200B;元件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 按一下您新新增的元件，以個人化文字，並存取電子郵件Designer右窗格中的&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Styles]**&#x200B;索引標籤。

1. 使用工具列中的下列選項變更文字：

   熒幕擷圖

   * **[!UICONTROL Change text style]**：將粗體、斜體、底線或刪除線套用至您的文字。
   * **變更對齊方式**：選擇文字的靠左、靠右、置中或左右對齊。
   * **[!UICONTROL Create list]**：新增專案符號或編號清單至您的文字。
   * **[!UICONTROL Set heading]**：為您的文字最多新增六個標題層級。
   * **字型大小**：選取文字的字型大小（畫素）。
   * **[!UICONTROL Change font color]**：選擇字型的顏色。
   * **[!UICONTROL Insert link]**：將任何型別的連結新增至您的內容。
   * **[!UICONTROL Edit image]**：將影像或資產新增至文字元件。`[Learn more about asset management](../integrations/assets.md)`
   * **[!UICONTROL Change font color]**：選擇字型的顏色。
   * **[!UICONTROL Add personalization]**：新增個人化欄位，以自訂設定檔資料的內容。`[Learn more about content personalization](../personalization/personalize.md)`
   * **[!UICONTROL Show the source code]**：顯示文字的原始碼。 無法修改。
   * **[!UICONTROL Enable conditional content]**：新增條件式內容，以將元件的內容調整至目標設定檔。`[Learn more about dynamic content](../personalization/get-started-dynamic-content.md)`
   * **[!UICONTROL Duplicate]**：新增文字元件的復本。
   * **[!UICONTROL Delete]**：從您的電子郵件中刪除選取的文字元件。

1. 調整其他樣式屬性，例如文字顏色、字型系列、邊框、邊框間距、邊界等。 從&#x200B;**[!UICONTROL Styles]**&#x200B;索引標籤。

   熒幕擷圖

## 分隔線 {#divider}

使用&#x200B;**[!UICONTROL Divider]**&#x200B;元件插入分隔線，以組織電子郵件的版面配置和內容。

您可以從&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Styles]**&#x200B;標籤調整樣式屬性，例如線條顏色、樣式和高度。

熒幕擷圖

## HTML {#HTML}

使用&#x200B;**[!UICONTROL HTML]**&#x200B;元件來複製貼上現有HTML的不同部分。 這可讓您建立免費的模組化HTML元件，以重複使用某些外部內容。

1. 從&#x200B;**[!UICONTROL Content Components]**，將&#x200B;**[!UICONTROL HTML]**&#x200B;元件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 按一下新新增的元件，然後從內容工具列選取「**[!UICONTROL Show the source code]**」以新增HTML。

   熒幕擷圖

1. 複製並貼上您要新增至電子郵件的HTML程式碼，然後按一下&#x200B;**[!UICONTROL Save]**。

   熒幕擷圖

>[!NOTE]
>
>若要讓外部內容符合電子郵件Designer的規範，Adobe建議從草稿開始建立訊息，並將現有電子郵件的內容複製到元件中。

## 影像 {#image}

使用&#x200B;**[!UICONTROL Image]**&#x200B;元件將影像檔案從電腦插入電子郵件內容。

1. 從&#x200B;**[!UICONTROL Content components]**，將&#x200B;**[!UICONTROL Image]**&#x200B;元件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

   熒幕擷圖

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;索引標籤中，按一下&#x200B;**[!UICONTROL Browse]**&#x200B;以從您的資產選擇影像檔案，或按一下&#x200B;**[!UICONTROL Import media]**&#x200B;將資產上傳到Adobe Experience Manager Assets。

   若要深入瞭解[!DNL Adobe Experience Manager Assets]，請參閱[Adobe Experience Manager Assets檔案](https://experienceleague.adobe.com/docs/experience-manager-assets-essentials/help/introduction.html?lang=zh-Hant){target="_blank"}。

   >[!NOTE]
   >
   > 為確保您的連結維持作用中狀態並避免任何到期問題，我們建議您使用Adobe Assets，而不是仰賴影像的來源URL。

1. 您也可以使用&#x200B;**[!UICONTROL Find Adobe Stock photos]**&#x200B;選項直接在Adobe Stock中搜尋。

1. 按一下您新增的元件，然後設定影像屬性：

   * **[!UICONTROL Image title]**&#x200B;可讓您定義影像的標題。
   * **[!UICONTROL Alt text]**&#x200B;可讓您定義連結至影像的標題。 這會對應至alt HTML屬性。

   熒幕擷圖

1. 您也可以選擇&#x200B;**[!UICONTROL Find similar Stock photos]**。`[Learn more](../integrations/stock.md)`

1. 從&#x200B;**[!UICONTROL Styles]**&#x200B;索引標籤，調整其他樣式屬性，例如邊界、邊框等。 或新增連結以將您的對象重新導向至&#x200B;**[!UICONTROL Component settings]**&#x200B;窗格中的其他內容。

## 社交 {#social}

使用&#x200B;**[!UICONTROL Social]**&#x200B;元件將社群媒體頁面的連結插入您的電子郵件內容中。

1. 從&#x200B;**[!UICONTROL Content Components]**，將&#x200B;**[!UICONTROL Social]**&#x200B;元件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 選取您新新增的元件。

1. 在&#x200B;**[!UICONTROL Social]**&#x200B;索引標籤的&#x200B;**[!UICONTROL Settings]**&#x200B;欄位中，選擇要新增或移除的社群媒體。

   熒幕擷圖

1. 透過專用欄位選擇圖示的大小。

1. 按一下您的每個社群媒體圖示來設定您的對象將重新導向到的&#x200B;**[!UICONTROL URL]**。

   熒幕擷圖

1. 如有需要，您也可以從Assets變更每個社群媒體的圖示。

1. 調整其他樣式屬性，例如樣式、邊界、邊框等。 從&#x200B;**[!UICONTROL Styles]**&#x200B;索引標籤。

## 優惠決定 {#offer-decision}

使用&#x200B;**[!UICONTROL Offer decision]**&#x200B;元件將優惠插入您的訊息。 `[decision management](../offers/get-started/starting-offer-decisioning.md)`引擎會挑選要遞送給客戶的最佳優惠方案。

1. 從&#x200B;**[!UICONTROL Content Components]**，將&#x200B;**[!UICONTROL Offer decision]**&#x200B;元件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 按一下&#x200B;**[!UICONTROL Add]**&#x200B;以選取您的&#x200B;**[!UICONTROL Offer decision]**。

   熒幕擷圖

1. 從下拉式清單中選取您的&#x200B;**[!UICONTROL Placements]**。  然後，選取您要新增至內容的&#x200B;**[!UICONTROL Offer decision]**，然後按一下&#x200B;**[!UICONTROL Add]**。

   熒幕擷圖

1. 從&#x200B;**[!UICONTROL Offer decision]**&#x200B;索引標籤，您可以預覽或變更插入的選件。

瞭解如何在`[this section](add-offers-email.md)`中將個人化優惠新增至電子郵件。

>[!IMPORTANT]
>
>如果對歷程訊息中使用的優惠決定進行變更，您需要取消發佈歷程並重新發佈。  這將確保將變更納入歷程的訊息中，並且該訊息與最新更新一致。

