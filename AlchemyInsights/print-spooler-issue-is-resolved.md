---
title: A questão do spooler de impressão está resolvida
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801852"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="2a18c-102">A questão do spooler de impressão está resolvida</span><span class="sxs-lookup"><span data-stu-id="2a18c-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="2a18c-103">Se o seu dispositivo foi atualizado com o Windows 10  **OS Build 19041.329**, pode ter observado um problema em que determinadas impressoras não conseguem imprimir.</span><span class="sxs-lookup"><span data-stu-id="2a18c-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="2a18c-104">O spooler de impressão pode lançar um erro ou fechar inesperadamente ao tentar imprimir, e nenhuma saída vem da impressora afetada.</span><span class="sxs-lookup"><span data-stu-id="2a18c-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="2a18c-105">Esta questão é resolvida em OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="2a18c-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="2a18c-106">**Investigação em curso**</span><span class="sxs-lookup"><span data-stu-id="2a18c-106">**Ongoing investigation**</span></span>

<span data-ttu-id="2a18c-107">O ficheiro do Serviço de Subsistema da Autoridade de Segurança Local (LSASS)\*\* (Isass.exe) \*\*pode falhar em alguns dispositivos com a mensagem de erro: "Um processo crítico do sistema, C:\WINDOWS\system32\Isass.exe, falhou com o código de estado c0000008.</span><span class="sxs-lookup"><span data-stu-id="2a18c-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="2a18c-108">A máquina deve agora ser reiniciada".</span><span class="sxs-lookup"><span data-stu-id="2a18c-108">The machine must now be restarted".</span></span>  <span data-ttu-id="2a18c-109">**A Microsoft está a trabalhar numa resolução e irá fornecer uma atualização numa próxima versão.**</span><span class="sxs-lookup"><span data-stu-id="2a18c-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="2a18c-110">Para mais informações, consulte [os problemas conhecidos do Windows 10 Version 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)</span><span class="sxs-lookup"><span data-stu-id="2a18c-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>