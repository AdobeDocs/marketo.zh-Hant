---
unique-page-id: 11382829
description: Marketo [!DNL Outlook] Plugin Uninstall by IT - Marketo檔案 — 產品檔案
title: Marketo [!DNL Outlook] 外掛程式由IT解除安裝
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 2%

---

# Marketo [!DNL Outlook]外掛程式由IT解除安裝 {#marketo-outlook-plugin-uninstall-by-it}

以下是IT如何從遠端解除安裝Marketo [!DNL Outlook]外掛程式。

以&#39;System&#39;的身分執行以下命令列，或以/x引數的[系統管理]使用者帳戶執行解除安裝。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

若要進行疑難排解，您可以啟用記錄以建立輸出記錄檔。

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

若要指定日誌檔的位置，您可以在命令列中指定檔案路徑。

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>從遠端解除安裝外掛程式將會強制關閉使用者電腦上的[!DNL Outlook]。

如果您想要嘗試不同的記錄層級或使用者介面層級，請參閱[Microsoft的完整交換器清單](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6)。
