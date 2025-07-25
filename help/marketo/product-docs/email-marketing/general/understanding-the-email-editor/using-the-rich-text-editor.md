---
unique-page-id: 2953419
description: 使用Rtf編輯器 — Marketo檔案 — 產品檔案
title: 使用RTF編輯器
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 1%

---

# 使用RTF編輯器 {#using-the-rich-text-editor}

RTF編輯器(RTE)會顯示在整個Marketo中，您只要想要新增或編輯內容，都可使用此編輯器。 您會在登陸頁面、程式、電子郵件、表單和程式碼片段上看到版本。 只需按一下「**[!UICONTROL Edit Draft]**」，它就會彈現出來，為您服務。

## 編輯器設定 {#editor-settings}

根區塊元素設定會定義哪些標籤會包住您的內容。 依預設，電子郵件根區塊元素會使用`<p>`標籤。 您可以選擇按照以下步驟進行變更。

>[!TIP]
>
>雖然您可以選擇根區塊元素，我們一律建議您使用預設設定以獲得最佳的使用者體驗。

1. 按一下「**[!UICONTROL Admin]**」。

   ![](assets/one.png)

1. 按一下「**[!UICONTROL Email]**」。

   ![](assets/two.png)

1. 按一下「**[!UICONTROL Edit Text Editor Settings]**」。

   ![](assets/three.png)

1. 在&#x200B;**[!UICONTROL Email]/[!UICONTROL Snippet Editor]**&#x200B;下拉式清單中，選取`<div>`或[!UICONTROL None]並按一下&#x200B;**[!UICONTROL Save]**。 此範例中使用`<div>`。

   ![](assets/four.png)

   如果電子郵件範本中有`<div class=“mktEditable”></div>`，當您開啟區段並在編輯器中輸入「文字移至此處」時，將會看到下列HTML Source行為：

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>None</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;文字移至此處&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;文字移至此處&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>文字移至此處<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>您也可以按照相同步驟變更登入頁面編輯器的根區塊元素，但按一下步驟4中的&#x200B;**[!UICONTROL Landing Page Editor]**&#x200B;下拉式清單，而非[!UICONTROL Email] / [!UICONTROL Snippet Editor]。

>[!NOTE]
>
>RTF程式權杖的根區塊元素一律為`<p>`。

## 功能 {#features}

以下是您在RTE中可以找到的功能。

| 圖示 | 名稱 | 作用 |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | [!UICONTROL Font Family] | 選擇您的風格 — 我們有足夠的選擇！ |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | [!UICONTROL Font Size] | 您想要多大？ 25種選擇，從8px到90px。 |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | [!UICONTROL Styles] | 選擇「段落」或6種標題樣式（適用於登陸頁面）。 |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | [!UICONTROL Line Spacing] | 選取直線之間的距離。 |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | [!UICONTROL Text Color] | 黑色、紅色或您想要的任何顏色。 |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | [!UICONTROL Background Color] | 強調顯示。 |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | [!UICONTROL Bold] | **較深且較厚**。 |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | [!UICONTROL Italic] | *角度，強調或引號*。 |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | [!UICONTROL Underline] | 在文字下方加上線條。 |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | [!UICONTROL Alignment] | 使用此下拉式清單來配置文字和影像。 置中對齊、選擇靠左或靠右對齊，或以完全齊行的方式將邊緣展開至邊緣。 |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | 清單 | 從下拉式清單中選擇專案符號或數字。 專案符號很適合使用清單，數字適合使用步驟。 |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | [!UICONTROL Indent] | 選擇或多或少縮排。 用於段落或您要突顯的任何文字。 |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | [!UICONTROL Insert/Edit Link] | 放入網站或其他內容的連結；輕鬆進行變更。 |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | [!UICONTROL Insert/Edit Image] | 圖片千言萬語。 將其中一個。 按一下相機圖示以瀏覽您的Design Studio。 您可以並排放置影像。 |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | [!UICONTROL Insert Token] | 功能強大的工具，非常適合電子郵件個人化和資料追蹤。 請務必輸入預設值。 |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | [!UICONTROL Undo] | 糟糕！ 請回到上一步，然後再試一次。 |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | [!UICONTROL Redo] | 如果真的沒問題，請回到原始狀態。 |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | [!UICONTROL Table] | 建置您自己的檔案，就像這個。 下拉式功能表可讓您進行設定。 |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | [!UICONTROL Insert Anchor] | 放置錨點！ |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | [!UICONTROL Horizontal Line] | 許多用途 — 很適合分割區段。 |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | [!UICONTROL Edit HTML] | 彈出HTML Source編輯器，讓您調整程式碼。 |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | [!UICONTROL Subscript] | 低懸字母（如O`<sub>2</sub>`）。 |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | [!UICONTROL Superscript] | 您有超強的能力！ (2`<sup>6</sup>`)。 |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | [!UICONTROL Strikethrough] | `<s>Put a line through text, like this</s>`。 |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | [!UICONTROL Special Character] | 想聊聊歐元嗎？ 數學？ 您有243種選擇。 |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | [!UICONTROL Find and Replace] | 搜尋和變更專案的速度，會比自行尋找每個執行個體快得多。 |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | [!UICONTROL Clear Formatting] | 將專案恢復為標準。 |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | [!UICONTROL Cancel] | 按下按鈕說：「沒關係。」 |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | [!UICONTROL Save] | 按下按鈕說：「OK， I like it.」（確定，我喜歡。） |

>[!TIP]
>
>您可以在個別的熒幕上編輯HTML和文字。 請務必按一下「**[!UICONTROL Copy from HTML]**」標籤上的「**[!UICONTROL Text]**」，然後再按「**[!UICONTROL Save]**」，讓您的文字元合您的HTML。

>[!NOTE]
>
>下拉式清單中的字型不受任何限制。 您可以存取HTML程式碼，以使用未列出的程式碼。 Marketo支援所有Web字型，但Web字型並非在所有電子郵件使用者端中都能正常運作。

## 登陸頁面 {#landing-pages}

根區塊元素設定會定義哪些標籤會包住您的內容。 依預設，登入頁面根區塊元素會使用`<div>`標籤。 您可選擇依照下列步驟變更此設定。

>[!TIP]
>
>雖然您可以選擇根區塊元素，我們一律建議您使用預設設定以獲得最佳的使用者體驗。

1. 按一下「**[!UICONTROL Admin]**」。

   ![](assets/one.png)

1. 按一下「**[!UICONTROL Email]**」。

   ![](assets/two.png)

1. 按一下「**[!UICONTROL Edit Text Editor Settings]**」。

   ![](assets/three.png)

1. 在&#x200B;**[!UICONTROL Landing Page Editor]**&#x200B;下拉式清單中，選取`<p>`或[!UICONTROL None]並按一下&#x200B;**[!UICONTROL Save]**。 此範例中使用`<p>`。

   ![](assets/five.png)

   就是這樣！
