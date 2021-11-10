---
unique-page-id: 7515401
description: 建立引導式登錄頁面範本 — Marketo檔案 — 產品檔案
title: 建立引導式登錄頁面範本
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
source-git-commit: c309b69198c6f61d7475c6d3a6b1672e045b9b4a
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 0%

---

# 建立引導式登錄頁面範本 {#create-a-guided-landing-page-template}

引導式登錄頁面範本有特殊語法。 使用此語法來指定可自訂的內容，以及內容在從範本建立的每個登錄頁面上的結尾。 只有您指定為可編輯的地區或變數才可在「引導式」登錄頁面編輯器中自訂。

>[!TIP]
>
>使用良好的命名慣例，您的行銷團隊就會愛上您。

有兩種方式可宣告您的頁面上的某個項目應可編輯：

* 將物件宣告為「元素」。 登錄頁面建立者將能將影像、文字或Marketo資產新增至這些指定區域。
* 將字串宣告為「變數」。 登錄頁面建立者將能以true/false槓桿的字串、顏色或布林狀態取代該變數。

## 可編輯的元素 {#editable-elements}

將一般DOM元素新增至範本，然後使用Marketo特定類別名稱裝飾元素，以宣告元素。

## 文字 {#text}

如果您將地區定義為RTF，使用者將能夠編輯其內容 [使用Marketo的RTF編輯器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

必要屬性：\
**類**:&quot;mktoText&quot;\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
具有類別mktoText的元素內容（若有提供）將用作可編輯區域的預設值。

範例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

## 影像 {#image}

定義可編輯的影像元素有兩個選項。 您可以使用 `<div>`，指定要插入影像的容器或 `<img>` 標籤。

## 選項1 — 使用 `<div>` {#option-use-a-div}

必要屬性：

類別：&quot;mktoImg&quot;\
id:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
mktoName :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
mktoImgClass:字串。 此處的值將新增至的類別屬性 `<img>` div內的元素。

範例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## 選項2 — 使用 `<img>` {#option-use-a-img}

必要屬性：\
類別：&quot;mktoImg&quot;\
id:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
mktoName :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
src:字串URL。 這將用作影像的預設值。

範例：

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>使用 `<img>` 版本中，呈現的HTML將包含在 `<img>` 標籤。 會設為類別。」mktoImg.mktoGen,&quot;和將為display:inline-block。

## 表單 {#form}

範例：必要屬性：\
**類**:&quot;mktoForm&quot;\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## 程式碼片段 {#snippet}

必要屬性：\
**類**:&quot;mktoSnippet&quot;\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## 共用按鈕 {#share-button}

必要屬性：\
**類**:&quot;mktoShareButton&quot;\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## 影片 {#video}

>[!NOTE]
>
>在登錄頁面中使用影片元素時，Marketo僅支援YouTube的影片。 如果您使用其他服務，建議您使用RTF方塊並貼入視訊的內嵌程式碼。

必要屬性：
**類**:&quot;mktoVideo&quot;
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## 投票 {#poll}

必要屬性：\
**類**:&quot;mktoPoll&quot;\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## 轉介 {#referral}

必要屬性：\
**類**:&quot;mktoReferral&quot;\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## 抽獎 {#sweepstakes}

必要屬性：\
**類**:&quot;mktoSweepstakes&quot;\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## 可編輯的變數 {#editable-variables}

所有變數類型都透過參考兩側加上${ }字元序列的其id屬性值來使用。 這些變數可在檔案中的任何位置使用，但其他變數宣告內除外。

範例：

`<pre data-theme="Confluence">${var1}</pre>`

**聲明：**

變數在 `<head>` 範本的元素。 可用的變數類型有三種：字串、顏色和布林值。

## 字串 {#string}

必要屬性：\
**類** :&quot;mktoString&quot;,\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
**預設**:屬性的字串值。 若未提供，則留空。\
**allowHtml**:&quot;true&quot;或&quot;false&quot;。 控制是否將打印值而未HTML轉義。 若未設定，則預設為「false」。

基本範例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

所有屬性的範例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## 顏色 {#color}

必要屬性：\
**類** :&quot;mktoColor&quot;,\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
**預設**:7位數的十六進位字元顏色代碼。 例如：&quot;#336699&quot;

基本範例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

所有屬性的範例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## 布林值 {#boolean}

必要屬性：\
**類** :&quot;mktoBoolean&quot;,\
**id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。\
**mktoName** :字串。 這是將顯示在登錄頁面編輯器中的顯示名稱。 最佳實務是使用描述性名稱。

可選：\
**預設**:布林字串。 「true」或「false」會控制值是否在「開啟」或「關閉」位置開始。 若未提供，則為「false」。\
**false_value**:字串。 要為變數插入的值，當它處於「關閉」位置時。 若未提供，則為「false」。\
**true_value**:字串。 要為變數插入的值，當它處於「開啟」位置時。 若未提供，則為「true」。\
**false_value_name**:字串。 當值位於「關閉」位置時，要在登錄頁面編輯器中顯示的顯示名稱。 若未提供，則設為「OFF」。\
**true_value_name**:字串。 當值位於「開啟」位置時，要在登錄頁面編輯器中顯示的顯示名稱。 若未提供，則為「ON」。

基本範例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

所有屬性的範例：

此範例顯示一個常見的使用案例，其中布林變數會將css顯示屬性的值設為&quot;block&quot;或&quot;none&quot;，以透過CSS依ID顯示/隱藏元素，借此控制css元素的可見性。 登錄頁面編輯器將使用顯示名稱「顯示/隱藏」，而非「關閉/開啟」。

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>程式Token(my.token)也可以在引導式或自由格式登錄頁面中的任何地方使用。
