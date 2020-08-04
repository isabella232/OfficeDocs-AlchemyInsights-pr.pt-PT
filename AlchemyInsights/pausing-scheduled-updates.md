---
title: Pausas agendadas atualizações
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555515"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="2fa12-102">Pausas agendadas atualizações</span><span class="sxs-lookup"><span data-stu-id="2fa12-102">Pausing scheduled updates</span></span>

<span data-ttu-id="2fa12-103">Quando um comando de pausa é emitido, os dispositivos não processam o comando até à próxima vez que fizerem o check-in no Intune.</span><span class="sxs-lookup"><span data-stu-id="2fa12-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="2fa12-104">Por causa disto, os seus dispositivos podem ter:</span><span class="sxs-lookup"><span data-stu-id="2fa12-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="2fa12-105">Instalou as atualizações programadas antes do check-in.</span><span class="sxs-lookup"><span data-stu-id="2fa12-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="2fa12-106">Foi desligado quando emite o comando de pausa.</span><span class="sxs-lookup"><span data-stu-id="2fa12-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="2fa12-107">Neste caso, quando os dispositivos foram ligados, podem ter descarregado e instalado as atualizações programadas antes do check-in.</span><span class="sxs-lookup"><span data-stu-id="2fa12-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>