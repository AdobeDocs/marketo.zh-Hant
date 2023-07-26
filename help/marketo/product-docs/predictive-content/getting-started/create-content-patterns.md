---
unique-page-id: 11385579
description: 建立內容模式 — Marketo檔案 — 產品檔案
title: 建立內容模式
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 建立內容模式 {#create-content-patterns}

當您設定內容模式時，當網站訪客點按與內容模式相關的HTML網頁時，就會自動探索內容。 可用來將HTML頁面（部落格、新聞稿、新聞文章）以內容片段的方式新增至「所有內容」頁面。 當自動探索是根據內容模式時，它會在Web訪客檢視或按一下頁面的連結時，探索並追蹤與定義的URL模式相關的HTML頁面。 此內容片段（URL、頁面名稱和中繼資料，包括影像URL和說明）會新增至「所有內容」頁面，以準備預測性內容。 若要自動探索其他內容(例如PDF和內嵌視訊)，您需要 [啟用內容探索](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. 前往 **內容設定**.

   ![](assets/settings-dropdown-hand-2.png)

1. 按一下 **URL模式**.

   ![](assets/click-url-patterns-hand.png)

1. 按一下 **+** 以開啟可輸入資訊的列。

   ![](assets/content-settings-create-patterns-hand.png)

1. 新增網頁所在網域的URL副檔名。 選取類別（例如，部落格、文章、資料表、新聞稿）。

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >右側下拉式清單中的專案會反映您在設定時的類別 [已建立的類別](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. 按一下 **+** 以新增其他路徑。

   ![](assets/url-patterns-add2.png)

1. 新增其他路徑的副檔名和類別，然後按一下 **儲存**.

   ![](assets/url-patterns-save.png)

## 內容模式規則 {#content-pattern-rules}

* 您可以在運算式中的任何地方使用萬用字元(範例： _domain.com/&#42;_， _domain.com/&#42;部落格&#42;_)

* 我們建議使用/&#42; 在運算式結尾處，繼續模式探索(範例： _domain.com/blog/&#42;_ 探索Blog資料夾中的所有文章)
* 內容模式不區分大小寫(例如： _domain.com/Blog/&#42;_ 探索上的所有html頁面 _domain.com/Blog_ 和 _domain.com/blog_)

* 未探索URL引數（這可避免探索具有相同內容URL但不同引數的多個專案）

## 範例 {#examples}

的 _domain.com_：

<table> 
 <tbody> 
  <tr> 
   <th>URL模式</th> 
   <th>結果</th> 
  </tr> 
  <tr> 
   <td>部落格/*</td> 
   <td><p>探索符合模式domain.com/blog/的所有內容：</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>article/2017/*</td> 
   <td><p>探索符合模式domain.com/article/2017/的所有內容：</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>探索任何包含「資料表」一詞的URL：</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>新聞稿</td> 
   <td><p>只探索到一個完全相符的HTML頁面：</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>如果URL運算式為空，則URL模式只會探索首頁：</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
