---
unique-page-id: 11371040
description: 電子郵件範本語法 — Marketo檔案 — 產品檔案
title: 電子郵件範本語法
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# 電子郵件範本語法 {#email-template-syntax}

在Marketo的新Email 2.0體驗中，電子郵件範本是由元素、變數、模組或容器的任何組合所組成。 每個都是透過新增Marketo專用語法至HTML來定義。 電子郵件編輯器2.0支援舊版(v1.0)電子郵件範本；但是，它們不會包含新編輯器的所有功能。

Marketo電子郵件語法僅適用於範本和個別電子郵件；它有 **not** 如果內嵌在程式碼片段或RTF代號中，則可運作。

>[!NOTE]
>
>Marketo支援未設定來協助處理CSS/HTML。 如果您不熟悉CSS/HTML，請洽詢您的開發人員。

>[!CAUTION]
>
>包含Marketo語法的類別值（例如mktoModule、mktoContainer、mktoText）會區分大小寫。 自訂屬性名稱（即mktoimgwidth、mktoname）則否。

## 元素 {#elements}

元素是您在電子郵件範本中定義為可編輯的內容區域。 元素的編輯體驗對其類型是唯一的，並提供處理內容的簡單方式。 電子郵件範本中可能包含的元素包括：

* RTF
* 影像
* 程式碼片段
* 影片

## RTF {#rich-text}

如果您將地區定義為RTF，使用者將能夠編輯其內容 [使用Marketo的RTF編輯器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). 有兩種方式可在電子郵件範本內定義RTF元素：mktEditable和mktoText。 請記住，RTF元素一律可從電子郵件編輯器轉換為程式碼片段。

### 選項1 - mktEditable {#option-mkteditable}

由於電子郵件編輯器2.0與後向相容，因此某些舊電子郵件範本可能會在任何HTML元素上新增class=&quot;mktEditable&quot;，以指定RTF元素。 仍支援此功能，而元素的ID將用作電子郵件編輯器中的顯示名稱。

必要屬性

* **類**:&quot;mktEditable&quot;。
* **id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。

可選屬性

* **mktoName** :字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

預設值

HTML元素內（若有提供）包含class=&quot;mktEditable&quot;的內容將用作Rtf元素的預設值。

範例：

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### 選項2 - mktoText {#option-mktotext}

建議使用class=&quot;mktoText&quot;語法來指定RTF元素。 這可確保元素的顯示名稱一律正確。

必要屬性

* **類**:&quot;mktoText&quot;
* **id**:ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName** :字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

預設值

HTML元素內（若有提供）包含class=&quot;mktoText&quot;的內容將用作Rtf元素的預設值。

範例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 影像 {#images}

定義可編輯的影像元素有兩個選項。 您可以使用 `<div>`，它指定一個容器， `<img>` 將插入，或 `<img>` 標籤。 如果您只想讓使用者挑選會傳回影像URL的影像（而非DOM），請參閱下節中的「影像變數」。 以下兩個選項將插入HTML `<img>` 元素。

### 選項1 — 使用 `<div>` {#option-use-a-div}

必要屬性

* **類別：** &quot;mktoImg&quot;。
* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName :** 字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **mktoImgClass:** 字串。 此處的值將新增至的類別屬性 `<img>` div內的元素。
* **mktoImgSrc:** 作為放置在此div內之影像的預設值。 如果省略此項，則會使用預留位置。
* **mktoImgLink:** 指出 `<img>` 應由 `<a>` 標籤。 使用者可在電子郵件編輯器中變更此項目。
* **mktoImgLinkTarget:** 指出 `<a>` mktoImgLink屬性中的標籤應使用此目標。 如果未使用mktoImgLink，則無效。
* **mktoImgWidth:** 用作封閉的 `<img>`.
* **mktoImgHeight:** 用作封閉的 `<img>`.
* **mktoLockImgSize:** 用於解鎖 `<img>` 元素的height和width屬性，讓一般使用者可以修改（若省略，則預設為true）。
* **mktoLockImgStyle:** 用來鎖定 `<img>` 元素的style屬性（預設為false）。

預設值（選用）

**`<img>`**:要作為 `<img>` 元素。 如果您想要將內嵌樣式新增至影像，此功能會相當實用。 請記得包含周圍 `<a> </a>` 標籤，因此若使用者新增連結，您的樣式將不會被移除！

範例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### 選項2 — 使用\&lt;img> {#option-use-an-img}

>[!NOTE]
>
>此選項不允許使用者將連結新增至其影像。 如果這對您的範本很重要，請使用選項1。

必要屬性

* **類別：** &quot;mktoImg&quot;。
* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName:** 字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。  預設值（選用）
* **src:** 作為影像的預設值。 如果省略此項，則會使用預留位置。
* **mktoLockImgSize:** 用於解鎖 `<img>` 元素的height和width屬性，讓一般使用者可以修改（若省略，則預設為true）。
* **mktoLockImgStyle:** 用來鎖定 `<img>` 元素的style屬性（預設為false）。

範例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## 程式碼片段 {#snippets}

如果您將地區定義為程式碼片段，使用者將可以選擇已核准的 [程式碼片段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)他們想在這個區域插入。 雖然RTF元素可從電子郵件編輯器內轉換為程式碼片段，但當您明確將區域定義為程式碼片段時，無法將其轉換為RTF。 您可以使用 `<div>` 與class=&quot;mktoSnippet&quot;

必要屬性

* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName:** 字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

預設值（選用）

**mktoDefaultSnippetId**:預設應顯示的Marketo程式碼片段數值ID（只有在具有該ID的程式碼片段存在且在該工作區中獲核準時才有效）。

範例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## 影片 {#video}

如果您將地區定義為「影片」，使用者將能在電子郵件內插入YouTube或Vimeo URL，這些URL會顯示為縮圖影像（搭配「播放」按鈕）。 您可以使用 `<div>` with class=&quot;mktoVideo&quot;

必要屬性

* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName:** 字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **mktoImgClass:** 字串。 此處的值將新增至視訊縮圖的類別屬性 `<img>` div內。

範例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 變數 {#variables}

變數就像Token。 您會先在 `<head>` 使用 `<meta>` 標籤，然後在整個範本中使用標籤的次數可以滿足您的需求。 因為這些規則是在範本中定義的，所以一般使用者將能根據其規則修改其值。 請注意，您可以在範圍中將變數定義為本機或全域。 如果您在「模組」中使用變數（請參閱下方），且一般使用者複製該模組，則本機變數將有獨立值，而全域變數則會套用至這兩個模組。

## 字串 {#string}

如果您將變數指定為字串，一般使用者將能在電子郵件編輯器的文字方塊中輸入文字。 您可使用 `<meta>` with class=&quot;mktoString&quot;

必要屬性

* **id:** 如何參考電子郵件範本中的變數。
* **mktoName:** 字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **allowHTML:** 布林值。 控制變數的值是否HTML逸出。 若省略，則預設為False。
* **預設**:字串的預設值。 若省略，則留空。
* **mktoModuleScope**:布林值。 控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

使用範例：

`<pre data-theme="Confluence">${textHeader}</pre>`

## 清單 {#list}

如果您將變數指定為「清單」，使用者將能從您在電子郵件編輯器中定義的一組值中選取。 您可使用 `<meta>` with class=&quot;mktoList&quot;

必要屬性

* **id**:如何參考電子郵件範本中的變數。
* **mktoName:** 字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。
* **值：** 值清單（以逗號分隔）。 必須至少包含一個字串。

可選屬性

* **預設值：** 選取下拉式清單的預設值。 若省略，則會使用「values」屬性中的第一個值。
* **mktoModuleScope**:布林值。 控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

使用範例：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 數字 {#number}

如果您將變數指定為「數字」，使用者將能在電子郵件編輯器中輸入數字。 您可使用 `<meta>` with class=&quot;mktoNumber&quot;

必要屬性

* **id**:如何參考電子郵件範本中的變數。
* **mktoName**:字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。
* **預設值：** 變數的預設數值。

可選屬性

* **最小值：** 最小接受值。
* **最大：** 最大接受值。
* **件數：** 要附加到數字值的件數(例如：px、pt、em等) 顯示在「電子郵件編輯器」中，以及產生的程式碼中時。
* **步驟：** 數字變數應增加/減少的件數（0.1、1、10等）。 若省略，則預設為1。
* **mktoModuleScope**:布林值。 控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

使用範例：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## 顏色 {#color}

如果將變數指定為「顏色」，則最終用戶將能夠輸入十六進位顏色值，或從電子郵件編輯器中的檢色器中選擇一種顏色。 您可使用 `<meta>` with class=&quot;mktoColor&quot;

必要屬性

* **id**:如何參考電子郵件範本中的變數。
* **mktoName**:字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **預設值：** 顏色的預設值。 6位十六進位色碼。 例如：#ffffff。
* **mktoModuleScope**:布林值。 控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

使用範例：

`<pre data-theme="Confluence">${textColor}</pre>`

## 布林值 {#boolean}

如果您將變數指定為布林值，一般使用者將能在電子郵件編輯器中開啟/關閉選項。 您可使用 `<meta>` with class=&quot;mktoBoolean&quot;

必要屬性

* **id**:如何參考電子郵件範本中的變數。
* **mktoName**:字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **預設值：** 布爾值確定切換開關的預設狀態。 若省略，則為False。
* **false_value:** 切換為「關閉」位置時要插入的值。 若省略，則為False。
* **true_value:** 切換處於「開啟」位置時要插入的值。 若省略，則為true。
* **false_value_name:** 當處於「關閉」位置時，會在切換開關中顯示UI。 若省略，則為False。
* **true_value_name:** 當處於「開啟」位置時，切換開關中顯示的UI。 若省略，則為true。
* **mktoModuleScope**:布林值。 控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

使用範例：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML區塊 {#html-block}

如果您將變數指定為HTML區塊，一般使用者將能從電子郵件編輯器中輸入逐字HTML。 您可以使用 `<meta>` with class=&quot;mktoHTML&quot;

必要屬性

* **id**:如何參考電子郵件範本中的變數。
* **mktoName**:字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **預設值：** HTML編碼值，作為區塊的預設內容。
* **mktoModuleScope**:布林值。 控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

使用範例：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 影像變數 {#image-variable}

如果您將變數指定為「影像」，一般使用者將能從電子郵件編輯器中的影像選擇器中選擇影像。 選取的影像URL會是變數的值。 您可使用 `<meta>` with class=&quot;mktoImg&quot;

必要屬性

* **id**:如何參考電子郵件範本中的變數。
* **mktoName**:字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **預設值：** 元素的預設影像URL。
* **mktoModuleScope**:布林值。 控制在模組中使用變數時，變數是本機(true)還是全域(false)。 若省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

使用範例：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## 模組 {#modules}

模組是在範本層級定義的範本區段，會顯示給使用者以插入至其電子郵件。 因為您已預先建置這些模組，因此您可以確保這些模組能正常地與您其餘的電子郵件內容互動（以完全回應的方式）。 您只能將模組放入容器中。

>[!IMPORTANT]
>
>從包含已定義模組元件的電子郵件範本產生電子郵件時，對範本模組所做的任何變更都會 **not** 被推送至上述電子郵件。

**對於類型的容器 `<table>`, `<tbody>`, `<thead>`，或 `<tfoot>`:**

使用 `<tr>` with class=&quot;mktoModule&quot;

**對於類型的容器 `<td>`:**

使用 `<table>` with class=&quot;mktoModule&quot;

必要屬性

* **id**:如何在電子郵件範本中參考模組。
* **mktoName**:字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳作法是使用描述性名稱。

可選屬性

* **mktoActive:** 判斷此模組是否出現在電子郵件編輯器中的模組清單中。 預設為true。 若為false，一般使用者無法將模組新增至電子郵件。
* **mktoAddByDefault:** 決定建立時此模組是否位於使用此範本的新電子郵件的畫布中。 預設為true（如果mktoActive為false，則會忽略此值）。

>[!NOTE]
>
>包含Marketo語法的類別值（例如mktoModule、mktoContainer、mktoText）會區分大小寫。 自訂屬性名稱（即mktoimgwidth、mktoname）則否。

## 容器 {#containers}

容器保存模組並定義可放置的位置。 當使用者重新排序模組並在其電子郵件中插入模組時，容器會控制他們可能前往的位置。

**使用 `<table>`, `<tbody>`, `<thead>`, `<tfoot>` 或 `<td>` with class=&quot;mktoContainer&quot;**

必要屬性

**id**:如何在電子郵件範本中參考模組。

>[!CAUTION]
>
>容器只能包含模組 — 如果有其他項目存在，則容器會視為無效！ 每個範本僅允許一個容器。
