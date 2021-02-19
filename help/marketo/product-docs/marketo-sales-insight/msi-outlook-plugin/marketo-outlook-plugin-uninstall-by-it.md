---
unique-page-id: 11382829
description: Marketo Outlook外掛程式由IT人員解除安裝- Marketo Docs —— 產品檔案
title: IT人員解除安裝Marketo Outlook外掛程式
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# IT {#marketo-outlook-plugin-uninstall-by-it}解除安裝Marketo Outlook外掛程式

以下是IT人員如何遠端解除安裝Marketo Outlook外掛程式。

以「System（系統）」或具有/x開關的管理用戶帳戶的形式運行以下命令行以卸載。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

若需疑難排解，您可以啟用記錄來建立輸出記錄檔。

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

要指定日誌檔案的位置，可以在命令行中指定檔案路徑。

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>遠端解除安裝外掛程式會強制關閉使用者機器上的Outlook。

如果您要嘗試不同的日誌記錄級別或用戶介面級別，請參閱[ Microsoft的交換機完整清單](https://support.microsoft.com/en-us/kb/227091)。
