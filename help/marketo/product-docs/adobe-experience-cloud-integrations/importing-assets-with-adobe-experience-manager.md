---
unique-page-id: 37355768
description: 使用Adobe Experience Manager匯入資產 — Marketo檔案 — 產品檔案
title: 使用Adobe Experience Manager匯入資產
exl-id: 56ccf38f-3c99-4018-9989-719854e37a20
source-git-commit: c396c205d3cececc752f9b563c0d2ab41ff92b6a
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 使用Adobe Experience Manager匯入資產 {#importing-assets-with-adobe-experience-manager}

「資產選擇器」可讓Marketo客戶存取、選取AEM資產，並將其匯入Marketo的Design Studio。 **需要管理員權限**.

>[!AVAILABILITY]
>
>並非所有客戶都購買過此功能。 如需詳細資訊，請連絡您的客戶成功經理。

>[!PREREQUISITES]
>
>請確定您已執行 [AEM設定](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/configuring-adobe-experience-manager-integration.md).

>[!IMPORTANT]
>
>目前，此功能僅完全支援Firefox。 Safari不支援，且視您的SameSite Cookie設定而定，在最新版Chrome中可能無法運作。

1. 按一下 **Design Studio**.

   ![](assets/one-1.png)

1. 按一下「新增」下拉式清單，然後選取 **從Adobe Experience Manager匯入**.

   ![](assets/two-1.png)

1. 選擇要將影像保存到的資料夾。

   ![](assets/three-1.png)

1. 登入Adobe Experience Manager（如果尚未登入）。

   ![](assets/four-1.png)

1. 選擇您的資料夾。 然後按一下縮圖以選取您想要的影像（您最多可以選擇10個）。 按一下 **選擇** 時才能使用。

   ![](assets/five.png)

   >[!NOTE]
   >
   >影像大小不能超過100MB。

1. 按一下 **匯入** 來完成此程式。

   ![](assets/six-1.png)

   就這樣！ 按一下 **關閉** 返回Design Studio。

   ![](assets/seven-1.png)

## 注意事項 {#things-to-note}

* Marketo目前支援Adobe Experience Manager 6.4和6.5版。

* 您執行個體中的所有使用者都能檢視/存取您匯入的影像。

* 影像不會自動更新。 如果您匯入Marketo Design Studio的影像在AEM中更新，您必須手動將其重新匯入Marketo。
