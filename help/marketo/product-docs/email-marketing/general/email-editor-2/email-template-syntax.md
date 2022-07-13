---
unique-page-id: 11371040
description: 電子郵件模板語法 — Marketo文檔 — 產品文檔
title: 電子郵件模板語法
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# 電子郵件模板語法 {#email-template-syntax}

在Marketo的新Email 2.0體驗中，電子郵件模板由元素、變數、模組或容器的任意組合組成。 每個都通過向HTML添加特定於Marketo的語法來定義。 舊(v1.0)電子郵件模板在電子郵件編輯器2.0中受支援；不過，新編輯的所有功能都不包括在內。

Marketo的電子郵件語法只適用於模板和單個電子郵件；它 **不** 如果嵌入到代碼段或富文本標籤中，則工作。

>[!NOTE]
>
>Marketo支援未設定為協助CSS/HTML。 如果您不熟悉CSS/HTML，請咨詢您的開發人員。

>[!CAUTION]
>
>包含Marketo語法的類值（即mktoModule、mktoContainer、mktoText）區分大小寫。 自定義屬性名稱（即mktoimgwidth、mktoname）不是。

## 元素 {#elements}

元素是您在電子郵件模板中定義為可編輯的內容區域。 元素的編輯體驗是其類型所獨有的，並提供了處理內容的簡單方法。 電子郵件模板中可能包含的元素包括：

* 富文本
* 影像
* 片段
* 視頻

## 富文本 {#rich-text}

如果將區域定義為RTF，則用戶將能夠編輯其內容 [使用Marketo的富格文本編輯器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)。 在電子郵件模板中定義富格文本元素有兩種方法：mktEditable和mktoText。 請記住， Rich Text元素始終可以從電子郵件編輯器中轉換為代碼段。

### 選項1 - mktEditable {#option-mkteditable}

由於Email Editor 2.0向後相容，因此某些舊電子郵件模板可能通過在任何HTML元素上添加class=&quot;mktEditable&quot;來指定富文本元素。 這仍然受支援，並且元素的ID是將在電子郵件編輯器中用作顯示名稱的內容。

必需屬性

* **類**:&quot;mktEditable&quot;。
* **ID**:ID字串。 僅包含字母、數字、破折號「 — 」和下划線「_」。 不允許使用空格。 必須唯一。

可選屬性

* **mkto名稱** :字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

預設值

HTML元素（如果提供）中包含class=&quot;mktEditable&quot;的內容將用作RT元素的預設值。

示例：

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### 選項2 - mktoText {#option-mktotext}

建議使用class=&quot;mktoText&quot;語法指定Rich Text元素。 這可確保元素始終具有正確的顯示名稱。

必需屬性

* **類**:&quot;mktoText&quot;
* **ID**:ID字串。 僅包含字母、數字、破折號「 — 」和下划線「_」。 不允許使用空格。 必須唯一。
* **mkto名稱** :字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

預設值

HTML元素（如果提供）中包含class=&quot;mktoText&quot;的內容將用作RTF元素的預設值。

示例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 影像 {#images}

您有兩個用於定義可編輯影像元素的選項。 您可以使用 `<div>`，它指定 `<img>` 將插入，或 `<img>` 標籤。 如果希望最終用戶僅選擇將返回影像URL（而不是DOM）的影像，請參閱下面一節中的「影像變數」。 以下兩個選項將插入一個HTML `<img>` 的子菜單。

### 選項1 — 使用 `<div>` {#option-use-a-div}

必需屬性

* **類：** &quot;mktoImg&quot;。
* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和下划線「_」。 不允許使用空格。 必須唯一。
* **mktoName :** 字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **mktoImgClass:** 字串。 此處的值將添加到的類屬性 `<img>` div中的元素。
* **mktoImgSrc:** 用作放置在此div中的影像的預設值。 如果省略此項，則使用佔位符。
* **mktoImgLink:** 表示 `<img>` 應該被一個 `<a>` 標籤。 用戶可以在電子郵件編輯器中更改此項。
* **mktoImgLinkTarget:** 表示 `<a>` mktoImgLink屬性中的標籤應使用此目標。 如果未使用mktoImgLink，則無效。
* **mktoImg寬度：** 用作封閉上的寬度 `<img>`。
* **mktoImgHeight:** 用作封閉上的高度 `<img>`。
* **mktoLockImgSize:** 用於解鎖 `<img>` 元素的height和width屬性，以便最終用戶可以修改（如果省略，則預設為true）。
* **mktoLockImgStyle:** 用於鎖定 `<img>` 元素的style屬性（預設為false）。

預設值（可選）

**`<img>`**:用作 `<img>` 將放置影像的元素。 如果要向影像添加內聯樣式，則非常有用。 記住要包括周圍 `<a> </a>` 標籤，因此如果用戶添加連結，您的樣式將不會被刪除！

示例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### 選項2 — 使用\&lt;img> {#option-use-an-img}

>[!NOTE]
>
>此選項不允許最終用戶向其映像添加連結。 如果這對模板很重要，請使用選項1。

必需屬性

* **類：** &quot;mktoImg&quot;。
* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和下划線「_」。 不允許使用空格。 必須唯一。
* **mkto名稱：** 字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。  預設值（可選）
* **src:** 用作影像的預設值。 如果省略此項，則使用佔位符。
* **mktoLockImgSize:** 用於解鎖 `<img>` 元素的height和width屬性，以便最終用戶可以修改（如果省略，則預設為true）。
* **mktoLockImgStyle:** 用於鎖定 `<img>` 元素的style屬性（預設為false）。

示例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## 片段 {#snippets}

如果將區域定義為代碼段，則最終用戶將能夠選擇批准的 [代碼段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)他們想在這個區域插入。 雖然可以在電子郵件編輯器中將富文本元素轉換為片段，但當您將某個區域具體定義為「片段」時，它無法轉換為富文本。 可以使用 `<div>` with class=&quot;mktoSnippet&quot;

必需屬性

* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和下划線「_」。 不允許使用空格。 必須唯一。
* **mkto名稱：** 字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

預設值（可選）

**mktoDefaultSnippetId**:預設情況下應出現的Marketo代碼段的數字ID（僅當具有該ID的代碼段存在且在該工作區中已獲批准時才起作用）。

示例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## 視頻 {#video}

如果將一個區域定義為視頻，最終用戶將能夠在電子郵件內插入一個YouTube或Vimeo URL，該URL將顯示為縮略圖（使用「播放」按鈕）。 可以使用 `<div>` 與class=&quot;mktoVideo&quot;

必需屬性

* **id:** ID字串。 僅包含字母、數字、破折號「 — 」和下划線「_」。 不允許使用空格。 必須唯一。
* **mkto名稱：** 字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **mktoImgClass:** 字串。 此處的值將添加到視頻縮略圖的class屬性 `<img>` div內。

示例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 變數 {#variables}

變數就像令牌。 首先在 `<head>` 使用 `<meta>` 標籤，然後在整個模板中使用它們的次數。 因為它們是在模板中定義的，因此最終用戶將能夠根據其規則修改其值。 請注意，可將變數定義為局部或全局範圍。 如果在「模組」中使用變數（請參見下面的內容），並且最終用戶複製該模組，則本地變數將具有獨立值，而全局變數將應用於這兩個模組。

## 字串 {#string}

如果將變數指定為「字串」，則最終用戶將能夠在電子郵件編輯器的文本框中輸入文本。 使用 `<meta>` 與class=&quot;mktoString&quot;

必需屬性

* **id:** 如何在電子郵件模板中引用變數。
* **mkto名稱：** 字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **allowHTML:** 布爾型。 控制變數的值是否是HTML轉義的。 如果省略，則預設為False。
* **預設**:字串的預設值。 如果省略，則為空。
* **mktoModuleScope**:布爾型。 控制在模組中使用變數時，變數是本地(true)還是全局(false)。 如果省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

示例用法：

`<pre data-theme="Confluence">${textHeader}</pre>`

## 清單 {#list}

如果將變數指定為「清單」，則最終用戶將能夠從您在電子郵件編輯器中定義的一組值中進行選擇。 使用 `<meta>` 與class=&quot;mktoList&quot;

必需屬性

* **ID**:如何在電子郵件模板中引用變數。
* **mkto名稱：** 字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。
* **值：** 以逗號分隔的值清單。 必須至少有一個字串。

可選屬性

* **預設：** 選擇下拉清單的預設值。 如果省略，則使用「values」屬性中的第一個值。
* **mktoModuleScope**:布爾型。 控制在模組中使用變數時，變數是本地(true)還是全局(false)。 如果省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

示例用法：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 數字 {#number}

如果將變數指定為「數字」，則最終用戶將能夠在電子郵件編輯器中輸入數字。 使用 `<meta>` 與class=&quot;mktoNumber&quot;

必需屬性

* **ID**:如何在電子郵件模板中引用變數。
* **mkto名稱**:字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。
* **預設：** 變數的預設數值。

可選屬性

* **分鐘：** 最小接受值。
* **最大：** 最大接受值。
* **單位：** 要附加到數字值的單位(例如：px、pt、em等) 顯示在「電子郵件編輯器」中，以及生成的代碼中。
* **步驟：** 數量變數應增加/減少的單位數（0.1、1、10等）。 如果省略，則預設為1。
* **mktoModuleScope**:布爾型。 控制在模組中使用變數時，變數是本地(true)還是全局(false)。 如果省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

示例用法：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## 顏色 {#color}

如果將變數指定為「顏色」，則最終用戶將能夠輸入十六進位顏色值或從電子郵件編輯器中的顏色選擇器中選擇顏色。 使用 `<meta>` 與class=&quot;mktoColor&quot;

必需屬性

* **ID**:如何在電子郵件模板中引用變數。
* **mkto名稱**:字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **預設：** 顏色的預設值。 6位十六進位顏色代碼。 例如：#ffffff。
* **mktoModuleScope**:布爾型。 控制在模組中使用變數時，變數是本地(true)還是全局(false)。 如果省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

示例用法：

`<pre data-theme="Confluence">${textColor}</pre>`

## 布林值 {#boolean}

如果將變數指定為布爾值，則最終用戶將能夠在電子郵件編輯器中開啟/關閉選項。 使用 `<meta>` with class=&quot;mktoBoolean&quot;

必需屬性

* **ID**:如何在電子郵件模板中引用變數。
* **mkto名稱**:字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **預設：** 確定切換開關的預設狀態的布爾值。 如果省略，則為False。
* **false_value:** 切換處於OFF位置時要插入的值。 如果省略，則為False。
* **true_value:** 切換處於ON位置時要插入的值。 如果省略，則為True。
* **false_value_name:** 當處於「關閉」位置時，切換中顯示的UI。 如果省略，則為False。
* **true_value_name:** 當處於ON位置時，切換中顯示的UI。 如果省略，則為True。
* **mktoModuleScope**:布爾型。 控制在模組中使用變數時，變數是本地(true)還是全局(false)。 如果省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

示例用法：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML塊 {#html-block}

如果將變數指定為HTML塊，則最終用戶將能夠從電子郵件編輯器中輸入逐字HTML。 使用指定HTML塊變數 `<meta>` 與class=&quot;mktoHTML&quot;

必需屬性

* **ID**:如何在電子郵件模板中引用變數。
* **mkto名稱**:字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **預設：** HTML編碼值，用作塊的預設內容。
* **mktoModuleScope**:布爾型。 控制在模組中使用變數時，變數是本地(true)還是全局(false)。 如果省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

示例用法：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 影像變數 {#image-variable}

如果將變數指定為「影像」，則最終用戶將能夠從電子郵件編輯器中的影像選取器中選擇影像。 所選影像URL將是變數的值。 使用 `<meta>` 與class=&quot;mktoImg&quot;

必需屬性

* **ID**:如何在電子郵件模板中引用變數。
* **mkto名稱**:字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **預設：** 元素的預設影像URL。
* **mktoModuleScope**:布爾型。 控制在模組中使用變數時，變數是本地(true)還是全局(false)。 如果省略，則預設為False。

示例聲明：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

示例用法：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## 模組 {#modules}

模組是在模板級別定義的模板化部分，這些部分將顯示給最終用戶，供其插入電子郵件。 因為您已預先構建了這些模組，所以您可以確保它們能夠與您的其餘電子郵件內容（以完全響應的方式）正常交互。 您只能將模組放入容器中。

>[!IMPORTANT]
>
>當從包含已定義模組元件的電子郵件模板生成電子郵件時，對模板的模組所做的任何更改都將 **不** 被推送到郵件中。

**用於類型的容器 `<table>`。 `<tbody>`。 `<thead>`或 `<tfoot>`:**

使用 `<tr>` 與class=&quot;mktoModule&quot;

**用於類型的容器 `<td>`:**

使用 `<table>` 與class=&quot;mktoModule&quot;

必需屬性

* **ID**:在電子郵件模板中引用模組的方式。
* **mkto名稱**:字串。 這是將在電子郵件編輯器2.0中顯示的顯示名稱。最佳做法是使用描述性名稱。

可選屬性

* **mktoActive:** 確定此模組是否出現在電子郵件編輯器中的模組清單中。 預設為true。 如果為false，則最終用戶無法將模組添加到電子郵件中。
* **mktoAddByDefault:** 確定此模組是否位於建立時使用此模板的新電子郵件的畫布中。 預設值為true（如果mktoActive為false，則忽略此值）。

>[!NOTE]
>
>包含Marketo語法的類值（即mktoModule、mktoContainer、mktoText）區分大小寫。 自定義屬性名稱（即mktoimgwidth、mktoname）不是。

## 容器 {#containers}

容器容納模組並定義可放置模組的位置。 當最終用戶重新訂購模組並將其插入其電子郵件中時，容器會控制他們可以去哪裡。

**使用 `<table>`。 `<tbody>`。 `<thead>`。 `<tfoot>` 或 `<td>` 與class=&quot;mktoContainer&quot;**

必需屬性

**ID**:在電子郵件模板中引用模組的方式。

>[!CAUTION]
>
>容器只能包含模組 — 如果存在其他內容，則容器被視為無效！ 每個模板只允許一個容器。
