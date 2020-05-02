---
title: Resolução de problemas relacionadas com importação de ficheiros PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991377"
---
# <a name="troubleshooting-pst-import-issues"></a>Resolução de problemas relacionadas com importação de ficheiros PST

- Se estiver a importar no próprio cliente do Outlook, consulte [Corrigir problemas ao importar um ficheiro .pst do Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Se estiver a utilizar o Serviço de Importação e este não responder, note que cada ficheiro PST que carregar para a localização de Armazenamento do Azure não deve exceder 20 GB. Os ficheiros PST superiores a 20 GB poderão ter um impacto no desempenho do processo de importação de ficheiros PST.

- Se pretender verificar o estado de uma tarefa de importação específica, pode utilizar [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Para mais informações sobre o serviço de importação, consulte [Descrição geral da importação dos ficheiros PST da sua organização](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
