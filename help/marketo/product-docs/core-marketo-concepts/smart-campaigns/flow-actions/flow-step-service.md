---
description: 流程步驟服務 — Marketo檔案 — 產品檔案
title: 流程步驟服務
exl-id: 81367562-8b27-4ec5-8a9b-b02083a2e999
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1224'
ht-degree: 0%

---

# 流程步驟服務 {#flow-step-service}

自助服務流程步驟是用於編寫、發佈和將Web服務整合到Adobe Marketo Engage Smart Campaigns中的框架和功能集。 本指南適用於想要安裝及使用已建立和發佈之服務的Marketo Engage使用者。 如需製作和發佈您自己的服務的資訊，請參閱服務提供者介面[[!DNL GitHub] 的](https://github.com/adobe/Marketo-SSFS-Service-Provider-Interface){target="_blank"}存放庫。 您可以在[這裡](https://github.com/adobe/mkto-flow-lookup){target="_blank"}找到概念證明查閱表格實作。

## 入門和管理服務 {#onboarding-and-managing-services}

安裝自訂流程步驟需要Marketo中的管理員許可權。 除了安裝URL之外，服務的所有其他方面都可以在完成初始上線後進行編輯，方法是從「服務提供者」格線向下切入服務詳細資訊畫面。

## 安裝URL {#installation-url}

若要開始安裝，您必須先取得定義您服務的OpenAPI檔案的URL。 您的服務提供者應該能夠提供此資訊給您，而且通常會有以`/openapi.json`結尾的URL。 完整的URL看起來會類似`https://www.example.com/OpenAPI.json`。 有了此URL後，請移至[!UICONTROL Service Providers]區段中的[!UICONTROL Admin]功能表。

按一下&#x200B;**[!UICONTROL Next]**，移至「輸入服務認證」區段。

![](assets/flow-step-service-1.png)

## 輸入服務認證 {#enter-service-credentials}

若要存取正在安裝的服務，Marketo必須具備有效的API認證。 您的服務提供者應提供這些認證。 服務有三個不同的驗證選項，因此您可能會看到認證的三個不同提示之一： **API金鑰** （只有一個輸入欄位）、**基本驗證** （需要使用者名稱和密碼，也可能需要名為「領域」的欄位）和&#x200B;**OAuth2** （使用&#x200B;_使用者端認證_&#x200B;授權，需要&#x200B;_使用者端識別碼_&#x200B;和&#x200B;_使用者端密碼_）。

儲存認證時，Marketo會嘗試呼叫服務的狀態端點，以驗證其是否有效。 如果提供的認證無效，您將會看到指出此問題的錯誤。

>[!CAUTION]
>
>如果建立並刪除服務提供者，以後將無法重複使用其服務提供者、API、觸發程式或篩選器名稱。

## 入門指南（選用） {#onboarding-guide}

有些服務供應商會包含選用的入門指南步驟。 此步驟將包含特定於該服務的任何其他完成服務上線的指示。

## 欄位對應 {#field-mapping}

為了從特定銷售機會欄位接收或傳回資料，該欄位必須對應。 雖然在入門期間必須執行對應步驟，但您稍後可能一律會回過頭來變更對應。 在不同畫面中設定了兩種對應： **傳出欄位** (當Marketo叫用流程步驟時傳送至服務)和&#x200B;**傳入欄位** (當服務傳回資料至Marketo時可能從服務接收資料的欄位)。

>[!NOTE]
>
>對應傳出欄位即表示您授予Marketo許可權，可傳輸該欄位中與由相關服務處理之潛在客戶相關的資料。 請確保您擁有適當的法律地位和授權，可以將這些資料傳輸至您的服務提供者，因為這些欄位可能包含資料隱私權、保護及租賃法律所涵蓋的個人識別資訊。

可以在不中斷服務的情況下停用選擇性欄位對應，但可能不會完全移除或停用必要的對應。

## 服務導向對應 {#service-driven-mappings}

具有固定輸入和輸出集的服務（如事件註冊流程步驟）使用&#x200B;**服務導向的對應**。 對於這類對應，服務提供者會以API名稱的形式提供資料型別和提示。 如果提示符合現有潛在客戶欄位的API名稱，則該欄位會自動填入對應區段。 對於沒有相符提示的欄位，您將需要從具有相符資料型別的欄位清單中手動填入對應。 必須填入必要的對應才能完成上線。

![](assets/flow-step-service-2.png)

## 使用者導向對應 {#user-driven-mappings}

沒有固定輸入和輸出集的服務（如日期格式服務）使用&#x200B;**使用者導向對應**。 這表示每個傳入和傳出欄位都必須由管理員設定。

![](assets/flow-step-service-3.png)

## 傳出欄位 {#outgoing-fields}

傳出欄位是在智慧行銷活動中使用該流程步驟時傳送到「流程步驟服務」的欄位。

## 傳入欄位 {#incoming-fields}

傳入欄位是允許「流程步驟服務」將資料寫入其中的欄位。

## 組態選項（選擇性） {#configuration-options}

有些服務有選擇性的或必要的全域組態選項。 如果需要任何選項，則在儲存或完成入門之前，必須為所有需要的選項設定值。 名稱為斜體的引數會以標頭的形式傳送至叫用的服務。

![](assets/flow-step-service-4.png)

## 棄用服務 {#retiring-a-service}

為了在不中斷使用中的情況下加速轉換至新的或替代服務版本，服務提供者選單中的服務可以淘汰。 **棄用服務**&#x200B;會從Smart Campaign流量調色盤移除對應的流量步驟，因此無法建立其新的使用方式。 在大多數情況下，當您選擇淘汰服務時，應該有可取代現有服務的替代服務。

## 服務淘汰 {#service-deprecation}

有時服務提供者需要淘汰流程步驟服務，做為軟體生命週期的正常部分。 當服務提供者宣佈此專案時，「停用日期」和「訊息」將會填入「服務提供者」格線檢視中。 如果繼續使用已過時的服務，不再以預期的方式回應，或停止接受來自Marketo Smart Campaigns的請求，則可能會導致服務中斷，因此您應該密切注意您收到的任何服務過時的通知，並採取適當的步驟來停用或取代仍在使用中的服務中的任何步驟。

## 使用協力廠商和自訂流量步驟 {#using-third-party-and-custom-flow-steps}

已安裝的流程步驟的使用方式與標準流程步驟大致相同。 由服務定義的所有流程引數都會呈現給一般使用者。

## 重新整理挑選清單 {#refreshing-picklists}

Marketo會每晚重新整理服務的挑選清單選擇，但有時您需要新的可用選擇，例如建立行銷活動。 您可以使用重新整理按鈕，從流程步驟的任何執行個體輕鬆重新整理這些內容，或前往「[!UICONTROL Admin] > [!UICONTROL Service Providers]」功能表，並在選取服務後按一下「[!UICONTROL Refresh Picklist]」。

## 檢查傳入欄位 {#checking-incoming-fields}

您可以透過將游標移至其工具提示圖示上，來檢查為指定流程步驟設定的傳入欄位。 這對於判斷潛在客戶流經哪些欄位可能會變更非常有用，因此您可以使用這些欄位在後續步驟中設定選擇。

![](assets/flow-step-service-5.png)

## 傳入欄位和資料值變更 {#incoming-fields-and-data-value-changes}

與大多數其他流程步驟不同，以SSFS架構實作的步驟可能會將資料寫回由管理員對應的潛在客戶欄位，並將這些變更記錄為資料值變更活動。  當流程步驟以這種方式寫入資料時，在Smart Campaign繼續進行任何後續步驟之前，將完成所有這些變更，以便在後續的流程步驟選擇中可以依賴所寫入的任何資料。

## 服務記錄檔與統計資料 {#service-logs-and-statistics}

每個「流程步驟服務」都有數種相關的記錄，可協助監控健全狀態，並疑難排解與整合相關的任何問題。

## 服務統計資料 {#service-statistics}

「服務」統計記錄會彙總每個服務的呼叫與回呼結果。 它們依時間、層級（區塊或記錄）和程式碼分組，並提供計數和每個收到之程式碼的最新記錄訊息。 此儀表板的主要設計用途是協助監控服務健康狀態。
