---
unique-page-id: 2359414
description: 簡單計分——行銷檔案——產品檔案
title: 簡易計分
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---


# 簡易計分 {#simple-scoring}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!PREREQUISITES]
>
>* [設定並新增人員](get-set-up-and-add-a-person.md)
>* [具有表單的著陸頁面](landing-page-with-a-form.md)

>



## 步驟1:建立計分促銷活動 {#step-create-a-scoring-campaign}

1. 前往「行銷 **活動** 」區。

   ![](assets/ma-1.png)

1. 以滑鼠右鍵按一下 **Learning** 資料夾，然後按 **一下New Campaign資料夾**。

   ![](assets/two-2.png)

1. 將促銷活動資料夾命名為「計分」。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >如果您已有「計分」資料夾，請將此資料夾命名為不同的名稱，例如「計分1」。 資料夾名稱必須是唯一的。

1. 然後以滑鼠右鍵按一下新的 **計分資料夾** ，並選 **取新的智慧型促銷活動**。

   ![](assets/four.png)

1. **將促銷活動命名** 「變更分數」，然後按一下「建 **立**」。

   ![](assets/five-1.png)

1. 按一下「智 **能清單** 」頁籤。

   ![](assets/six-1.png)

   我們希望此促銷活動在使用者填寫您的試用 **申請表時執行**。

1. 尋找並拖曳「填 **出表單」觸發器** ，到左側畫布上。

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. 選擇 **我的表單**。

   >[!NOTE]
   >
   >如果您完成「 [Landing Page」（著陸頁面）並取得Form](landing-page-with-a-form.md) quick win，則應該有此表單。 如果您對表單使用不同的名稱，請選取該名稱。

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. 按一下「**流量**」標籤。

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. 將「變 **更分數** 」流動動作拖曳至左側畫布。

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. 您可以輸入任何值以新增至人員的分數。 讓我們在「更改」欄位中輸入 **&quot;+5** &quot;。

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >良好的評分促銷活動是為銷售人員提供高品質人員的關鍵。 閱讀 [**銷售機會評分的最終指南**](http://www.marketo.com/definitive-guides/lead-scoring/)。

1. 按一下「 **排程** 」標籤和「 **啟動** 」按鈕。

   ![](assets/twelve-1.png)

1. 按一 **下確認畫面** 上的「啟動」。

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>活動後，每次有人填寫表單時，就會執行此促銷活動。 促銷活動會持續執行，直到停用為止。

## 步驟2:填寫表格 {#step-fill-out-the-form}

1. 選取您在「Landing Page」（著陸頁面） [中建立的「Form](landing-page-with-a-form.md) quick win」（表單快速成功）著陸頁面。

   ![](assets/fourteen-1.png)

1. 按一 **下「檢視核准頁面**」。 著陸頁面將會在新標籤中開啟。

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. 填寫表格並填入您的名字、姓氏和電子郵件地址，然後按一下「送 **出** 」。

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >使用您第一次以個人身分輸入時使用的相同名稱和電子郵件地址，以套用「+5」分數增加。

## 步驟3:檢視人員資訊 {#step-view-the-person-info}

1. 轉至「資料庫」區域。

   ![](assets/db-2.png)

1. 搜尋填寫表單時使用的電子郵件地址。

   ![](assets/eighteen.png)

1. 連按兩下您的人。

   ![](assets/nineteen.png)

您的人員詳細資料將會在新標籤或視窗中開啟。 瞭解填寫表格時，您的分數如何提高5分？!

![](assets/twenty.png)

**恭喜！** 您已建立計分促銷活動。
[◄使命2:Landing Page with a Form](landing-page-with-a-form.md) [Mission 4:電子郵件自動回應►](email-auto-response.md)