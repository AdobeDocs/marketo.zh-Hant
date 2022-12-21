---
unique-page-id: 9438139
description: 將人員新增至封鎖清單 — Marketo檔案 — 產品檔案
title: 將人員添加到封鎖清單
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 將人員添加到封鎖清單 {#add-person-to-blocklist}

將人員添加到您的封鎖清單會阻止他們接收您的通信。

>[!NOTE]
>
>Marketo正在將產品中的黑名單和白名單等詞語變更為封鎖名單和允許清單。 在此更新期間，您可能會在UI和檔案螢幕擷取畫面中看到舊辭彙，並在檔案文字中看到新辭彙。 我們為任何混淆道歉。

1. [建立新的預設程式](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) 然後給它命名 **添加到封鎖名單**.

1. 按一下 **新增** 選取 **新本機資產**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. 為清單命名，然後按一下 **建立**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. 將所有人員添加到 **智慧清單** 要添加到你的封鎖名單。

   >[!NOTE]
   >
   >封鎖名單上的人員將不會收到操作電子郵件。

   ![](assets/three-6.png)

1. 按一下 **新增** 選取 **新智慧型行銷活動**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. 將 **新智慧型行銷活動**. 按一下 **建立**。

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. 拖放 **智慧清單成員**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. 選取您剛建立的智慧清單。

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. 拖放 **變更資料值**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. 若 **流量**，輸入 **列出的塊** 針對 **屬性** 設定 **新值** to **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. 在 **排程** 索引標籤，選取 **執行一次**.

   ![](assets/ten.png)

1. 選擇 **立即運行** 按一下 **執行**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   耶！ 這些人將不再收到電子郵件。

   >[!TIP]
   >
   >建立 [觸發智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) 使用 **變更資料值** with **列出的塊為true** 適用於未來具有可封鎖清單屬性的所有人。
