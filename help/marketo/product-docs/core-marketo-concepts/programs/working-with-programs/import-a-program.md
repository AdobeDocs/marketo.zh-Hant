---
unique-page-id: 1147108
description: 匯入計畫 — Marketo檔案 — 產品檔案
title: 匯入計畫
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 匯入計畫 {#import-a-program}

程式可從一個Marketo訂閱匯入到另一個訂閱。 例如，您可以在沙箱中建立計畫，然後將其匯入您的即時訂閱中。 此外，您也可以從Marketo方案庫匯入預先建立的方案。

## 匯入方案 {#importing-a-program}

1. 前往 **行銷活動。**

   ![](assets/import-a-program-1.png)

1. 按一下 **新增** 下拉式清單。 選取 **匯入計畫**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >「程式匯入」僅適用於已啟用「匯入程式」許可權之角色的使用者。 進一步瞭解 [管理使用者角色和許可權](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >若要將沙箱帳戶連線至您的即時訂閱，請連絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).

1. 選取Marketo **訂閱** 以及要匯入的方案。 按一下 **下一個**.

   ![](assets/import-a-program-3.png)

1. 指定 **行銷活動資料夾** 適用於匯入的方案。 按一下 **下一個。**

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >確定 **使用預設衝突** 已選取規則。 當您將方案匯入具有相同名稱資產的執行個體時，需要使用衝突規則。

1. 選擇您需要的衝突詳細資料，然後按一下 **下一個**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >將使用「自訂流程步驟」或「智慧列示」規則（衍生自「流程步驟服務」）的程式匯入目的地執行處理（其中有一個以上的相容服務提供者），將會提示匯入使用者將步驟或規則指派給目的地執行處理中的正確服務提供者。

1. 預覽詳細資料和 **匯入** 程式。

   ![](assets/import-a-program-6.png)

匯入完成後，您將會收到電子郵件確認。

>[!NOTE]
>
>您需要重新排程匯入的批次行銷活動，並啟動觸發行銷活動。 系統會自動停用行銷活動排程，並觸發匯入方案中的行銷活動。

## 程式匯入期間對外部資產的影響 {#impact-on-external-assets-during-program-imports}

程式會使用外部資產，例如電子郵件範本、登陸頁面範本、影像、表單、權杖和程式標籤。 您可以設定如何處理登入頁面範本和方案標籤，而Marketo會自動管理其餘專案。

**電子郵件/登入頁面範本：** 電子郵件/登陸頁面範本會匯入至Design Studio。 您可以使用衝突規則來設定相同名稱的範本存在時的行為。 使用預設規則時，如果存在具有相同名稱的數字，則會將數字附加至範本。 例如，如果您已有名為「標準範本」的範本，則新範本將命名為「標準範本 — 1」。

**登陸頁面/Forms：** 如果Design Studio中存在同名的表單或登陸頁面，仍會匯入這些表單或登陸頁面，但會在名稱后面附加一個數字（例如：登陸頁面 — 1）。

**影像：** 登入頁面使用的影像會匯入設計工作室，除非有相同名稱的影像存在。

**Token：** 在匯入程式期間，程式外部的權杖會轉換為本機權杖。

>[!CAUTION]
>
>影像型別我的權杖不支援程式匯入。 如果我的權杖有影像型別的程式已匯入， **否** Token將通過。

**程式標籤：** 您可以使用衝突規則來控制如何處理目的地帳戶中不存在的程式標籤。 使用預設規則將會建立程式標籤，或者您可以選擇忽略標籤。

>[!CAUTION]
>
>匯入方案時，包含下列內容的電子郵件/登入頁面 [動態內容](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) 將被跳過。
