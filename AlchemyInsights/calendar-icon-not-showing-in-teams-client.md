---
title: O ícone do Calendário não é apresentado no cliente do Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932198"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="84b00-102">O ícone do Calendário não é apresentado no cliente do Teams</span><span class="sxs-lookup"><span data-stu-id="84b00-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="84b00-103">O separador Calendário no Teams necessita de acesso a uma caixa de correio do Exchange através dos Serviços Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="84b00-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="84b00-104">A caixa de correio do Exchange pode estar Online ou No Local.</span><span class="sxs-lookup"><span data-stu-id="84b00-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="84b00-105">Para utilizadores Online que não vejam o separador Calendário, certifique-se de que [têm licença para uma caixa de correio Exchange Online e que a caixa de correio está ativada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="84b00-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="84b00-106">Se o utilizador tiver uma caixa de correio válida no Exchange Online, mas ainda não conseguir ver o separador Calendário, poderá estar a ter um problema de rede.</span><span class="sxs-lookup"><span data-stu-id="84b00-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="84b00-107">Utilize o [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) e execute os **Testes de Conectividade dos Serviços Web do Microsoft Exchange** para o utilizador afetado.</span><span class="sxs-lookup"><span data-stu-id="84b00-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="84b00-108">Por último, consulte as [Políticas de configuração de aplicações nas Aplicações do Teams](https://admin.teams.microsoft.com/policies/app-setup) para garantir que a aplicação Calendário não foi removida da política aplicada ao utilizador (provavelmente a **Global (predefinição da organização)**.</span><span class="sxs-lookup"><span data-stu-id="84b00-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="84b00-109">Se os seus utilizadores estiverem alojados No Local, precisa de confirmar que a sua Configuração híbrida tem bom estado de funcionamento.</span><span class="sxs-lookup"><span data-stu-id="84b00-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="84b00-110">Utilize o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para resolver problemas.</span><span class="sxs-lookup"><span data-stu-id="84b00-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="84b00-111">Tenha em conta que o [Teams necessita do Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="84b00-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
