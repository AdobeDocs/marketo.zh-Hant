---
unique-page-id: 7515401
description: 建立引導式登陸頁面範本 — Marketo檔案 — 產品檔案
title: 建立引導式登陸頁面範本
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 0%

---

# 建立引導式登陸頁面範本 {#create-a-guided-landing-page-template}

引導式登入頁面範本有特殊語法。 使用此語法來指定可自訂的專案，以及內容在由您的範本建立的每個登入頁面上的結束位置。 只有您指定為可編輯的區域或變數，才能在「引導式」登陸頁面編輯器中自訂。

>[!TIP]
>
>使用良好的命名慣例，您的行銷團隊就會愛上您。

有兩種方式可宣告頁面上的某個專案應為可編輯：

* 將物件宣告為「element」。 登入頁面建立者將能夠新增影像、文字或Marketo資產至這些指定區域。
* 將字串宣告為「變數」。 登入頁面建立者將能夠從true/false槓桿以字串、顏色或布林值狀態取代該變數。

## 可編輯元素 {#editable-elements}

宣告元素的方法為新增一般DOM元素至範本，然後以Marketo特定的類別名稱裝飾元素。

## 文字 {#text}

如果您將區域定義為RTF文字，使用者將可以編輯其內容 [使用Marketo的RTF編輯器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

必要的屬性：\
**類別**： &quot;mktoText&quot;\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
具有類別mktoText的元素內容（如果提供）將當作可編輯區域的預設值。

範例：

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## 影像 {#image}

您有兩個選項可定義可編輯的影像元素。 您可以使用 `<div>`，指定影像要插入的容器，或 `<img>` 標籤之間。

## 選項1 — 使用 `<div>` {#option-use-a-div}

必要的屬性：

類別： &quot;mktoImg&quot;\
ID：ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
mktoName ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
mktoImgClass：字串。 此處的值將新增至 `<img>` div內的元素。

範例：

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## 選項2 — 使用 `<img>` {#option-use-a-img}

必要的屬性：\
類別： &quot;mktoImg&quot;\
ID：ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
mktoName ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
src：字串URL。 這將做為影像的預設值。

範例：

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>使用時 `<img>` 版本，則呈現的HTML將包含 `<img>` 標籤之間。 它將會設定為類別。」mktoImg.mktoGen」和，則會顯示：inline-block。

## 表單 {#form}

範例：必要的屬性：\
**類別**： &quot;mktoForm&quot;\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## 程式碼片段 {#snippet}

必要的屬性：\
**類別**： &quot;mktoSnippet&quot;\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## 共用按鈕 {#share-button}

必要的屬性：\
**類別**：&quot;mktoShareButton&quot;\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## 視訊 {#video}

>[!NOTE]
>
>在登入頁面中使用視訊元素時，Marketo僅支援來自YouTube的視訊。 如果您使用其他服務，建議使用RTF文字方塊並在視訊的內嵌程式碼中貼上。

必要的屬性：
**類別**： &quot;mktoVideo&quot;
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## 投票 {#poll}

必要的屬性：\
**類別**： &quot;mktoPoll&quot;\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## 轉介 {#referral}

必要的屬性：\
**類別**： &quot;mktoReferral&quot;\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## 抽獎 {#sweepstakes}

必要的屬性：\
**類別**： &quot;mktoSweepstackes&quot;\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## 可編輯的變數 {#editable-variables}

所有變數型別都是透過參照包在${ }字元序列中的id屬性值來使用。 除了在其他變數宣告的內部，它們可以在檔案中的任何位置使用。

範例：

`${var1}`

**宣告：**

變數在內宣告為中繼標籤 `<head>` 範本的元素。 有三種型別的變數可供使用：字串、顏色和布林值。

## 字串 {#string}

必要的屬性：\
**類別** ：&quot;mktoString&quot;，\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
**預設**：屬性的字串值。 如果未提供，則為空白。\
**allowHtml**：&quot;true&quot;或&quot;false&quot;。 控制是否列印值而不進行HTML逸出。 若未設定，則預設值為「false」。

基本範例：

`<meta class="mktoString" id="var1" mktoName="My Variable">`

具有所有屬性的範例：

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## 顏色 {#color}

必要的屬性：\
**類別** ：&quot;mktoColor&quot;，\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
**預設**：7位數的十六進位字元色彩代碼。 例如：「#336699」

基本範例：

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

具有所有屬性的範例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## 布林值 {#boolean}

必要的屬性：\
**類別** ：&quot;mktoBoolean&quot;，\
**id**： ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** ：字串。 這是將顯示在登入頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
**預設**：布林值字串。 「true」或「false」控制值是否從ON或OFF位置開始。 &quot;false&quot; （若未提供）。\
**false_value**：字串。 當變數處於OFF位置時要插入的值。 &quot;false&quot; （若未提供）。\
**true_value**：字串。 當變數處於「開啟」位置時要插入的值。 若未提供，則為&quot;true&quot;。\
**false_value_name**：字串。 當值處於「關閉」位置時，要在登入頁面編輯器中顯示的顯示名稱。 若未提供，則為「關閉」。\
**true_value_name**：字串。 當值位於「開啟」位置時，要在登入頁面編輯器中顯示的顯示名稱。 若未提供，則為「開啟」。

基本範例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

具有所有屬性的範例：

此範例顯示一個常見的使用案例，其中的布林值變數會將css display屬性的值設為「block」或「none」，藉此控制css元素的可見度，進而使用CSS依ID顯示/隱藏元素。 登入頁面編輯器將使用顯示名稱Show/Hide來取代OFF/ON。

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>程式權杖(my.token)也可在引導式或自由表單登陸頁面中的任意位置使用。
