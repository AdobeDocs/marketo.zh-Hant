---
description: 發行說明 — 2022年3月 — Marketo檔案 — 產品檔案
title: 版本注意事項 - 2022 年 3 月
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 4%

---

# 發行說明：2022 年 3 月 {#release-notes-mar-22}

2022年3月發行版本包含下列功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

**_每季發行_**

下列功能將於&#x200B;**2022年3月11日**&#x200B;開始發行，並在接下來的幾週內分階段推出每個功能（除非另有指定）。

## 跨頻道協調 {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]**：透過主動式、主動式和1:1個人化對話將目標同時鎖定於銷售機會和帳戶，在您的網站上最大化每個商機。 [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}可讓Marketo Engage使用者開始運用聊天，作為B2B行銷和銷售使用案例整合式跨管道體驗的關鍵部分。 功能包括：直接在聊天中預約會議、潛在客戶路由、入門範本、建立拖放式交談等等。 Dynamic Chat包含在所有Marketo Engage套件中，並將於今年推出給所有Marketo Engage使用者。

* **電子郵件機器人活動篩選增強功能**：作為先前發行之[電子郵件機器人活動篩選](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}功能的增強功能，您現在可以選擇加入識別為機器人的記錄活動。 然後，您可以根據識別為機器人正在執行的活動來篩選及觸發動作。

## 次世代體驗 {#modern-ux}

* **新一代體驗中的Screens已更新**：我們為新一代體驗提供額外的重新整理熒幕，透過切換開關提供更新的設計和可用性增強功能：

   * [!UICONTROL Design Studio]中的表單清單檢視（包括新的大量動作）

* **匯入方案工作流程更新**：正在新一代體驗中傳遞匯入方案工作流程，其中包含更新的設計和可用性增強功能。 這將是一個自動變更，不需要切換開關。

* **新一代體驗切換開關的管理員控制**：以適合您的使用者的方式管理新一代體驗的推出，同時管理員能夠選取哪些使用者型別可以存取切換開關。

## 體驗自動化 {#experience-automation}

* **自助服務流程步驟(Beta)**：擴充Marketo Engage與您棧疊其他部分之間的連線，並有能力編寫自訂的流程步驟以用於Smart Campaigns。 Marketo使用者和合作夥伴均可運用此功能，允許在批次和可執行的行銷活動中使用外部Web服務，而非Webhook，後者只能用於觸發行銷活動。

* **資產有效期**：保持對時效性資產和行銷活動的控制，並能夠在傳統使用者體驗中的指定日期和時間排程其自動停用。

* **智慧型行銷活動優先順序覆寫**：確保高優先順序觸發智慧型行銷活動會儘快執行，並有能力覆寫標準行銷活動優先順序排名。 低優先順序觸發器智慧型行銷活動也可以降低優先順序，以釋出處理資源給其他高優先順序的工作。

## API增強功能 {#api-enhancements}

* **傳回停用電子郵件的開啟追蹤狀態**：允許透過API讀取電子郵件的開啟追蹤狀態
* **從電子郵件擷取動態內容主旨列**：可讓行銷人員在BI工具中執行動態主旨列分析
* **方案成員自訂欄位CRUD**：可讓行銷人員以程式設計方式建立方案成員自訂欄位
* **大量自訂物件匯出已更新於Filter**：可讓行銷人員以程式設計方式同步自訂物件
* **公開電子郵件程式的Head Start設定**：可讓行銷人員透過API設定電子郵件程式的Head Start
* **選擇性方案標籤更新**：可讓行銷人員推播選擇性標籤更新，而不需同時推播所有標籤
* **大量活動擷取actionResult欄位**：可讓行銷人員識別哪些活動被略過或失敗

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## [!DNL Bizible] {#bizible}

![（星形）](assets/yellow-star.png)

* **BI範本**： [!DNL Bizible]現在將提供Tableau和Power BI的可下載基礎報告成品和範例報告，以便快速開發針對您特定業務需求量身打造的自訂報告。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **電子郵件連線節流(GA)**：電子郵件連線節流可讓[!DNL Sales Connect]管理員設定使用Gmail或[!DNL Exchange]作為傳遞通道時的電子郵件傳送速率，讓電子郵件傳送給傳遞通道提供者的速率不超過強制的限制。

## 公告 {#announcements}

* **棄用Marketo Sky**：三月起，我們將不再提供Marketo Sky，因為我們的資源著重於提供新一代的使用者體驗。 為了維持目前Marketo Sky專屬功能的存取權，我們將「資產有效期」和「智慧型行銷活動優先順序覆寫」引入傳統體驗。 [按一下這裡](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)瞭解更多資訊。

**_產品發行網路研討會_**

[2022年3月和5月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
