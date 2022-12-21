---
unique-page-id: 10617187
description: 了解隱私權設定 — Marketo檔案 — 產品檔案
title: 了解隱私權設定
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# 了解隱私權設定 {#understanding-privacy-settings}

## 總覽 {#overview}

Marketo可讓行銷人員取得網站訪客追蹤同意的方式。 有兩種方式可選擇退出，或者您可以選擇由匿名IP追蹤。

* 網頁訪客在瀏覽器中選取「不追蹤」(DNT)功能（行銷人員會接受網頁訪客的「不追蹤」請求）
* 網站訪客使用網站上之行銷人員提供的選擇退出Cookie

或者，行銷人員可以追蹤使用者，但使用匿名的IP。

這些方法可能會影響Marketo在特定領域的值和功能。 但若行銷人員 *does&#39;t* 變更Marketo設定中的任何項目時，Marketo功能會維持不變。

## 不追蹤的瀏覽器設定 {#browser-settings-for-do-not-track}

網站訪客可以選擇「不追蹤」(DNT)來設定其瀏覽器，以防止任何網站進行追蹤。 這會防止追蹤此特定瀏覽器和裝置。 如需完整詳細資訊，請參閱瀏覽器的隱私權設定。

在Munchkin中，行銷人員可以 [決定是否支援或忽略瀏覽器的DNT設定](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

在網頁個人化中，行銷人員可以決定 [支援或忽略瀏覽器的DNT設定](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## 選擇退出特定網站 {#opt-out-from-a-specific-website}

您也可以允許網站訪客選擇退出您的網站追蹤，無論是否 **瀏覽器未追蹤** 設定。 這可讓網站訪客直接從您的網站指定其追蹤偏好設定。

若要這麼做，您必須將參數新增至已啟用市政追蹤之網頁上的選擇退出連結。 這可以是任何網頁，但網頁連結必須包含下列參數：

?marketo_opt_out=true

以下範例為具有退出連結的網頁，以及點按連結後的登陸頁面。 你的會有所不同。

這是一個網頁，其中在選擇退出連結中帶有「？marketo_opt_out=true」參數的按鈕。

![](assets/opt-out-1.png)

您可以建立並發佈登錄頁面，作為點按您具有&quot;?marketo_opt_out=true&quot;參數的連結時的後續頁面。

![](assets/opt-out-2.png)

按一下連結時，Marketo會新增以下的Cookie: **mkto_opt_out** 瀏覽器，此瀏覽器會針對使用上述參數點按連結的網站訪客，停用Munchkin追蹤。

若要驗證Cookie是否可以種植，請確認您是Cookie銷售線索，然後按一下連結。 然後檢查您的瀏覽器Cookie，確認 **mkto_opt_out** 已新增cookie。

![](assets/opt-out-3.png)

>[!NOTE]
>
>目前僅適用於Munchkin 152及更新版本。

## 選擇加入 {#opt-in}

行銷人員可在電子郵件、表單、登錄頁面和其他方法中使用Marketo的功能，讓使用者能夠選擇加入。

## 使用匿名IP進行追蹤 {#tracking-using-an-anonymized-ip}

行銷人員可使用匿名的IP位址追蹤使用者，以保留隱私。 若要這麼做，請將此程式碼新增至內嵌於網站中的RTP或Munchkin Javascript。

* 若為Munchkin，只需將{&quot;anonymizeIP&quot;,true}新增至init函式即可。

   >[!NOTE]
   >
   >使用此參數需要啟用Munchkin V2。 若要啟用訂閱功能，請聯絡 [Marketo支援](https://nation.marketo.com/community/support_solutions).

* 若為網頁個人化(RTP)，請將此項目新增至javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
