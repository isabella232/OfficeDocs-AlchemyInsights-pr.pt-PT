---
title: A sua caixa de correio de arquivo está quase cheia
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974660"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="bb580-102">A sua caixa de correio de arquivo está quase cheia</span><span class="sxs-lookup"><span data-stu-id="bb580-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="bb580-103">Se o utilizador receber o aviso; **A sua caixa de correio de arquivo está quase cheia,** ou precisa de aumentar o tamanho da sua caixa de correio de arquivo, aqui ficam algumas dicas:</span><span class="sxs-lookup"><span data-stu-id="bb580-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="bb580-104">Se o utilizador for designado um Plano Online de Troca 1, atualize para a licença **Exchange Online Plan 2** para aumentar o tamanho de 50 GB para 100GB.</span><span class="sxs-lookup"><span data-stu-id="bb580-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="bb580-105">Se o utilizador já tiver sido atribuído a um dos seguintes: **Exchange Online Plan 2** ou um Exchange Online Plan 1 com um add-on de arquivamento online de intercâmbio, utilize os passos abaixo para permitir o arquivamento de auto-expansão:.</span><span class="sxs-lookup"><span data-stu-id="bb580-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="bb580-106">[Ligue-se a Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="bb580-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="bb580-107">Executar o seguinte comando para o utilizador:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="bb580-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="bb580-108">Executar o seguinte comando para confirmar que está ativado para o utilizador:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="bb580-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="bb580-109">Para mais informações consulte:</span><span class="sxs-lookup"><span data-stu-id="bb580-109">For more information see:</span></span>

- [<span data-ttu-id="bb580-110"> Ativar o arquivamento ilimitado - Ajuda de administração - Microsoft 365 Compliance | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="bb580-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="bb580-111">Trocar limites online - Descrições de Serviços | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="bb580-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="bb580-112">Upgrade para um plano de negócios diferente | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="bb580-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

