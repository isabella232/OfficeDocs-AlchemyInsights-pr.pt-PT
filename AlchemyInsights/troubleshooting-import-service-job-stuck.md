---
title: Remoção de tarefas do Serviço de Importação com problemas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125490"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Remoção de tarefas do Serviço de Importação com problemas

Se tiver problemas com a tarefa de Importar serviço com problemas ou falhas, examine e experimente o seguinte:

- Reveja o tamanho do ficheiro PST. O tamanho máximo recomendado de um ficheiro PST para importação é de 20 GB.

- Se suspeitar que itens ignorados devido a corrupção, execute Scanpst.exe para diagnosticar e corrigir erros em ficheiros PST.

- Se vir um erro "MapiExceptionShutoffQuotaExceeded" durante a importação, certifique-se de que a caixa de correio de destino tem capacidade suficiente para importar os ficheiros PST pretendidos.

Para obter mais informações sobre a remoção de problemas relacionados com a importação de tarefas PST, consulte Remoção de problemas com tarefas de [importação PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

Para obter informações sobre como corrigir problemas ao importar PSTs para o Outlook, consulte Corrigir problemas ao importar um ficheiro [.pst (Outlook.pst) (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)