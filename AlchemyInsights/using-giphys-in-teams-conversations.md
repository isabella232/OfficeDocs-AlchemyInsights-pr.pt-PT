---
title: Usando Giphys em conversas de equipas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982581"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="87221-102">Usando Giphys em conversas de equipas</span><span class="sxs-lookup"><span data-stu-id="87221-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="87221-103">O acesso de Giphys no chat de Equipas é ativado por padrão.</span><span class="sxs-lookup"><span data-stu-id="87221-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="87221-104">Como administrador, pode controlar se o Giphys estiver disponível para os [utilizadores, definindo uma política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) e garantindo que **o Uso de Giphys nas conversas** é **On**.</span><span class="sxs-lookup"><span data-stu-id="87221-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="87221-105">Se os GIFs não estiverem a funcionar como esperado nas conversas das equipas, verifique:</span><span class="sxs-lookup"><span data-stu-id="87221-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="87221-106">A [política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) tem de permitir o Giphys.</span><span class="sxs-lookup"><span data-stu-id="87221-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="87221-107">Para verificar utilizando cmdlets PowerShell:</span><span class="sxs-lookup"><span data-stu-id="87221-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="87221-108">Verifique se consegue [gerir equipas com PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="87221-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="87221-109">Executar o comando PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verificar se **AllowGiphy** está definido para **TRUE**.</span><span class="sxs-lookup"><span data-stu-id="87221-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="87221-110">Se **o AllowGiphy** estiver definido como **FALSE,** executar o seguinte comando PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="87221-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="87221-111">[As experiências conectadas opcionais](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) devem ser ativadas para permitir o acesso ao URL giphy.</span><span class="sxs-lookup"><span data-stu-id="87221-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="87221-112">Se tiver várias políticas de mensagens de equipas configuradas para o seu inquilino, pode determinar a identidade da política atribuída ao utilizador impactado com o comando PowerShell [Get-CsOnlineUser -Identidade](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> ; Selecione TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="87221-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
