---
unique-page-id: 7515401
description: 建立引導式著陸頁面範本——行銷檔案——產品檔案
title: 建立引導式著陸頁面範本
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# 建立引導式著陸頁面範本{#create-a-guided-landing-page-template}

>[!NOTE]
>
>厭倦讀書了？ [使用逐步指](https://youtu.be/3O7e4GdZKsM) 示觀看這個酷炫的影片。

引導式著陸頁面範本有特殊語法。 使用此語法來指定可自訂的內容，以及內容最終會顯示在從範本建立的每個著陸頁面上的位置。 只有您指定為可編輯的區域或變數才可在「引導」著陸頁面編輯器中自訂。

>[!TIP]
>
>使用良好的命名慣例，您的行銷團隊就會愛上您。

有兩種方式可宣告您頁面上的內容應該是可編輯的：

* 將物件宣告為「元素」。 著陸頁面製作程式可將影像、文字或Marketo資產新增至這些指定的地區。
* 將字串宣告為「變數」。 著陸頁面建立程式將可從true/false槓桿將變數取代為字串、顏色或布林狀態。

## 可編輯的元素{#editable-elements}

元素的宣告方式為：新增一般DOM元素至範本，然後使用Marketo特定類別名稱來裝飾元素。

## 文字{#text}

如果您將地區定義為Rich Text，使用者將可使用Marketo的Rich Text Editor](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)編輯其內容。[

所需屬性：\
**類別**:&quot;mktoText&quot;\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

可選：\
具有類別mktoText（如果提供）的元素內容將用作可編輯區域的預設值。

範例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

### 影像{#image}

您有兩個選項可用來定義可編輯的影像元素。 您可以使用`<div>`或`<img>`標籤，該標籤指定將影像插入的容器。

## 選項1 —— 使用`<div>` {#option-use-a-div}

所需屬性：

類別：&quot;mktoImg&quot;\
id:ID字串。 僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
mktoName :字串。 這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

可選：\
mktoImgClass:字串。 此處的值將添加到div內`<img>`元素的class屬性中。

範例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## 選項2 —— 使用`<img>` {#option-use-a-img}

所需屬性：\
類別：&quot;mktoImg&quot;\
id:ID字串。 僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
mktoName :字串。 這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

可選：\
src:字串URL。 這將用作影像的預設值。

範例：

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>使用`<img>`版本時，轉譯的HTML將包含`<img>`標籤周圍的已生成div包裝函式。 它會設為類別。」mktoImg.mktoGen」，並將是display:inline-block。

## 表單{#form}

範例：必要屬性：\
**類別**:&quot;mktoForm&quot;\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## 程式碼片段{#snippet}

所需屬性：\
**類別**:&quot;mktoSnippet&quot;\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## 共用按鈕{#share-button}

所需屬性：\
**類別**:&quot;mktoShareButton&quot;\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## 視頻{#video}

>[!NOTE]
>
>在著陸頁面中使用視訊元素時，Marketo僅支援YouTube的視訊。 如果您使用其他服務，建議您使用豐富式文字方塊並貼入視訊的內嵌程式碼。

所需屬性：
**class**:&quot;mktoVideo&quot;
**id**:ID字串。 僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## 民調問答{#poll}

所需屬性：\
**類別**:&quot;mktoPoll&quot;\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## 轉介{#referral}

所需屬性：\
**類別**:&quot;mktoReferral&quot;\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## 抽獎活動{#sweepstakes}

所需屬性：\
**類別**:&quot;mktoSweepstakes&quot;\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

範例：

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## 可編輯的變數{#editable-variables}

所有變數類型都會參照其id屬性值，並包裝在${ }個字元序列中。 這些變數可在檔案中的任何位置使用，但在其他變數宣告內部除外。

範例：

`<pre data-theme="Confluence">${var1}</pre>`

**聲明：**

變數會宣告為範本`<head>`元素內的中繼標籤。 可用的變數有三種類型：字串、顏色和布林值。

## 字串{#string}

所需屬性：\
**類別** :&quot;mktoString&quot;,\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

可選：\
**預設**:屬性的字串值。如果未提供，則為空白。\
**allowHtml**:「true」或「false」。控制值是否列印而未逸出HTML。 如果未設定，預設為「false」。

基本範例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

所有屬性的範例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## 顏色{#color}

所需屬性：\
**類別** :&quot;mktoColor&quot;,\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

可選：\
**預設**:7位HEX字元色彩碼。例如：&quot;#336699&quot;

基本範例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

所有屬性的範例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## 布林{#boolean}

所需屬性：\
**類別** :&quot;mktoBoolean&quot;,\
**id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。\
**mktoName** :字串。這是顯示名稱，將顯示在著陸頁面編輯器中。 最佳實務是使用描述性名稱。

可選：\
**預設**:布林字串。「true」或「false」會控制值是否從ON或OFF位置開始。 若未提供&quot;false&quot;。\
**false_value**:字串。變數處於OFF位置時要插入的值。 若未提供&quot;false&quot;。\
**true_value**:字串。變數處於ON位置時要插入的值。 若未提供&quot;true&quot;，則為&quot;true&quot;。\
**false_value_name**:字串。當值位於OFF位置時，要在著陸頁面編輯器中顯示的顯示名稱。 如果未提供，則為「OFF」。\
**true_value_name**:字串。當值位於ON位置時，要在著陸頁面編輯器中顯示的顯示名稱。 如果未提供「ON」。

基本範例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

所有屬性的範例：

此範例顯示一個常見的使用案例，其中布林變數會將css顯示屬性的值設為&quot;block&quot;或&quot;none&quot;，以使用CSS依ID顯示／隱藏元素，以控制css元素的可見性。 著陸頁面編輯器將使用顯示名稱「顯示／隱藏」，而非「關閉／開啟」。

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>程式Token(my.token)也可在引導式或自由格式登陸頁面中的任何位置使用。
