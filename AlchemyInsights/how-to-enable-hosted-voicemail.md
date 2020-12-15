---
title: Como ativar o Correio de Voz hospedado
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679169"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="56181-102">Como ativar o Correio de Voz hospedado</span><span class="sxs-lookup"><span data-stu-id="56181-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="56181-103">Para ativar o Correio de Voz, **o HostedVoicemail** tem de ser definido para $true.</span><span class="sxs-lookup"><span data-stu-id="56181-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="56181-104">A propriedade **HostedVoicemail** no utilizador utilizando Remote PowerShell (RPS).</span><span class="sxs-lookup"><span data-stu-id="56181-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="56181-105">Para obter mais informações sobre a ligação ao RPS, consulte a [Visão Geral powershell das equipas da Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre a ligação ao RPS.</span><span class="sxs-lookup"><span data-stu-id="56181-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="56181-106">O Administrador das Equipas deve ser registado no Remote PowerShell para equipas.</span><span class="sxs-lookup"><span data-stu-id="56181-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="56181-107">A partir do PowerShell, o Teams Admin pode executar **set-csuser user@contoso.com -HostedVoiceMail $true** onde o sip uri é do utilizador em questão.</span><span class="sxs-lookup"><span data-stu-id="56181-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="56181-108">As alterações às políticas podem demorar até 24 horas a replicar-se.</span><span class="sxs-lookup"><span data-stu-id="56181-108">Changes to policies can take up to 24 hours to replicate.</span></span>