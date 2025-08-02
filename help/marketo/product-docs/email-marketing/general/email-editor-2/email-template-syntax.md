---
unique-page-id: 11371040
description: 電子郵件範本語法 — Marketo檔案 — 產品檔案
title: 電子郵件範本語法
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 2%

---

# 電子郵件範本語法 {#email-template-syntax}

在Marketo的全新電子郵件2.0體驗中，電子郵件範本是由元素、變數、模組或容器的任何組合所組成。 每個變數都是透過將Marketo專屬的語法新增至您的HTML來定義。 電子郵件編輯器2.0支援舊的(v1.0)電子郵件範本；但是，這些範本不會包含新編輯器的所有功能。

Marketo電子郵件語法只適用於範本和個別電子郵件；如果內嵌在代碼片段或RTF權杖中，則&#x200B;**無法**&#x200B;運作。

>[!NOTE]
>
>Marketo支援未設定為協助CSS/HTML。 如果您不熟悉CSS/HTML，請洽詢開發人員。

>[!CAUTION]
>
>包含Marketo語法的類別值（即mktoModule、mktoContainer、mktoText）會區分大小寫。 自訂屬性名稱（即mktoimgwidth、mktoname）則否。

## 元素 {#elements}

元素是您在電子郵件範本中定義為可編輯的內容區域。 元素的編輯體驗與其型別不同，且提供簡單的內容處理方式。 電子郵件範本中可包含的可能元素包括：

* RTF文字
* 影像
* 程式碼片段
* 影片

## RTF文字 {#rich-text}

如果您將區域定義為RTF格式，使用者將可以使用Marketo的RTF編輯器[編輯其內容](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)。 在電子郵件範本內定義RTF元素有兩個方法： mktEditable和mktoText。 請記住，RTF元素永遠都可以在電子郵件編輯器中轉換為程式碼片段。

### 選項1 - mktEditable {#option-mkteditable}

由於Email Editor 2.0可回溯相容，因此某些舊版電子郵件範本可能會藉由在任何HTML元素上新增class=&quot;mktEditable&quot;來指定RTF文字元素。 這仍受支援，且元素的ID將是電子郵件編輯器內作為顯示名稱使用的。

必要屬性

* **類別**： &quot;mktEditable&quot;。
* **id**：識別碼字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。

選擇性屬性

* **mktoName** ：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

預設值

HTML元素（如果提供）中具有class=&quot;mktEditable&quot;的內容將用作RTF元素的預設值。

範例：

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### 選項2 - mktoText {#option-mktotext}

建議您使用class=&quot;mktoText&quot;語法來指定RTF元素。 這可確保元素始終有正確的顯示名稱。

必要屬性

* **類別**： &quot;mktoText&quot;
* **id**：識別碼字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName** ：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

預設值

HTML元素（如果提供）中具有class=&quot;mktoText&quot;的內容將用作RTF元素的預設值。

範例：

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## 影像 {#images}

您有兩個選項可定義可編輯的影像元素。 您可以使用`<div>`或`<img>`標籤，指定將`<img>`插入其中的容器。 如果您打算讓使用者直接挑選會傳回影像URL （而非DOM）的影像，請參閱下節中的「影像變數」。 下列兩個選項將會插入HTML `<img>`元素。

### 選項1 — 使用`<div>` {#option-use-a-div}

必要屬性

* **類別：** &quot;mktoImg&quot;。
* **識別碼：**&#x200B;識別碼字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName ：**&#x200B;字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **mktoImgClass：**&#x200B;字串。 此處值將新增至div內`<img>`元素的類別屬性。
* **mktoImgSrc：**&#x200B;要做為這個div中影像的預設值。 如果省略，則會使用預留位置。
* **mktoImgLink：**&#x200B;表示`<img>`應該用帶有此目的地URL的`<a>`標籤括住。 使用者可在電子郵件編輯器中變更此設定。
* **mktoImgLinkTarget：**&#x200B;表示mktoImgLink屬性中的`<a>`標籤應使用此目標。 如果未使用mktoImgLink，則沒有任何效果。
* **mktoImgWidth：**&#x200B;用作括住的`<img>`上的寬度。
* **mktoImgHeight：**&#x200B;用作所括住`<img>`的高度。
* **mktoLockImgSize：**&#x200B;用於解鎖`<img>`專案的高度與寬度屬性，讓一般使用者可以修改（若省略，預設值為true）。
* **mktoLockImgStyle：**&#x200B;用於鎖定`<img>`專案的樣式屬性（預設為false）。

預設值（選擇性）

**`<img>`**：要做為將放置影像的`<img>`元素。 如果要將內嵌樣式新增至影像，則此功能非常有用。 請記得加入周圍`<a> </a>`的標籤，這樣如果使用者新增連結，您的樣式就不會被移除！

範例：

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### 選項2 — 使用\&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>此選項不允許一般使用者將連結新增至其影像。 如果這對您的範本很重要，請使用選項1。

必要屬性

* **類別：** &quot;mktoImg&quot;。
* **識別碼：**&#x200B;識別碼字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName：**&#x200B;字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。  預設值（選擇性）
* **src：**&#x200B;做為影像的預設值。 如果省略，則會使用預留位置。
* **mktoLockImgSize：**&#x200B;用於解鎖`<img>`專案的高度與寬度屬性，讓一般使用者可以修改（若省略，預設值為true）。
* **mktoLockImgStyle：**&#x200B;用於鎖定`<img>`專案的樣式屬性（預設為false）。

範例：
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## 程式碼片段 {#snippets}

如果您將區域定義為程式碼片段，一般使用者將可以選擇他們要插入此區域的已核准[程式碼片段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)。 雖然RTF元素可以從電子郵件編輯器內轉換為代碼片段，但當您明確將區域定義為代碼片段時，無法將它轉換為RTF。 您可以使用`<div>`搭配class=&quot;mktoSnippet&quot;來指定代碼片段區域

必要屬性

* **識別碼：**&#x200B;識別碼字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName：**&#x200B;字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

預設值（選擇性）

**mktoDefaultSnippetId**：預設應顯示的Marketo程式碼片段數值ID （只有在具有該ID的程式碼片段存在且在該工作區中核準時，才能運作）。

範例：

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## 影片 {#video}

如果您將地區定義為視訊，一般使用者可插入將在電子郵件中顯示為縮圖影像（具有「播放」按鈕）的YouTube或Vimeo URL。 您可以使用`<div>`並搭配使用class=&quot;mktoVideo&quot;來指定視訊區域

必要屬性

* **識別碼：**&#x200B;識別碼字串。 僅包含字母、數字、破折號「 — 」和底線「_」。 不允許空格。 必須是唯一的。
* **mktoName：**&#x200B;字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **mktoImgClass：**&#x200B;字串。 此處的值將新增至div內視訊縮圖`<img>`的class屬性。

範例：

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## 變數 {#variables}

變數就像代號。 您先使用`<head>`標籤在電子郵件範本的`<meta>`區段中定義這些標籤，然後在整個範本中視需要多次使用這些標籤。 由於已在範本中定義，一般使用者將能根據其規則修改其值。 請注意，您可以在範圍中將變數定義為本機或全域。 如果您在「模組」中使用變數（請參閱下文），而一般使用者重複該模組，則區域變數會有獨立的值，而全域變數將套用至兩個模組。

## 字串 {#string}

如果您將變數指定為String，一般使用者就可以在電子郵件編輯器的文字方塊中輸入文字。 您指定字串變數，使用`<meta>`搭配class=&quot;mktoString&quot;

必要屬性

* **id：**&#x200B;如何在電子郵件範本中參考變數。
* **mktoName：**&#x200B;字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **allowHTML：**&#x200B;布林值。 控制變數的值是否為HTML逸出。 如果省略，則預設為False。
* **預設**：字串的預設值。 若省略，則為空白。
* **mktoModuleScope**：布林值。 控制變數在模組中使用時為本機(true)或全域(false)。 如果省略，則預設為False。

宣告範例：

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

使用範例：

`${textHeader}`

## 清單 {#list}

如果您將變數指定為「清單」，一般使用者將能夠選取您在電子郵件編輯器中定義的一組值。 您指定清單變數，使用`<meta>`搭配class=&quot;mktoList&quot;

必要屬性

* **id**：如何在電子郵件範本中參考變數。
* **mktoName：**&#x200B;字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。
* **值：**&#x200B;逗號分隔值清單。 必須至少有一個字串。

選擇性屬性

* **預設值：**&#x200B;選取下拉式清單的預設值。 如果省略，則會使用「values」屬性的第一個值。
* **mktoModuleScope**：布林值。 控制變數在模組中使用時為本機(true)或全域(false)。 如果省略，則預設為False。

宣告範例：

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

使用範例：

`${textFontFamily}`

## 數字 {#number}

如果您指定變數作為數字，一般使用者可在電子郵件編輯器中輸入數字。 您指定使用`<meta>`搭配class=&quot;mktoNumber&quot;的數字變數

必要屬性

* **id**：如何在電子郵件範本中參考變數。
* **mktoName**：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。
* **預設值：**&#x200B;變數的預設數值。

選擇性屬性

* **分鐘：**&#x200B;分鐘接受的值。
* **最大值：**&#x200B;接受的最大值。
* **單位：**&#x200B;當顯示在電子郵件編輯器以及產生的程式碼中時，附加至數字值（例如：px、pt、em等）的單位。
* **步驟：**&#x200B;數字變數應該增加/減少多少單位（0.1、1、10等）。 如果省略，預設值為1。
* **mktoModuleScope**：布林值。 控制變數在模組中使用時為本機(true)或全域(false)。 如果省略，則預設為False。

宣告範例：

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> `

使用範例：

`${textFontSize}`

## 顏色 {#color}

如果您將變數指定為「顏色」，一般使用者將可以輸入十六進位顏色值，或從電子郵件編輯器中的檢色器選擇顏色。 您使用`<meta>`搭配class=&quot;mktoColor&quot;指定色彩變數

必要屬性

* **id**：如何在電子郵件範本中參考變數。
* **mktoName**：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **預設值：**&#x200B;顏色的預設值。 6位數的十六進位色彩代碼。 例如： #ffffff。
* **mktoModuleScope**：布林值。 控制變數在模組中使用時為本機(true)或全域(false)。 如果省略，則預設為False。

宣告範例：

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

使用範例：

`${textColor}`

## 布林值 {#boolean}

如果您將變數指定為布林值，一般使用者就可以在電子郵件編輯器中切換開啟/關閉選項。 您使用`<meta>`搭配class=&quot;mktoBoolean&quot;指定布林值變數

必要屬性

* **id**：如何在電子郵件範本中參考變數。
* **mktoName**：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **預設值：**&#x200B;布林值，決定切換開關的預設狀態。 若省略，則為False。
* **false_value：**&#x200B;當切換開關處於關閉位置時要插入的值。 若省略，則為False。
* **true_value：**&#x200B;當切換處於「開啟」位置時要插入的值。 若省略，則為True。
* **false_value_name：** UI顯示在「關閉」位置的切換中。 若省略，則為False。
* **true_value_name：** UI顯示在「開啟」位置的切換中。 若省略，則為True。
* **mktoModuleScope**：布林值。 控制變數在模組中使用時為本機(true)或全域(false)。 如果省略，則預設為False。

宣告範例：

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

使用範例：

`${showFooter}`

## HTML區塊 {#html-block}

如果您將變數指定為HTML區塊，一般使用者將可從電子郵件編輯器輸入逐字HTML。 您使用`<meta>`搭配class=&quot;mktoHTML&quot;來指定HTML區塊變數

必要屬性

* **id**：如何在電子郵件範本中參考變數。
* **mktoName**：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **預設：** HTML編碼值做為區塊的預設內容。
* **mktoModuleScope**：布林值。 控制變數在模組中使用時為本機(true)或全域(false)。 如果省略，則預設為False。

宣告範例：

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

使用範例：

`${trackingPixel}`

## 影像變數 {#image-variable}

如果您將變數指定為影像，一般使用者將可從電子郵件編輯器中的影像選擇器中選擇影像。 選取的影像URL將是變數的值。 您使用`<meta>`搭配class=&quot;mktoImg&quot;指定影像變數

必要屬性

* **id**：如何在電子郵件範本中參考變數。
* **mktoName**：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **預設值：**&#x200B;元素的預設影像URL。
* **mktoModuleScope**：布林值。 控制變數在模組中使用時為本機(true)或全域(false)。 如果省略，則預設為False。

宣告範例：

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

使用範例：

`${heroBackgroundImage}`

## 模組 {#modules}

模組是在範本層級定義的範本化區段，將會顯示供一般使用者插入其電子郵件。 由於您已預先建立這些模組，因此可確保這些模組能正常地與您的其他電子郵件內容互動（以完全回應式方式）。 您只能將模組放入容器中。

>[!IMPORTANT]
>
>從包含已定義模組元件的電子郵件範本產生電子郵件時，對範本模組所做的任何變更都將&#x200B;**不**&#x200B;推送至該電子郵件。

**針對型別`<table>`、`<tbody>`、`<thead>`或`<tfoot>`的容器：**

使用`<tr>`搭配class=&quot;mktoModule&quot;指定

**針對型別`<td>`的容器：**

使用`<table>`搭配class=&quot;mktoModule&quot;指定

必要屬性

* **id**：如何在電子郵件範本中參考此模組。
* **mktoName**：字串。 這是將顯示在電子郵件編輯器2.0中的顯示名稱。最佳實務是使用描述性名稱。

選擇性屬性

* **mktoActive：**&#x200B;判斷此模組是否出現在電子郵件編輯器的模組清單中。 預設為true。 若為false，一般使用者無法將該模組新增至電子郵件。
* **mktoAddByDefault：**&#x200B;決定此模組是否會在建立時使用這個範本的新電子郵件的畫布中。 預設值為true （如果mktoActive為false，則會忽略此值）。

>[!NOTE]
>
>包含Marketo語法的類別值（即mktoModule、mktoContainer、mktoText）會區分大小寫。 自訂屬性名稱（即mktoimgwidth、mktoname）則否。

## 容器 {#containers}

容器內含模組，並定義模組可放置的位置。 當使用者重新排序並將模組插入電子郵件時，容器會控制他們可能前往的位置。

使用&#x200B;**、`<table>`、`<tbody>`、`<thead>`或具有class=&quot;mktoContainer&quot;`<tfoot>`的`<td>`指定**

必要屬性

**id**：如何在電子郵件範本中參考此模組。

>[!CAUTION]
>
>容器只能包含模組 — 如果有其他專案存在，則會將容器視為無效！ 每個範本只允許一個容器。
