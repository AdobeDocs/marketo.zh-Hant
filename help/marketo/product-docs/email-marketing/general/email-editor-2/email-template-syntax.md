---
unique-page-id: 11371040
description: 電子郵件範本語法 - Marketo 文件 - 產品文件
title: 電子郵件範本語法
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '2449'
ht-degree: 100%

---

# 電子郵件範本語法 {#email-template-syntax}

在 Marketo 的全新電子郵件 2.0 體驗中，電子郵件範本可由元素、變數、模組或容器的任何組合組成。每個都可透過將 Marketo 特定語法新增至您的 HTML 來加以定義。電子郵件編輯器 2.0 可支援舊版 (v1.0) 電子郵件範本；但是，這些範本卻不包含新編輯器的所有功能。

Marketo 電子郵件語法僅適用於範本和個別電子郵件；如果內嵌在程式碼片段或 RTF 文字權杖中，則&#x200B;**無法**&#x200B;運作。

>[!NOTE]
>
>Marketo 支援未設定為協助 CSS/HTML。如果您不熟悉 CSS/HTML，請詢問開發人員。

>[!CAUTION]
>
>包含 Marketo 語法的類別值 (即 mktoModule、mktoContainer、mktoText) 會區分大小寫。自訂屬性名稱 (即 mktoimgwidth、mktoname) 則不會。

## 元素 {#elements}

元素是您在電子郵件範本中定義為可編輯的內容區域。元素的編輯體驗會依其類型而有所不同，並可提供簡單的方式來處理內容。電子郵件範本中可能包含下列元素：

* RTF 文字
* 影像
* 程式碼片段
* 影片

## RTF 文字 {#rich-text}

如果您將區域定義為 RTF 文字，則使用者即可](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)使用 Marketo 的 RTF 文字編輯器[編輯其內容。在電子郵件範本內定義 RTF 文字元素的方法有兩種：mktEditable 和 mktoText。請謹記，RTF 文字一律可以在電子郵件編輯器中轉換為程式碼片段。

### 選項 1 - mktEditable {#option-mkteditable}

由於電子郵件編輯器 2.0 可向後相容，因此某些舊版電子郵件範本可能會藉由在任何 HTML 元素上新增 class=&quot;mktEditable&quot; 來指定 RTF 文字元素。此功能仍受支援，且元素的識別碼會用於在電子郵件編輯器內作為顯示名稱。

必要屬性

* **class**：&quot;mktEditable&quot;。
* **id**：識別碼字串。僅包含字母、數字、破折號「-」和底線「_」。不允許有任何空格。必須為唯一。

選擇性屬性

* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

預設值

HTML 元素 (如果提供) 中具有 class=&quot;mktEditable&quot; 的內容會用作 RTF 文字元素的預設值。

範例：

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### 選項 2 - mktoText {#option-mktotext}

建議您使用 class=&quot;mktoText&quot; 語法來指定 RTF 文字元素。這可確保元素隨時都有正確的顯示名稱。

必要屬性

* **class**：&quot;mktoText&quot;
* **id**：識別碼字串。僅包含字母、數字、破折號「-」和底線「_」。不允許有任何空格。必須為唯一。
* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

預設值

HTML 元素 (如果提供) 中具有 class=&quot;mktoText&quot; 的內容會用作 RTF 文字元素的預設值。

範例：

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## 影像 {#images}

定義可編輯影像元素有兩個選項。您可以使用 `<div>` (會指定要插入 `<img>` 的容器) 或 `<img>` 標記。如果您打算讓終端使用者直接挑選會傳回影像 URL (而非 DOM) 的影像，請參閱下節中的「影像變數」。下列兩個選項會插入 HTML `<img>` 元素。

### 選項 1 — 使用 `<div>` {#option-use-a-div}

必要屬性

* **class：**&quot;mktoImg&quot;。
* **id：**&#x200B;識別碼字串。僅包含字母、數字、破折號「-」和底線「_」。不允許有任何空格。必須為唯一。
* **mktoName：**&#x200B;字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **mktoImgClass：**&#x200B;字串。這裡的值會新增至 div 內 `<img>` 元素的類別屬性。
* **mktoImgSrc：**&#x200B;將用作在此 div 內部放置之影像的預設值。若省略，則會使用預留位置。
* **mktoImgLink：**&#x200B;表示 `<img>` 應該以包含此目的地 URL 的 `<a>` 標記包圍。使用者可在電子郵件編輯器中變更此設定。
* **mktoImgLinkTarget：**&#x200B;表示 mktoImgLink 屬性中的 `<a>` 標記應該使用此目標。若未同時使用 mktoImgLink，則不會產生任何效果。
* **mktoImgWidth：**&#x200B;用於設定框住的 `<img>` 的寬度。
* **mktoImgHeight：**&#x200B;用於設定框住的 `<img>` 的高度。
* **mktoLockImgSize：**&#x200B;用於解除鎖定 `<img>` 元素的高度與寬度屬性，讓終端使用者可進行修改 (若省略，則預設為 true)。
* **mktoLockImgStyle：**&#x200B;用於鎖定 `<img>` 元素的樣式屬性 (預設為 false)。

預設值 (選用)

**`<img>`**：將用作要放入影像之 `<img>` 元素。如果要將內嵌樣式新增至影像，則此功能非常實用。請記得包括外圍的 `<a> </a>` 標記，這樣如果使用者新增連結，您的樣式即不會遭移除！

範例：

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### 選項 2 — 使用 \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>此選項不允許終端使用者將連結新增至其影像。如果這對您的範本很重要，請使用選項 1。

必要屬性

* **class：**&quot;mktoImg&quot;。
* **id：**&#x200B;識別碼字串。僅包含字母、數字、破折號「-」和底線「_」。不允許有任何空格。必須為唯一。
* **mktoName：**&#x200B;字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。預設值 (選用)
* **src：**&#x200B;將用作影像的預設值。若省略，則會使用預留位置。
* **mktoLockImgSize：**&#x200B;用於解除鎖定 `<img>` 元素的高度與寬度屬性，讓終端使用者可進行修改 (若省略，則預設為 true)。
* **mktoLockImgStyle：**&#x200B;用於鎖定 `<img>` 元素的樣式屬性 (預設為 false)。

範例：`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## 程式碼片段 {#snippets}

如果您將區域定義為程式碼片段，則終端使用者即可選擇要在此區域中插入哪個已核准的[程式碼片段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)。雖然 RTF 文字元素可以從電子郵件編輯器內轉換為程式碼片段，但如果您明確地將區域定義為程式碼片段，則無法將其轉換為 RTF 文字。您可以使用具有 class=&quot;mktoSnippet&quot; 的 `<div>` 來指定程式碼片段區域

必要屬性

* **id：**&#x200B;識別碼字串。僅包含字母、數字、破折號「-」和底線「_」。不允許有任何空格。必須為唯一。
* **mktoName：**&#x200B;字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

預設值 (選用)

**mktoDefaultSnippetId**：預設應顯示的 Marketo 程式碼片段數值識別碼 (只有在該工作區中已存在並核准具有該識別碼的程式碼片段時才能運作)。

範例：

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## 影片 {#video}

如果您將一塊區域定義為影片，則終端使用者即可插入將在電子郵件中顯示為縮圖影像 (包含「播放」按鈕) 的 YouTube 或 Vimeo URL。您可以使用具有 class=&quot;mktoVideo&quot; 的 `<div>` 來指定影片區域

必要屬性

* **id：**&#x200B;識別碼字串。僅包含字母、數字、破折號「-」和底線「_」。不允許有任何空格。必須為唯一。
* **mktoName：**&#x200B;字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **mktoImgClass：**&#x200B;字串。這裡的值會新增至 div 內影片縮圖 `<img>` 的類別屬性。

範例：

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## 變數 {#variables}

變數就像權杖。您可先使用 `<meta>` 標記在電子郵件範本的 `<head>` 區段中定義它們，然後就可以在整個範本中依您的需要多次使用。由於已在範本中定義，終端使用者即可根據其規則修改其值。請注意，您可以在範圍中將變數定義為區域或全域。如果您在「模組」中使用變數 (請參閱下文)，而終端使用者重複該模組，則區域變數會具有獨立的值，而全域變數則同時適用於兩個模組。

## 字串 {#string}

如果您將變數指定為字串，則終端使用者即可在電子郵件編輯器的文字方塊中輸入文字。您可使用具有 class=&quot;mktoString&quot; 的 `<meta>` 來指定字串變數

必要屬性

* **id：**&#x200B;如何在電子郵件範本中參照變數。
* **mktoName：**&#x200B;字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **allowHTML：**&#x200B;布林值。控制變數的值是否為 HTML 逸出。若省略，則預設為 False。
* **default**：字串的預設值。若省略，則為空白。
* **mktoModuleScope**：布林值。控制變數用於模組中時為區域 (true) 或全域 (false)。若省略，則預設為 False。

範例宣告：

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

範例用法：

`${textHeader}`

## 清單 {#list}

如果您將變數指定為「清單」，則終端使用者即可從您在電子郵件編輯器中定義的一組值中進行挑選。您可使用具有 class=&quot;mktoList&quot; 的 `<meta>` 來指定清單變數

必要屬性

* **id**：如何在電子郵件範本中參照變數。
* **mktoName：**&#x200B;字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。
* **values：**&#x200B;以逗號分隔的值清單。必須至少有一個字串。

選擇性屬性

* **default：**&#x200B;特定下拉式清單的預設值。若省略，則會使用「values」屬性的第一個值。
* **mktoModuleScope**：布林值。控制變數用於模組中時為區域 (true) 或全域 (false)。若省略，則預設為 False。

範例宣告：

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

範例用法：

`${textFontFamily}`

## 數字 {#number}

如果您將變數指定為數字，則終端使用者即可在電子郵件編輯器中輸入數字。您可使用具有 class=&quot;mktoNumber&quot; 的 `<meta>` 來指定數字變數

必要屬性

* **id**：如何在電子郵件範本中參照變數。
* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。
* **default：**&#x200B;變數的預設數值。

選擇性屬性

* **min：**&#x200B;最小可接受值。
* **max：**&#x200B;最大可接受值。
* **units：**&#x200B;在電子郵件編輯器以及產生的程式碼中顯示時要附加至數字值 (例如：px、pt、em 等) 的單位。
* **step：**&#x200B;數字變數應該增加/減少多少單位 (0.1、1、10 等)。若省略，則預設為 1。
* **mktoModuleScope**：布林值。控制變數用於模組中時為區域 (true) 或全域 (false)。若省略，則預設為 False。

範例宣告：

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

範例用法：

`${textFontSize}`

## 顏色 {#color}

如果您將變數指定為「顏色」，則終端使用者即可輸入十六進位顏色值，或從電子郵件編輯器中的檢色器中選擇顏色。您可使用具有 class=&quot;mktoColor&quot; 的 `<meta>` 來指定顏色變數

必要屬性

* **id**：如何在電子郵件範本中參照變數。
* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **default:**&#x200B;顏色的預設值。6 位數的十六進位顏色代碼。例如：#ffffff。
* **mktoModuleScope**：布林值。控制變數用於模組中時為區域 (true) 或全域 (false)。若省略，則預設為 False。

範例宣告：

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

範例用法：

`${textColor}`

## 布林值 {#boolean}

如果您將變數指定為布林值，終端使用者即可在電子郵件編輯器中切換開啟/關閉選項。您可使用具有 class=&quot;mktoBoolean&quot; 的 `<meta>` 來指定布林值變數

必要屬性

* **id**：如何在電子郵件範本中參照變數。
* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **default：**&#x200B;決定切換開關預設狀態的布林值。若省略，則為 False。
* **false_value：**&#x200B;切換開關處於「關閉」位置時要插入的值。若省略，則為 False。
* **true_value：**&#x200B;切換開關處於「開啟」位置時要插入的值。若省略，則為 True。
* **false_value_name：**&#x200B;切換開關在「關閉」位置時所顯示的 UI。若省略，則為 False。
* **true_value_name：**&#x200B;切換開關在「開啟」位置時所顯示的 UI。若省略，則為 True。
* **mktoModuleScope**：布林值。控制變數用於模組中時為區域 (true) 或全域 (false)。若省略，則預設為 False。

範例宣告：

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

範例用法：

`${showFooter}`

## HTML 區塊 {#html-block}

如果您將變數指定為 HTML 區塊，則終端使用者即可從電子郵件編輯器中輸入逐字 HTML。您可使用具有 class=&quot;mktoHTML&quot; 的 `<meta>` 來指定 HTML 區塊變數

必要屬性

* **id**：如何在電子郵件範本中參照變數。
* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **default：**&#x200B;用於作為區塊預設內容的 HTML 編碼值。
* **mktoModuleScope**：布林值。控制變數用於模組中時為區域 (true) 或全域 (false)。若省略，則預設為 False。

範例宣告：

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

範例用法：

`${trackingPixel}`

## 影像變數 {#image-variable}

如果您將變數指定為影像，則終端使用者即可從電子郵件編輯器內的影像選擇器中選擇影像。選取的影像 URL 即為變數的值。您可使用具有 class=&quot;mktoImg&quot; 的 `<meta>` 來指定影像變數

必要屬性

* **id**：如何在電子郵件範本中參照變數。
* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **default：**&#x200B;元素的預設影像 URL。
* **mktoModuleScope**：布林值。控制變數用於模組中時為區域 (true) 或全域 (false)。若省略，則預設為 False。

範例宣告：

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

範例用法：

`${heroBackgroundImage}`

## 模組 {#modules}

模組為在範本層級所定義的範本化區段，會顯示以供終端使用者插入其電子郵件中。由於您已預先建立這些模組，因此可確保這些模組會和您電子郵件的其餘內容順暢地 (以完整回應式方式) 互動。您僅能將模組放入容器中。

>[!IMPORTANT]
>
>若電子郵件是從包含已定義模組元件的電子郵件範本產生，對範本模組所進行的任何變更都&#x200B;**不會**&#x200B;推送至該電子郵件。

**對於 `<table>`、`<tbody>`、`<thead>` 或 `<tfoot>` 類型的容器：**

已使用具有 class=&quot;mktoModule&quot; 的 `<tr>` 來指定

**對於 `<td>` 類型的容器：**

已使用具有 class=&quot;mktoModule&quot; 的 `<table>` 來指定

必要屬性

* **id**：如何在電子郵件範本中參照模組。
* **mktoName**：字串。這是會在電子郵件編輯器 2.0 中顯示的顯示名稱。最佳做法為使用描述性名稱。

選擇性屬性

* **mktoActive：**&#x200B;決定此模組是否會顯示在電子郵件編輯器內的模組清單中。預設為 true。若為 false，則終端使用者即無法將該模組新增至電子郵件。
* **mktoAddByDefault：**&#x200B;決定此模組在建立時是否會在使用此範本的新電子郵件畫布中。預設為 true (如果 mktoActive 為 false，則會忽略此值)。

>[!NOTE]
>
>包含 Marketo 語法的類別值 (即 mktoModule、mktoContainer、mktoText) 會區分大小寫。自訂屬性名稱 (即 mktoimgwidth、mktoname) 則不會。

## 容器 {#containers}

容器會保存模組，並定義可放置模組的位置。終端使用者重新排序並將模組插入其電子郵件時，容器會控制可放置的位置。

**已使用具有 class=&quot;mktoContainer&quot; 的 `<table>`、`<tbody>`、`<thead>`、`<tfoot>` 或 `<td>` 來指定**

必要屬性

**id**：如何在電子郵件範本中參照模組。

>[!CAUTION]
>
>容器僅能包含模組 - 如果出現其他內容，則會將容器視為無效！每個範本僅允許一個容器。
