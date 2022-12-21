---
unique-page-id: 11385579
description: 建立內容模式 — Marketo檔案 — 產品檔案
title: 建立內容模式
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 建立內容模式 {#create-content-patterns}

當您設定內容模式時，當網頁訪客點按與內容模式相關的HTML網頁時，會自動探索內容。 它可用來將HTML頁面（部落格文章、新聞稿、新聞文章）新增為「所有內容」頁面的內容片段。 當自動探索是根據內容模式時，它會在網頁訪客檢視或按一下頁面連結時，探索並追蹤與定義的URL模式相關的HTML頁面。 此內容片段(URL、頁面名稱和中繼資料（包括影像URL和說明）會新增至「所有內容」頁面，以準備預測內容。 若要自動探索其他內容，例如PDF和內嵌視訊，您需要 [啟用內容探索](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. 前往 **內容設定**.

   ![](assets/settings-dropdown-hand-2.png)

1. 按一下 **URL模式**.

   ![](assets/click-url-patterns-hand.png)

1. 按一下 **+** 以開啟一行，在其中可以輸入資訊。

   ![](assets/content-settings-create-patterns-hand.png)

1. 新增網頁存在之網域的URL副檔名。 選取類別（例如，部落格、文章、資料表、新聞發佈）。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右側下拉式清單中的項目會反映您在 [建立類別](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. 按一下 **+** 來新增其他路徑。

   ![](assets/url-patterns-add2.png)

1. 新增其他路徑的擴充功能和目錄，然後按一下 **儲存**.

   ![](assets/url-patterns-save.png)

## 內容模式規則 {#content-pattern-rules}

* 您可以在運算式中的任何地方使用萬用字元(範例： _domain.com/&#42;_, _domain.com/&#42;部落格&#42;_)

* 建議使用/&#42; 在運算式的結尾處，以繼續模式探索(範例： _domain.com/blog/&#42;_ 發現部落格資料夾中的所有貼文)
* 內容模式不區分大小寫(例如： _domain.com/Blog/&#42;_ 會探索到所有html頁面 _domain.com/Blog_ 和 _domain.com/blog_)

* 未探索到URL參數（這可避免探索到多個項目，其中包含相同的內容URL，但參數不同）

## 範例 {#examples}

針對 _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>URL模式</th> 
   <th>結果</th> 
  </tr> 
  <tr> 
   <td>部落格/*</td> 
   <td><p>探索符合模式的所有內容domain.com/blog/ :</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>第2017/*條</td> 
   <td><p>探索符合模式的所有內容domain.com/article/2017/ :</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>發現包含「資料表：」一詞的任何URL</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>新聞稿</td> 
   <td><p>只會發現一個完全相符的HTML頁面：</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>如果URL運算式為空，URL模式只會探索首頁：</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
