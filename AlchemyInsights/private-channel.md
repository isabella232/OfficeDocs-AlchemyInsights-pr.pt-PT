---
title: Canal privado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005449"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="0dd0c-102">Canais privados em Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0dd0c-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="0dd0c-103">Canais privados é uma nova funcionalidade nas Equipas microsoft.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="0dd0c-104">Note que os canais privados não podem ser convertidos a partir de canais padrão ou vice-versa.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="0dd0c-105">Para mais detalhes sobre canais privados, tais como informações sobre [a criação e adesão de canais privados](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) e [sites de private channel SharePoint,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)consulte [canais privados em Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="0dd0c-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="0dd0c-106">**Nota:** Como a configuração para a retenção de mensagens de canal privado ainda não é suportada, os inquilinos com políticas de retenção ativadas não terão canais privados habilitados por padrão.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="0dd0c-107">Os canais privados podem ser ativados no centro de administração das Equipas.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="0dd0c-108">Além disso, note que, embora a retenção de mensagens de canal privado não seja suportada, a retenção de ficheiros partilhados em canais privados é suportada.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="0dd0c-109">**Precisa de um novo dono de equipa?**</span><span class="sxs-lookup"><span data-stu-id="0dd0c-109">**Need a new team owner?**</span></span>

<span data-ttu-id="0dd0c-110">Se o seu dono de canal privado sair, pode adicionar um novo dono de equipa através da Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="0dd0c-111">Vá [aqui](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) para instalar as Equipas Powershell.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="0dd0c-112">Aqui está o cmdlet que você vai precisar:</span><span class="sxs-lookup"><span data-stu-id="0dd0c-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="0dd0c-113">Para obter mais informações sobre as equipas Powershell, consulte a visão geral da [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="0dd0c-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
