---
unique-page-id: 11371040
description: 電子郵件範本語法——行銷人員檔案——產品檔案
title: 電子郵件範本語法
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '2395'
ht-degree: 0%

---


# 電子郵件範本語法{#email-template-syntax}

在Marketto的全新Email 2.0體驗中，電子郵件範本是由元素、變數、模組或容器的任意組合所組成。 每個都是透過新增Marketto特定語法至HTML來定義。 舊版(v1.0)電子郵件範本在Email Editor 2.0中受到支援；但是，它們不會包含所有新編輯的功能。

Marketo電子郵件語法僅適用於範本和個別電子郵件；如果內嵌在程式碼片段或Rich Text Token中，**not**&#x200B;便能運作。

>[!NOTE]
>
>Marketo支援未設定為協助CSS/HTML。 如果您不熟悉CSS/HTML，請洽詢您的開發人員。

>[!CAUTION]
>
>包含Marketo語法的類別值（例如mktoModule、mktoContainer、mktoText）會區分大小寫。 自訂屬性名稱（例如mktoimgwidth、mktoname）則否。

## 元素{#elements}

元素是您在電子郵件範本中定義為可編輯的內容區域。 元素的編輯體驗是其類型獨一無二的，並提供處理內容的簡單方式。 電子郵件範本中可能包含的元素包括：

* Rich Text
* 影像
* 程式碼片段
* 影片

## 富格文本{#rich-text}

如果您將地區定義為Rich Text，使用者將可使用Marketo的Rich Text Editor](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)編輯其內容。 [在電子郵件範本中定義Rich Text元素有兩種方式：mktEditable和mktoText。 請記住，「豐富文字」元素永遠可以從電子郵件編輯器中轉換為程式碼片段。

### 選項1 - mktEditable {#option-mkteditable}

由於Email Editor 2.0與後向相容，因此某些舊式電子郵件範本可能會在任何HTML元素上新增class=&quot;mktEditable&quot;來指定豐富型文字元素。 這仍受支援，而元素的ID則是電子郵件編輯器中用來做為顯示名稱的項目。

必要屬性

* **類別**:&quot;mktEditable&quot;。
* **id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。

可選屬性

* **mktoName** :字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

預設值

HTML元素內含class=&quot;mktEditable&quot;的內容（如果提供）將用作Rich Text元素的預設值。

範例：

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### 選項2 - mktoText {#option-mktotext}

建議使用class=&quot;mktoText&quot;語法來指定Rich Text元素。 這可確保元素始終有正確的顯示名稱。

必要屬性

* **類別**:&quot;mktoText&quot;
* **id**:ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。
* **mktoName** :字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

預設值

HTML元素內含class=&quot;mktoText&quot;的內容（如果提供）將用作Rich Text元素的預設值。

範例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 影像{#images}

您有兩個選項可用來定義可編輯的影像元素。 您可以使用`<div>`（指定`<img>`將插入的容器）或`<img>`標籤。 如果您只想讓使用者選擇會傳回影像URL的影像（與DOM相反），請參閱下方章節中的「影像變數」。 以下兩個選項將插入HTML `<img>`元素。

### 選項1 —— 使用`<div>` {#option-use-a-div}

必要屬性

* **class:** &quot;mktoImg&quot;。
* **id:** ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。
* **mktoName:** String。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **mktoImgClass:** String。此處的值將添加到div內`<img>`元素的class屬性中。
* **mktoImgSrc:** To be used as the default value for the image that is placed in this div.若省略此項，則會使用預留位置。
* **mktoImgLink：指** 出應 `<img>` 該由含有此目 `<a>` 標URL的標籤所包圍。使用者可在電子郵件編輯器中變更此項。
* **mktoImgLinkTarget：指** 出mktoImgLink屬 `<a>` 性中的標籤應使用此目標。如果未使用mktoImgLink，則無效。
* **mktoImgWidth:** 用作封閉的寬度 `<img>`。
* **mktoImgHeight:** 用作封閉高度 `<img>`。
* **mktoLockImgSize：用** 於解除鎖 `<img>` 定元素的height和width屬性，以便使用者修改（若省略，預設為true）。
* **mktoLockImgStyle:** 用於鎖 `<img>` 定元素的style屬性（預設為false）。

預設值（選用）

**`<img>`**:要用作將 `<img>` 放置影像的元素。當您要新增內嵌樣式至影像時，此功能很實用。 請記住要包含周圍的`<a> </a>`標籤，因此，如果使用者新增連結，您的樣式就不會被移除！

範例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### 選項2 —— 使用\&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>此選項不允許使用者新增影像的連結。 如果這對您的範本很重要，請使用選項1。

必要屬性

* **class:** &quot;mktoImg&quot;。
* **id:** ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。
* **mktoName：字** 串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。  預設值（選用）
* **src:** 將用作影像的預設值。若省略此項，則會使用預留位置。
* **mktoLockImgSize：用** 於解除鎖 `<img>` 定元素的height和width屬性，以便使用者修改（若省略，預設為true）。
* **mktoLockImgStyle:** 用於鎖 `<img>` 定元素的style屬性（預設為false）。

範例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## 代碼片段{#snippets}

如果您將地區定義為「程式碼片段」，一般使用者將可選擇要插入此地區的已核准[程式碼片段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)。 雖然Rich Text元素可從電子郵件編輯器轉換為Snippets，但當您將地區明確定義為Snippet時，它無法轉換為Rich Text。 您可以使用`<div>`搭配class=&quot;mktoSnippet&quot;來指定「程式碼片段」區域

必要屬性

* **id:** ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。
* **mktoName：字** 串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

預設值（選用）

**mktoDefaultSnippetId**:預設應出現的Marketo程式碼片段數值ID（僅當具有該ID的程式碼片段存在且已在該工作區中核準時，才能運作）。

範例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## 視頻{#video}

如果您將地區定義為「影片」，使用者將可以插入YouTube或Vimeo URL，該URL會顯示為電子郵件中的縮圖影像（使用「播放」按鈕）。 您可以使用`<div>`搭配class=&quot;mktoVideo&quot;來指定視訊區域

必要屬性

* **id:** ID字串。僅包含字母、數字、破折號&quot;-&quot;和底線&quot;_&quot;。 不允許空格。 必須是唯一的。
* **mktoName：字** 串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **mktoImgClass:** String。此處的值將添加到div內視頻縮略圖`<img>`的class屬性中。

範例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 變數{#variables}

變數就像Token。 您首先使用`<meta>`標籤在電子郵件範本的`<head>`區段中定義這些標籤，然後在整個範本中使用這些標籤，視需要多次。 由於這些值是在範本中定義的，因此使用者將可根據其規則修改其值。 請注意，您可以在範圍中將變數定義為局部或全域。 如果您在「模組」中使用變數（請參閱下面），而使用者複製該模組，則本機變數將具有獨立值，而全域變數將套用至這兩個模組。

## 字串{#string}

如果您指定變數為「字串」，一般使用者就可以在電子郵件編輯器的文字方塊中輸入文字。 您使用`<meta>`搭配class=&quot;mktoString&quot;指定字串變數

必要屬性

* **id：您** 在電子郵件範本中參考變數的方式。
* **mktoName：字** 串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **allowHTML:** Boolean。控制變數的值是否為HTML逸出。 若省略，則預設為False。
* **預設**:字串的預設值。如果省略，則為空白。
* **mktoModuleScope**:布林。控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

範例用法：

`<pre data-theme="Confluence">${textHeader}</pre>`

## 清單{#list}

如果您指定變數為「清單」，使用者將可從您在電子郵件編輯器中定義的一組值中挑選。 您使用`<meta>`搭配class=&quot;mktoList&quot;指定清單變數

必要屬性

* **id**:您在電子郵件範本中參考變數的方式。
* **mktoName：字** 串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。
* **值：以逗** 號分隔的值清單。至少必須有一個字串。

可選屬性

* **default：選** 取下拉式清單的預設值。若省略，則會使用「值」屬性的第一個值。
* **mktoModuleScope**:布林。控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

範例用法：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 編號{#number}

如果您指定變數為「編號」，一般使用者就可以在電子郵件編輯器中輸入數字。 您使用`<meta>`搭配class=&quot;mktoNumber&quot;指定Number變數

必要屬性

* **id**:您在電子郵件範本中參考變數的方式。
* **mktoName**:字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。
* **default：變** 數的預設數值。

可選屬性

* **min:** Min accepted value.
* **max:** Max accepted value.
* **單位：** 要附加到數字值的單位(例如：px、pt、em等)顯示在「電子郵件編輯器」中，以及產生的代碼中。
* **步驟：** 數字變數應增加／減少多少單位（0.1、1、10等）。若省略，預設為1。
* **mktoModuleScope**:布林。控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

範例用法：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## 顏色{#color}

如果您指定變數為「顏色」，使用者將可輸入十六進位顏色值，或從電子郵件編輯器的檢色器選擇顏色。 您使用`<meta>`搭配class=&quot;mktoColor&quot;來指定顏色變數

必要屬性

* **id**:您在電子郵件範本中參考變數的方式。
* **mktoName**:字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **default:** 顏色的預設值。6位十六進位色碼。 例如：#ffffff.
* **mktoModuleScope**:布林。控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

範例用法：

`<pre data-theme="Confluence">${textColor}</pre>`

## 布林{#boolean}

如果您指定變數為布林值，一般使用者將可在電子郵件編輯器中開啟／關閉選項。 您使用`<meta>`搭配class=&quot;mktoBoolean&quot;指定布林變數

必要屬性

* **id**:您在電子郵件範本中參考變數的方式。
* **mktoName**:字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **default:** 確定切換開關的預設狀態的布爾值。若省略，則為False。
* **false_value：切** 換為OFF位置時要插入的值。若省略，則為False。
* **true_value：切** 換為ON位置時要插入的值。如果省略，則為true。
* **false_value_name:** UI顯示在切換為OFF位置時。若省略，則為False。
* **true_value_name:** UI顯示在ON位置切換時。如果省略，則為true。
* **mktoModuleScope**:布林。控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

範例用法：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML區塊{#html-block}

如果您將變數指定為HTML區塊，一般使用者將可從電子郵件編輯器中輸入逐字發文HTML。 您使用`<meta>`搭配class=&quot;mktoHTML&quot;指定HTML區塊變數

必要屬性

* **id**:您在電子郵件範本中參考變數的方式。
* **mktoName**:字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **default:** HTML編碼值，用作區塊的預設內容。
* **mktoModuleScope**:布林。控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

範例用法：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 影像變數{#image-variable}

如果您指定變數為「影像」，一般使用者就可以在電子郵件編輯器中從影像選擇器中選擇影像。 選取的影像URL將是變數的值。 您使用`<meta>`搭配class=&quot;mktoImg&quot;指定影像變數

必要屬性

* **id**:您在電子郵件範本中參考變數的方式。
* **mktoName**:字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **default：元** 素的預設影像URL。
* **mktoModuleScope**:布林。控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

範例用法：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## 模組{#modules}

模組是在範本層級定義的範本區段，將顯示給使用者以插入其電子郵件。 由於您已預先建立這些模組，因此您可以確保這些模組能與您其餘的電子郵件內容正常互動（完全自適應）。 您只能將模組放入容器中。

**對於類型、 `<table>`、 `<tbody>` `<thead>`或的容器 `<tfoot>`:**

使用`<tr>`搭配class=&quot;mktoModule&quot;指定

**對於類型的容器 `<td>`:**

使用`<table>`搭配class=&quot;mktoModule&quot;指定

必要屬性

* **id**:您在電子郵件範本中參考模組的方式。
* **mktoName**:字串。這是將顯示在「電子郵件編輯器2.0」中的顯示名稱。最佳實務是使用描述性名稱。

可選屬性

* **mktoActive：決** 定此模組是否顯示在電子郵件編輯器中的模組清單中。預設為true。 如果為false，則一般使用者無法將模組新增至電子郵件。
* **mktoAddByDefault：決** 定此模組是否位於建立時使用此範本之新電子郵件的畫布中。預設為true（如果mktoActive為false，則會忽略此值）。

>[!NOTE]
>
>包含Marketo語法的類別值（例如mktoModule、mktoContainer、mktoText）會區分大小寫。 自訂屬性名稱（例如mktoimgwidth、mktoname）則否。

## 容器{#containers}

容器保存模組並定義可放置模組的位置。 當使用者重新排序並將模組插入電子郵件時，容器會控制他們可前往的位置。

**使用class= `<table>`&quot;mktoContainer&quot; `<tbody>`指定 `<thead>`,  `<tfoot>` or with  `<td>` class=&quot;mktoContainer&quot;**

必要屬性

**id**:您在電子郵件範本中參考模組的方式。

>[!CAUTION]
>
>容器只能包含模組——如果有其他項目存在，容器即視為無效！ 每個範本僅允許一個容器。
