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
# <a name="your-archive-mailbox-is-almost-full"></a>A sua caixa de correio de arquivo está quase cheia

Se o utilizador receber o aviso; **A sua caixa de correio de arquivo está quase cheia,** ou precisa de aumentar o tamanho da sua caixa de correio de arquivo, aqui ficam algumas dicas:

1. Se o utilizador for designado um Plano Online de Troca 1, atualize para a licença **Exchange Online Plan 2** para aumentar o tamanho de 50 GB para 100GB.
1. Se o utilizador já tiver sido atribuído a um dos seguintes: **Exchange Online Plan 2** ou um Exchange Online Plan 1 com um add-on de arquivamento online de intercâmbio, utilize os passos abaixo para permitir o arquivamento de auto-expansão:.
 
    1. [Ligue-se a Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Executar o seguinte comando para o utilizador:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Executar o seguinte comando para confirmar que está ativado para o utilizador:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Para mais informações consulte:

- [ Ativar o arquivamento ilimitado - Ajuda de administração - Microsoft 365 Compliance | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Trocar limites online - Descrições de Serviços | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade para um plano de negócios diferente | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

