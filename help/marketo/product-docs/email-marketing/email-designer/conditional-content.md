---
solution: Marketo Engage
product: marketo
title: 條件式內容
description: 在電子郵件中使用條件式內容，以根據收件者動態顯示內容。
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 6b9f6d4b276115e1f3f3dac73eb64e5358a76516
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# 條件式內容 {#conditional-content}

條件式內容可讓您動態控制哪些對象可以看到哪些內容。 使用現有的區段，根據預先定義的條件來決定收件者看到的內容。

>[!PREREQUISITES]
>
>已建立至少一個區段[&#128279;](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)且[已核准](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)。

## 新增條件式內容 {#add-conditional-content}

1. 開啟所需的電子郵件，然後按一下&#x200B;**編輯電子郵件內容**。

   ![](assets/conditional-content-1.png)

1. 選取您要設定條件的內容（在此範例中，我們選取的是頁首影像）。 按一下&#x200B;_啟用條件式內容_&#x200B;圖示。

   ![](assets/conditional-content-2.png)

1. 反白方塊會變成橘色。 在左側，按一下&#x200B;_選取條件_&#x200B;圖示(![](assets/icon-select-condition.png))以定義變體。

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. 選擇想要的區段，然後按一下&#x200B;**選取**。

   ![](assets/conditional-content-4.png)

1. 按一下&#x200B;_編輯影像_&#x200B;圖示以取代變體的現有影像。 選擇新影像的來源。 在此範例中，我們在Marketo Engage訂閱中選擇&#x200B;_影像與檔案_&#x200B;資料庫。

   ![](assets/conditional-content-5.png)

1. 選擇適用的影像，然後按一下&#x200B;**選取**。

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. 新影像隨即顯示。 建議您重新命名變體，以便於識別。 只要按一下省略符號並選取&#x200B;**重新命名**&#x200B;即可。

   >[!NOTE]
   >
   >按一下省略符號也可讓您檢視及複製變體的已定義條件。 如果您有多個變體，則可使用刪除選項。 如果您只有一個變體，刪除該變體的方式是只要重新按一下&#x200B;_啟用條件式內容_&#x200B;圖示（現在當您將游標停留在變體上時，會顯示&#x200B;_停用條件式內容_）。

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. 若要新增其他變體（選擇性），請按一下[新增變體] **&#x200B;**，然後遵循相同的步驟。

   ![](assets/conditional-content-8.png)

1. 完成後，每個變體都會顯示您選取的內容。

   ![](assets/conditional-content-9.gif)

1. 收件者會根據每個區段中定義的規則檢視內容。 在上述範例中，凡是在您的Marketo Engage欄位&#x200B;_最愛的運動_&#x200B;中列出「足球」的人，都會看到足球影像。

>[!MORELIKETHIS]
>
>* [定義區段規則](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [在Marketo中建立自訂欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
