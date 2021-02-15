---
unique-page-id: 11382815
description: IT人員安裝Marketo Outlook外掛程式- Marketo Docs —— 產品檔案
title: IT部門安裝Marketo Outlook外掛程式
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---


# IT {#marketo-outlook-plugin-installation-by-it}安裝Marketo Outlook外掛程式

有時公司政策要求其IT團隊在員工的電腦上安裝所有軟體。 在這些情況下，IT部門通常使用自己的部署軟體遠程執行此操作。 本文檔提供在部署過程中用作輸入的命令行，以遠程安裝Outlook插件。

>[!PREREQUISITES]
>
>[設定](https://docs.marketo.com/display/DOCS/Install+the+Marketo+Add-in+for+Outlook+with+an+Enterprise+Key) 企業金鑰。

以「System」（系統）或具有要安裝的/i開關的管理用戶帳戶形式運行以下命令行。 `<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

若需疑難排解，您可以啟用記錄來建立輸出記錄檔。 `<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

要指定日誌檔案的位置，可以在命令行中指定檔案路徑。 `<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>日誌檔案的儲存位置必須存在，否則安裝將中止。

如果您要嘗試不同的日誌記錄級別或用戶介面級別，請參閱[ Microsoft的交換機完整清單](https://support.microsoft.com/en-us/kb/227091)。

>[!MORELIKETHIS]
>
>[IT人員解除安裝Marketo Outlook外掛程式](marketo-outlook-plugin-uninstall-by-it.md)

