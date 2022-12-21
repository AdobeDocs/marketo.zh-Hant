---
unique-page-id: 3571797
description: 第2步（共3步） — 為Marketo建立Salesforce使用者（專業版） — Marketo檔案 — 產品檔案
title: 第2步（共3步） — 建立Marketo的Salesforce使用者（專業人員）
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 4%

---

# 第2步（共3步）:建立Marketo的Salesforce使用者（專業版） {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>[第1步（共3步）:將Marketo欄位添加到Salesforce(Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

在本文中，您將使用Salesforce頁面配置來自訂欄位權限，並建立Marketo-Salesforce同步使用者。

## 設定頁面配置 {#set-page-layouts}

Salesforce Professional使用「頁面配置」設定欄位級輔助功能，而不是使用Salesforce Enterprise/Unlimited的配置檔案。 依照這些步驟操作，Marketo同步使用者便可更新自訂欄位。

1. 類型 **頁面配置** ，而不按 **輸入**，然後按一下 **頁面配置** 在 **銷售機會**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 按一下 **編輯** 在「銷售機會配置」旁邊。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 按一下並拖曳新 **區段** 到頁面配置中。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 輸入&quot;Marketo&quot; **區段名稱** 按一下 **確定**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 按一下並拖曳欄位 **贏取日期** 進入 **Marketo** 區段。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 對下列欄位重複上述步驟：

   * 贏取計畫
   * 贏取方案Id
   * 電子郵件選擇退出
   * 推斷的城市
   * 推斷公司
   * 推斷國家
   * 推斷的大都會區
   * 推斷的電話區碼
   * 推斷的郵遞區號
   * 推斷的州別地區
   * 銷售機會分數
   * 原始反向連結
   * 原始搜尋引擎
   * 原始搜索片語
   * 原始源資訊
   * 原始源類型

   >[!NOTE]
   >
   >這些欄位必須位於頁面版面上，Marketo才能讀/寫這些欄位。

   >[!TIP]
   >
   >向下拖曳至頁面右側，為欄位建立兩欄。 您可以將欄位從一側移至另一側，以平衡欄長度。

1. 按一下 **儲存** 完成添加欄位時。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 對Salesforce重複上述所有步驟 **連絡人頁面配置**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 記得按一下 **儲存** 你用完了 **連絡人頁面配置**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >請確定 **全天事件** 欄位已新增至 **事件頁面配置**.

## 建立同步用戶 {#create-sync-user}

Marketo需要存取Salesforce的憑證。 使用下列步驟建立的專用使用者，最好能完成此操作。

>[!NOTE]
>
>如果貴組織沒有其他Salesforce許可證，則可以使用現有的 **行銷使用者** 和 **系統管理員** 設定檔。

1. 在導覽列中輸入「使用者」，然後按一下 **使用者** 在 **管理使用者**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 按一下 **新用戶**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填寫必填欄位，選取 **用戶許可：Salesforce**，請設定 **設定檔：系統管理員**，檢查 **行銷使用者** 按一下 **儲存**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >請確定您輸入的電子郵件地址有效。 您需要以同步使用者身分登入，才能重設密碼。

太棒了！ 現在您有一個帳戶，Marketo可以用來連線至Salesforce。 我們來吧。

>[!MORELIKETHIS]
>
>[第3步（共3步）:連接Marketo和Salesforce（專業版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
