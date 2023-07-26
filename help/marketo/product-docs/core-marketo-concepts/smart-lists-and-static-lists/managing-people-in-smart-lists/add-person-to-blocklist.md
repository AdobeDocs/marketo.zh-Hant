---
unique-page-id: 9438139
description: 將人員新增至封鎖清單 — Marketo檔案 — 產品檔案
title: 將個人新增至封鎖清單
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 將個人新增至封鎖清單 {#add-person-to-blocklist}

將人員新增至您的封鎖清單會防止他們收到您的信件。

>[!NOTE]
>
>Marketo正在將產品中的黑名單和白名單等辭彙變更為封鎖名單和允許清單。 在此更新中，您可能會在UI和檔案熒幕擷取畫面中看到舊辭彙，並在檔案文字中看到新辭彙。 若有任何混淆，敬請見諒。

1. [建立新的預設程式](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) 並為其命名 **新增至封鎖清單**.

1. 按一下 **新增** 並選取 **新增本機資產**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. 為清單命名，然後按一下 **建立**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. 將所有人員新增至 **智慧清單** 您想要新增至封鎖清單中。

   >[!NOTE]
   >
   >封鎖清單上的人員不會收到操作電子郵件。

   ![](assets/three-6.png)

1. 按一下 **新增** 並選取 **新增智慧型行銷活動**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. 為命名 **新增智慧型行銷活動**. 按一下 **建立**。

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. 拖放 **智慧清單的成員**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. 選取您剛建立的智慧清單。

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. 拖放 **變更資料值**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. 對於 **流量**，輸入 **區塊已列出** 針對 **屬性** 並設定 **新值** 至 **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. 在 **排程** 索引標籤，選取 **執行一次**.

   ![](assets/ten.png)

1. 選取 **立即執行** 並按一下 **執行**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   好耶！ 這些人將不再收到電子郵件。

   >[!TIP]
   >
   >建立 [觸發智慧行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) 使用 **變更資料值** 替換為 **封鎖清單為true** 適用於未來所有具有可封鎖清單屬性的人。
