---
unique-page-id: 10096681
description: 了解網路研討會計畫狀態 — Marketo檔案 — 產品檔案
title: 了解網路研討會計畫狀態
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 了解網路研討會計畫狀態 {#understanding-webinar-program-statuses}

方案狀態代表人員作為事件成員進行的不同事件狀態。 它們與管道類型相關聯。 Marketo的內建管道類型稱為 **網路研討會**. 狀態可用於批次和觸發促銷活動。

人們會以線性方式移動程式狀態，而不會回到狀態。 例如，狀態為 **已出席** 無法移回 **已註冊**.

以下是與網路研討會頻道相關聯之節目狀態的簡短說明。

>[!TIP]
>
>若要手動更新狀態，請按一下  **從網路研討會提供者重新整理** 在 **事件動作** 下拉式清單。

![](assets/image2015-12-17-13-3a52-3a39.png)

**不在程式中**  — 使用此狀態可從事件中移除人員。

**受邀**  — 使用此狀態將人員添加到事件中。

**待批准**  — 使用此狀態可延遲向您的人員發送確認電子郵件。 請參閱以下主題中的「手動核准註冊者」： [ON24事件註冊更新](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target=&quot;_blank&quot;}以取得詳細資訊。

**已列出等待**  — 使用此狀態讓一些人等待，直到其他座位可用。

**已拒絕**  — 使用此狀態拒絕將人員註冊到您的事件。

**已註冊**  — 當您使用ON24整合時，此狀態會將人員推送至ON24。 當ON24回應人員已成功註冊時，會更新該人員的狀態。

**註冊錯誤**  — 此狀態反映使用者嘗試註冊事件時遇到錯誤。

>[!NOTE]
>
>如果發生註冊錯誤，您可以查看方案的「成員」頁簽中的「狀態原因」列，以獲取該人員的其他資訊。 修正錯誤後，您可以手動將使用者的程式狀態變更為「已在Marketo中註冊」。

**已出席**  — 網路研討會結束時，ON24會返回參加者的清單。 此狀態會自動提取至Marketo。

**隨選出席**  — 參加網路研討會封存版本的人會獲得此狀態。

**無顯示**  — 網路研討會結束時，從ON24提取出席資料後，註冊但未參加的人的狀態將更新為「無節目」。 ON24可能需要30分鐘到3小時，才能準備最終的出席資訊並在Marketo中提供。

>[!NOTE]
>
>若要讓Marketo提取「無顯示」狀態，人員必須已註冊 *在Marketo*. 無法擷取來自On24資料摘要的「否顯示」。

>[!MORELIKETHIS]
>
>[了解Marketo ON24適配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}
