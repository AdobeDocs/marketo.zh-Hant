---
description: 設定 — Marketo檔案 — 產品檔案
title: 設定
feature: Dynamic Chat
exl-id: 824cd1de-a407-4250-8777-33eec0777361
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 1%

---

# 設定 {#configuration}

瞭解如何自訂聊天機器人對話視窗的外觀。

若要開始，請按一下 **設定**.

![](assets/configuration-1.png)

有多種不同的自訂選項。

![](assets/configuration-2.png)

## 樣式標籤 {#style-tab}

### 樣式 {#style}

您將在此處定義顯示對話方塊的聊天機器人的外觀和風格，包括：顏色、字型、機器人Widget的位置以及聊天機器人的名稱/頭像。

每個類別的顏色由 [十六進位色彩值](https://color.adobe.com/create/color-wheel){target="_blank"} (例如，white = #ffffff、red = #bf1932等)。

![](assets/configuration-3.png)

錨點可讓您的網站訪客開啟/關閉對話方塊。 您可以選擇讓該圖示顯示在右下角或左下角。 您也可以增加/減少邊框間距（圖示與網頁底部之間的間距）。

![](assets/configuration-4.png)

### 專員設定 {#agent-settings}

在「代理程式設定」中，您可以將標籤新增至聊天箱(例如：「Adobe機器人」)，標籤會顯示在其頂端。 您也可以判斷回應延遲（以秒為單位），並變更您的聊天頭像。 若要上傳您自己的顯示圖片影像，請按一下 **+** 按鈕。

![](assets/configuration-5.png)

>[!NOTE]
>
>自訂頭像應為小於256kb且小於200x200畫素的正方形影像。 支援的檔案型別包括： .jpg、.png、.gif、.webp、.svg。

完成變更時，請記得按一下 **儲存**.

![](assets/configuration-6.png)

## 隱私權索引標籤 {#privacy-tab}

按一下 **隱私權** 索引標籤來新增/編輯網站隱私權原則的URL （選用）。

![](assets/configuration-7.png)

## 安裝標籤 {#installation-tab}

為了讓聊天機器人出現在您的網站上，您必須先安裝Dynamic ChatJavaScript程式碼片段。 按一下此標籤以尋找/複製必要的程式碼。 如果您不熟悉此作業，請連絡您的網站團隊或IT部門以尋求協助。

![](assets/configuration-8.png)

>[!TIP]
>
>如果您的網站使用內容安全性原則，您可能需要將下列URL加入白名單，聊天機器人才能如期運作：
>
>* `*.adoberesources.net`
>* `*.adobe.io`
>* `*.typekit.net`

>[!NOTE]
>
>Marketo支援未設定為協助疑難排解HTML。 如需HTML協助，請洽詢網頁開發人員。
