---
description: 瞭解C2PA中繼資料如何自動附加至Marketo Engage中AI產生的影像、透過編輯保留，並用於內容來源。
title: Marketo Engage中的C2PA中繼資料
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 10781cbfd51019a2e4af346803a2e35ef40855d0
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 2%

---

# Marketo Engage中的C2PA中繼資料

圍繞創作AI透明度的新法律不斷湧現，Adobe正在努力滿足各個司法轄區的適用要求。 C2PA中繼資料是Adobe用來符合這些法律要求的來源工具。

C2PA中繼資料是持久且隱藏的中繼資料，會記錄內容的建立或編輯方式。 當您在Marketo Engage中使用產生式AI工具產生或編輯影像時，C2PA中繼資料會自動附加至該影像（您不需要採取任何動作）。 它是加密且易於篡改的資訊，可協助檢視者瞭解內容的譜系並確保品牌資產的完整性。 此資訊包括：

* **簽發者或簽署者**：發行數位簽章以認證或簽署資產的實體或公司的相關資訊。
* **問題日期**： C2PA中繼資料套用至資產的日期。
* **評分與使用狀況**：資產製作者的相關資訊，包括名稱、社群媒體控制代碼或其他身分相關資訊。
* **處理序**：對資產進行任何編輯或修改的記錄。
* **裝置詳細資料**：有關用來建立或編輯資產的應用程式或裝置的資訊。
* **使用的AI工具**：如果使用generative AI建立資產，則可能會包含使用的模型名稱。
* **其他相關資訊**：也包含其他資料，以協助提供有關資產歷史記錄的更多內容。

## 附加C2PA中繼資料的動作

下表根據Marketo Engage影像產生中所執行的影像動作，總結了附加C2PA中繼資料的時間。

| 動作 | 說明 | 要附加C2PA中繼資料嗎？ | 使用案例範例 |
|---|---|---|---|
| **使用[產生影像]工具** | 從文字提示、參照影像建立新影像，或產生類似影像。 | 一律。 影像是由產生式AI產生，因此一律會攜帶最新的C2PA中繼資料。 | 電子郵件促銷活動的橫幅影像是從描述所需視覺效果的文字提示中產生。 |
| **裁切影像** | 將影像調整至要求的尺寸。 | 僅當來源影像已具有C2PA中繼資料時。 裁切會重新建立影像的畫素，通常會擦除C2PA中繼資料，因此Marketo Engage會在裁切前從來源影像讀取該影像，然後重新建置該影像，並將其重新附加至裁切的結果。 裁切本身不會新增創作AI動作，而是保留現有動作。 | 產生的橫幅影像會裁切成適合網頁：透過裁切會保留C2PA中繼資料。 用作推播通知背景的上傳庫存像片會被裁切以適合熒幕：由於庫存像片不執行產生式AI動作，因此不會建立任何C2PA中繼資料。 |
| **新增文字覆蓋** | 在背景影像上方演算產生的文字。 | 僅當背景影像已具有C2PA中繼資料時。 演算覆蓋圖時，會從背景加上文字產生新影像，這通常會清除該C2PA中繼資料，因此Marketo Engage會預先從背景影像讀取該中繼資料，然後重新建置並重新附加至結果。 覆蓋步驟不會新增新產生的AI動作。 | 促銷標題會在登陸頁面產生的背景影像上呈現為文字重疊：背景影像的C2PA中繼資料會保留。 |

## 內容型別及其範圍

**影像**：已涵蓋。 使用產生式AI產生影像時，會附加C2PA中繼資料，並透過在Marketo Engage中由影像產生執行的裁切和文字覆蓋作業來保留。

**文字**：不適用。 在Marketo Engage中產生影像的純文字輸出，例如產生復本、翻譯和品牌對齊建議，不需要C2PA中繼資料。

## 內容移動時發生什麼事

Marketo Engage會保留與支援的影像資產相關聯的C2PA中繼資料。 如果影像在匯入Marketo Engage時包含C2PA中繼資料，則當資產用於產生的行銷活動內容和傳出電子郵件體驗時，會保留中繼資料。

## 其他資源

* [Generative AI內容透明度](https://experienceleague.adobe.com/zh-hant/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency){target="_blank"}
* [Adobe Experience Cloud Generative AI使用者指南](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}
* [護欄與限制](https://experienceleague.adobe.com/zh-hant/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails){target="_blank"}
