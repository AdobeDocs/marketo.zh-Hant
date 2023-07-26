---
unique-page-id: 10096681
description: 瞭解網路研討會計畫狀態 — Marketo檔案 — 產品檔案
title: 瞭解網路研討會計畫狀態
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 瞭解網路研討會計畫狀態 {#understanding-webinar-program-statuses}

方案狀態代表個人作為事件成員所處理的不同事件狀態。 它們與管道型別相關聯。 Marketo有一個內建的管道型別，稱為 **網路研討會**. 狀態可用於批次和觸發行銷活動。

人們以線性方式在計畫狀態中移動，而不會回到狀態。 例如，某人擁有 **已出席** 無法移回到 **已註冊**.

以下為與網路研討會頻道相關之計畫狀態的簡短說明。

>[!TIP]
>
>若要手動更新狀態，請按一下  **從網路研討會提供者重新整理** 在 **事件動作** 下拉式清單。

![](assets/image2015-12-17-13-3a52-3a39.png)

**不在計畫中**  — 使用此狀態從事件中移除人員。

**已邀請**  — 使用此狀態來將人員新增至事件。

**未決核准**  — 使用此狀態可延遲傳送確認電子郵件給您的人員。 請參閱以下主題中的「手動核准註冊者」： [ON24事件註冊更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} 以取得詳細資訊。

**等待已列出**  — 使用此狀態可讓部分人等待，直到有額外的座位可用。

**已拒絕**  — 使用此狀態來拒絕人員註冊您的事件。

**已註冊**  — 當您使用ON24整合時，此狀態會將人員推送到ON24。 當ON24回應人員已成功註冊時，人員狀態會更新。

**註冊錯誤**  — 此狀態反映使用者嘗試註冊事件時發生錯誤。

>[!NOTE]
>
>如果發生註冊錯誤，您可以檢視計畫「成員」標籤中的「狀態原因」欄，以取得該人員的其他資訊。 修正錯誤後，您可以手動將使用者的程式狀態變更為已在Marketo中註冊。

**已出席**  — 網路研討會結束時，ON24會傳回出席者清單。 系統會自動將此狀態提取至Marketo。

**已出席隨選**  — 參加封存版網路研討會的人員會收到此狀態。

**無節目**  — 網路研討會結束時，當出席資料從ON24提取後，已註冊但未出席者的狀態會更新為「沒有顯示」。 ON24可能需要花費30分鐘到3小時的時間，以準備最終出席資訊，並在Marketo中提供。

>[!NOTE]
>
>為了讓Marketo能夠提取「不顯示」狀態，人員必須已註冊 *在Marketo中*. 我們無法擷取來自On24資料摘要的「沒有節目」。

>[!MORELIKETHIS]
>
>[瞭解Marketo ON24介面卡事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
