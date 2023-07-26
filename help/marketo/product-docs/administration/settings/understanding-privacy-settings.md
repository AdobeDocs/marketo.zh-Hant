---
unique-page-id: 10617187
description: 瞭解隱私設定 — Marketo檔案 — 產品檔案
title: 瞭解隱私權設定
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 瞭解隱私權設定 {#understanding-privacy-settings}

## 概觀 {#overview}

Marketo為行銷人員提供了取得網頁訪客同意追蹤他們的方法。 有兩種方式選擇退出，或者您可以選擇由匿名化IP追蹤。

* 網站訪客在其瀏覽器中選取「不要追蹤」(DNT)功能（行銷人員會接受網站訪客的「不要追蹤」請求）
* 網站訪客使用行銷人員在網站上提供的選擇退出Cookie

或者，行銷人員可以追蹤使用者，但使用匿名化的IP。

這些方法可能會影響Marketo在特定區域中的價值和功能。 但是，如果行銷人員 _不會_ 變更Marketo設定中的任何專案，Marketo功能會維持不變。

## Do Not Track的瀏覽器設定 {#browser-settings-for-do-not-track}

網站訪客可以選擇「不要追蹤」(DNT)，設定瀏覽器以防止任何網站進行追蹤。 這會防止追蹤此特定瀏覽器和裝置。 如需完整詳細資料，請參閱瀏覽器的隱私權設定。

在 [!DNL Munchkin]，行銷人員可以 [決定是否支援或忽略瀏覽器的DNT設定](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

在Web Personalization中，行銷人員可以決定是否要 [支援或忽略瀏覽器的DNT設定](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## 選擇退出特定網站 {#opt-out-from-a-specific-website}

您也可以允許網站訪客選擇退出您網站的網站追蹤，無論是否允許 **瀏覽器不追蹤** 設定已設定。 這可讓網站訪客直接從您的網站指定其追蹤偏好設定。

若要這麼做，您必須在具有下列專案的網頁上，將引數新增至選擇退出連結： [!DNL Munchkin] 已啟用追蹤。 這可以是任何網頁，但網頁連結必須包含以下引數：

？marketo_opt_out=true

以下是含有選擇退出連結的網頁範例，以及按一下連結後適用的登陸頁面。 您的會有所不同。

以下是網頁，其中包含在選擇退出連結中包含「？marketo_opt_out=true」引數的按鈕。

![](assets/understanding-privacy-settings-1.png)

您可以建立並發佈登入頁面，作為您與「？marketo_opt_out=true」引數連結被點按時的後續追蹤頁面。

![](assets/understanding-privacy-settings-2.png)

點按連結時，Marketo會新增名為的Cookie **mkto_opt_out** 至訪客的瀏覽器以停用 [!DNL Munchkin] 追蹤使用上述引數點按連結的網站訪客。

若要驗證是否可以植入Cookie，請確認您是Cookie潛在客戶，然後按一下連結。 然後檢查您的瀏覽器Cookie，以確認 **mkto_opt_out** 已新增Cookie。

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>目前僅適用於 [!DNL Munchkin] 版本152及更高版本。

## 選擇加入 {#opt-in}

行銷人員可在電子郵件、表單、登入頁面和其他方法中使用Marketo的功能，讓使用者選擇加入。

## 使用匿名化IP進行追蹤 {#tracking-using-an-anonymized-ip}

行銷人員可使用匿名化的IP位址追蹤使用者，以保留隱私權。 要執行此操作，請將此程式碼新增到RTP或 [!DNL Munchkin] 內嵌在網站中的Javascript。

* 的 [!DNL Munchkin]，只需將{&quot;anonymizeIP&quot;，true}新增至init函式。

  >[!NOTE]
  >
  >使用此引數需要 [!DNL Munchkin] V2已啟用。 若要為您的訂閱啟用此功能，請聯絡 [Marketo支援](https://nation.marketo.com/community/support_solutions).

* 針對Web Personalization (RTP)，請將此專案新增至javascript：

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
