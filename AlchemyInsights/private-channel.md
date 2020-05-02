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
# <a name="private-channels-in-microsoft-teams"></a>Canais privados em Microsoft Teams

Canais privados é uma nova funcionalidade nas Equipas microsoft. Note que os canais privados não podem ser convertidos a partir de canais padrão ou vice-versa.

Para mais detalhes sobre canais privados, tais como informações sobre [a criação e adesão de canais privados](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) e [sites de private channel SharePoint,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)consulte [canais privados em Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Nota:** Como a configuração para a retenção de mensagens de canal privado ainda não é suportada, os inquilinos com políticas de retenção ativadas não terão canais privados habilitados por padrão. Os canais privados podem ser ativados no centro de administração das Equipas. Além disso, note que, embora a retenção de mensagens de canal privado não seja suportada, a retenção de ficheiros partilhados em canais privados é suportada.

**Precisa de um novo dono de equipa?**

Se o seu dono de canal privado sair, pode adicionar um novo dono de equipa através da Teams Powershell.


- Vá [aqui](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) para instalar as Equipas Powershell.

Aqui está o cmdlet que você vai precisar:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Para obter mais informações sobre as equipas Powershell, consulte a visão geral da [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
