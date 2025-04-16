---
description: GenAI功能 — Marketo檔案 — 產品檔案
title: GenAI功能
feature: Interactive Webinars
exl-id: 3e0a41b0-7ff3-4676-bafc-4e7a0725a737
source-git-commit: a4db7dbc6d62edd3d2efdba08c402d762fdaf921
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# GenAI功能 {#gen-ai-features}

為您錄製的網路研討會自動產生章節和摘要，讓對象更容易存取和導覽。

* **自動產生章節**： AI支援的技術會為您的網路研討會內容建立章節。

* **AI產生的摘要**：取得網路研討會的自動化文字摘要。

* **可編輯的內容**：視需要使用手動和AI支援的編輯功能，修改產生的章節和摘要。

* **輕鬆整合**：將HTML程式碼複製到您選取的網頁編輯器，輕鬆將章節和摘要新增至您的登陸頁面。

## 啟用GenAI {#enable-genai}

>[!PREREQUISITES]
>
>在使用這些功能之前，您必須先接受Adobe GenAI條款與條件。 如果您尚未這麼做，請聯絡Adobe客戶團隊（您的客戶經理）以取得詳細資料。

在您接受Adobe GenAI條款與條件後，下一步就是為個別使用者啟用它。 方法是前往「**[!UICONTROL Admin]** > **[!UICONTROL Interactive Webinars]**」並選取哪些使用者應該可以存取GenAI。

![](assets/gen-ai-features-1.png){width="800" zoomable="yes"}

## 如何存取 {#how-to-access}

1. 導覽至Marketo Engage互動式網路研討會中的網路研討會概觀頁面。

1. 進行您的隨選網路研討會後，請等待30到60分鐘，讓AI處理您的錄製。 [產生]按鈕可用時，即變為可點按。

1. 按一下「**[!UICONTROL Generate]**」。

   ![](assets/gen-ai-features-2.png){width="800" zoomable="yes"}

1. 隨即開啟新標籤，顯示AI產生的章節和文字摘要。

## 編輯產生的內容 {#edit-generated-content}

1. 檢閱產生的章節和摘要。

1. 如果需要變更，請按一下&#x200B;**[!UICONTROL Edit]**&#x200B;按鈕。

   進行修改：

   * 編輯摘要和/或章節標題中的文字。

   * 如有需要，可編輯時間戳記欄位中的值，以調整時間戳記。

   * 選取不要的章節並按一下&#x200B;**[!UICONTROL Delete]**&#x200B;以刪除它們。

   * 選取兩個連續章節並按一下&#x200B;**[!UICONTROL Merge]**&#x200B;以合併它們。

      * AI會產生由兩個所選章節組成的複合章節

      * 若要合併多個章節，您必須一次合併兩個章節

     ![](assets/gen-ai-features-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >* 如有需要，您可以使用&#x200B;_向上縮圖_ ![向上縮圖圖示](assets/icon-thumbs-up.png)或&#x200B;_向下縮圖_ ![向下縮圖圖示](assets/icon-thumbs-down.png)圖示，來評等產生的章節/摘要品質。 您也可以按一下標幟圖示![標幟圖示](assets/icon-flag.png)來標幟任何有問題的內容。
   >
   >* 如果您對初始摘要不滿意，可以按一下「**[!UICONTROL Regenerate summary]**」按鈕並產生另一個版本。

1. 按一下畫面右上方的&#x200B;**[!UICONTROL Save]**&#x200B;按鈕以儲存變更。

## 使用產生的內容 {#use-generated-content}

複製您要使用的內容後，將其貼到您選擇的編輯器(例如Marketo Engage登陸頁面編輯器)中並進行任何所需的調整。

### 摘要 {#summary}

**複製HTML** — 按一下「**[!UICONTROL Copy HTML]**」按鈕以取得所有文字，並在表格內以HTML程式碼格式化。

**僅限文字** — 如果您只想要文字，只要反白文字，並選取Ctrl/Cmd+C （或按一下滑鼠右鍵）加以複製即可。

### 章節 {#chapters}

**複製HTML** — 按一下「**[!UICONTROL Copy HTML]**」按鈕，在視訊播放器內取得所有錄製內容及其章節的格式。

## 注意事項 {#things-to-note}

* 刪除或合併章節只會影響章節棧疊，不影響視訊內容本身。 這些動作是永久性的。

* GenAI功能具有彈性，可搭配各種網頁編輯器使用，而不僅僅是Marketo Engage中的編輯器。

* 請一律預覽您的變更，以確保所需的功能和外觀。

* 刪除網路研討會也會刪除GenAI內容。

* 如果您想要刪除GenAI內容而不刪除網路研討會，請聯絡Adobe帳戶團隊（您的帳戶經理），或傳送資料刪除請求到： `marketo-webinar-genai-alerts@adobe.com`。
