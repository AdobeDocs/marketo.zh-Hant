---
unique-page-id: 7515401
description: Learn how to create a guided landing page template in Marketo. Use syntax to define editable regions and variables for the guided editor.
title: 建立引導式登陸頁面範本
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 4a95c37fe8c09cdbe3cc84e701f0fc50286fc276
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 21%

---

# 建立引導式登陸頁面範本 {#create-a-guided-landing-page-template}

Guided landing page templates have a special syntax. Use this syntax to specify what is customizable and where content will end up on each landing page built from your template. Only the regions or variables you specify as editable will be available for customization within the &quot;Guided&quot; landing page editor.

>[!TIP]
>
>Use good naming conventions and your marketing team will fall in love with you.

There are two ways to declare that something on your page should be editable:

* Declare an object as an &quot;element&quot;. The landing page creator will be able to add images, text, or Marketo assets into those specified regions.
* Declare a string as a &quot;variable&quot;. The landing page creator will be able to replace that variable with a string, color, or boolean state from a true/false lever.

## Editable Elements {#editable-elements}

Elements are declared by adding a normal DOM element to the template, then decorating the element with a Marketo-specific class name.

## 文字 {#text}

如果您將區域定義為 RTF 文字，則使用者即可](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)使用 Marketo 的 RTF 文字編輯器[編輯其內容。

Required attributes:
**class**：&quot;mktoText&quot;
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 This is the display name that will be shown in the landing page editor. Best practice is to use a descriptive name.

Optional:
The content of an element with class mktoText (if provided) will be used as the default value for the editable region.

範例：

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## 影像 {#image}

You have two options for defining editable Image Elements. You may use either a `<div>`, which specifies a container that the image will be inserted into, or an `<img>` tag.

## 選項 1 — 使用 `<div>` {#option-use-a-div}

Required attributes:

class: &quot;mktoImg&quot;
id: ID string. 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
mktoName : String. This is the display name that will be shown in the landing page editor. 最佳實務是使用描述性名稱。

可選：
mktoImgClass：字串。 這裡的值會新增至 div 內 `<img>` 元素的類別屬性。

範例：

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## 選項 2 — 使用 `<img>` {#option-use-a-img}

必要的屬性：
類別： &quot;mktoImg&quot;
ID：ID字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
mktoName ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：
src：字串URL。 這將做為影像的預設值。

範例：

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>使用`<img>`版本時，轉譯的HTML將在`<img>`標籤周圍包含產生的div包裝函式。 它將設定為class .&quot;mktoImg.mktoGen&quot;，並將顯示:inline-block。

## 表單 {#form}

範例:Required屬性：
**類別**： &quot;mktoForm&quot;
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## 程式碼片段 {#snippet}

必要的屬性：
**類別**： &quot;mktoSnippet&quot;
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## 共用按鈕 {#share-button}

必要的屬性：
**類別**： &quot;mktoShareButton&quot;
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## 影片 {#video}

>[!NOTE]
>
>在登入頁面中使用視訊元素時，Marketo僅支援來自YouTube的視訊。 如果您使用其他服務，建議使用RTF文字方塊並在視訊的內嵌程式碼中貼上。

必要的屬性：
**類別**： &quot;mktoVideo&quot;
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## 可編輯的變數 {#editable-variables}

所有變數型別都是透過參照包在${ }字元序列中的id屬性值來使用。 除了在其他變數宣告的內部，它們可以在檔案中的任何位置使用。

範例：

`${var1}`

**宣告：**

變數在範本的`<head>`元素內宣告為中繼標籤。 有三種型別的變數可供使用：字串、顏色和布林值。

## 字串 {#string}

必要的屬性：
**類別** ： &quot;mktoString&quot;，
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：
**預設**：屬性的字串值。 如果未提供，則為空白。
**allowHtml**： &quot;true&quot;或&quot;false&quot;。 控制是否會在未逸出HTML的情況下列印值。 若未設定，則預設值為「false」。

基本範例：

`<meta class="mktoString" id="var1" mktoName="My Variable">`

具有所有屬性的範例：

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## 顏色 {#color}

必要的屬性：
**類別** ： &quot;mktoColor&quot;，
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：
**預設**： 7位數的十六進位字元色彩代碼。 例如：「#336699」

基本範例：

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

具有所有屬性的範例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## 布林值 {#boolean}

必要的屬性：
**類別** ： &quot;mktoBoolean&quot;，
**id**：識別碼字串。 僅包含字母、數字、破折號「-」和底線「_」。 不允許有任何空格。 必須為唯一。
**mktoName**：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：
**預設**：布林字串。 「true」或「false」控制值是否從ON或OFF位置開始。 &quot;false&quot; （若未提供）。
**false_value**：字串。 當變數處於OFF位置時要插入的值。 &quot;false&quot; （若未提供）。
**true_value**：字串。 當變數處於「開啟」位置時要插入的值。 若未提供，則為&quot;true&quot;。
**false_value_name**：字串。 The display name to be shown in the landing page editor when the value is in the OFF position. &quot;OFF&quot; if not provided.
**true_value_name**: String. The display name to be shown in the landing page editor when the value is in the ON position. &quot;ON&quot; if not provided.

基本範例：

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

具有所有屬性的範例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

This example shows a common use case where a boolean variable controls the visibility of a css element by setting the value of css display property to either &quot;block&quot; or &quot;none&quot; to show/hide an element by id with CSS. The landing page editor will use the display name Show/Hide instead of OFF/ON.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Program tokens (my.token) can also be used anywhere in Guided or Free-form landing pages.
