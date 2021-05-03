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
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="d52b6-102">Remoção de tarefas do Serviço de Importação com problemas</span><span class="sxs-lookup"><span data-stu-id="d52b6-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="d52b6-103">Se tiver problemas com a tarefa de Importar serviço com problemas ou falhas, examine e experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d52b6-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="d52b6-104">Reveja o tamanho do ficheiro PST.</span><span class="sxs-lookup"><span data-stu-id="d52b6-104">Review the size of of the PST file.</span></span> <span data-ttu-id="d52b6-105">O tamanho máximo recomendado de um ficheiro PST para importação é de 20 GB.</span><span class="sxs-lookup"><span data-stu-id="d52b6-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="d52b6-106">Se suspeitar que itens ignorados devido a corrupção, execute Scanpst.exe para diagnosticar e corrigir erros em ficheiros PST.</span><span class="sxs-lookup"><span data-stu-id="d52b6-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="d52b6-107">Se vir um erro "MapiExceptionShutoffQuotaExceeded" durante a importação, certifique-se de que a caixa de correio de destino tem capacidade suficiente para importar os ficheiros PST pretendidos.</span><span class="sxs-lookup"><span data-stu-id="d52b6-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="d52b6-108">Para obter mais informações sobre a remoção de problemas relacionados com a importação de tarefas PST, consulte Remoção de problemas com tarefas de [importação PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="d52b6-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="d52b6-109">Para obter informações sobre como corrigir problemas ao importar PSTs para o Outlook, consulte Corrigir problemas ao importar um ficheiro [.pst (Outlook.pst) (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="d52b6-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>