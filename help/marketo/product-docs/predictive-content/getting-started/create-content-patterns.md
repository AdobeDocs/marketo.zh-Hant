---
unique-page-id: 11385579
description: 建立內容模式——行銷檔案——產品檔案
title: 建立內容模式
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---


# 建立內容模式{#create-content-patterns}

當您設定內容模式時，當網頁訪客點按與內容模式相關的HTML網頁時，就會自動發現內容。 它可用來將HTML頁面（部落格文章、新聞稿、新聞文章）新增至「所有內容」頁面。 當自動發現是以內容模式為基礎時，它會在網頁訪客檢視或點按頁面連結時，發現並追蹤與已定義URL模式相關的HTML頁面。 此內容片段（URL、頁面名稱和中繼資料，包括影像URL和說明）會新增至「所有內容」頁面，以準備預測性內容。 若要自動發現其他內容，例如PDF和內嵌視訊，您必須[啟用內容發現](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md)。

1. 前往&#x200B;**內容設定**。

   ![](assets/settings-dropdown-hand-2.png)

1. 按一下「URL模式」。****

   ![](assets/click-url-patterns-hand.png)

1. 按一下&#x200B;**+**&#x200B;以開啟您可輸入資訊的列。

   ![](assets/content-settings-create-patterns-hand.png)

1. 新增網頁所在網域的URL副檔名。 選擇類別（例如，部落格、文章、資料表、新聞發佈）。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右側下拉式清單中的項目會反映您在[建立類別](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md)時所設定的類別。

1. 按一下&#x200B;**+**&#x200B;添加其他路徑。

   ![](assets/url-patterns-add2.png)

1. 添加附加路徑的副檔名和目錄，然後按一下&#x200B;**保存**。

   ![](assets/url-patterns-save.png)

## 內容模式規則{#content-pattern-rules}

* 可以在表達式中的任意位置使用通配符(示例：_domain.com/*_、_domain.com/*blog*_

* 建議在運算式結尾使用/*以繼續模式搜尋(範例：_domain.com/blog/*_&#x200B;會發現Blog資料夾中的所有貼文)
* 內容模式不區分大小寫(範例：_domain.com/Blog/*_&#x200B;會發現&#x200B;_domain.com/Blog_&#x200B;和&#x200B;_domain.com/blog_&#x200B;上的所有html頁面

* 未發現URL參數（這可避免發現具有相同內容URL但參數不同的多個項目）

## 範例{#examples}

對於&#x200B;_domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>URL模式</th> 
   <th>結果</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>發現所有符合模式的內容domain.com/blog/:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>article/2017/*</td> 
   <td><p>發現所有符合模式的內容domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="—"></td> 
   <td><p>發現包含"資料表："的任何URL</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>新聞稿</td> 
   <td><p>只發現一個完全符合的HTML頁面：</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>如果URL運算式為空，URL模式只會發現首頁：</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
