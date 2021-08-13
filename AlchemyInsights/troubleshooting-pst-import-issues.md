---
title: Resolução de problemas relacionadas com importação de ficheiros PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972430"
---
# <a name="troubleshooting-pst-import-issues"></a>Resolução de problemas relacionadas com importação de ficheiros PST

- Se estiver a importar dentro do cliente Outlook, consulte Corrigir problemas ao importar um [ficheiro Outlook .pst.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Se estiver a utilizar o Serviço de Importação e estiver com problema, tenha em atenção que cada ficheiro PST que carregar para o Azure Armazenamento sua localização não deverá ter mais de 20 GB. Os ficheiros PST com mais de 20 GB podem afetar o desempenho do processo de importação PST. Para obter mais informações sobre a remoção de tarefas presas, consulte [Problemas que afetam as tarefas de importação de PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Se quiser verificar o estado de uma tarefa de importação específica, utilize [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Para obter detalhes completos sobre o serviço de importação, consulte o resumo da [importação dos ficheiros PST da sua organização.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
