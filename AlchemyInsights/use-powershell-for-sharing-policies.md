---
title: Use PowerShell para partilhar políticas e relações de organização
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862152"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Use PowerShell para partilhar políticas e relações de organização


Para as relações de organização, por favor reveja a sintaxe detalhada e as informações de parâmetros para : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) and [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Para criar política de partilha, utilize [a Nova Política de Partilha.](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) Para [aplicar uma política de partilha a uma caixa de correio ou utilizador,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) é necessário utilizar uma combinação de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) e [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) com a nova política criada. Para [modificar, desativar ou remover uma política](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) de partilha, é necessário utilizar a Política de Partilha de [Conjuntos](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) e [a Política de Partilha de Remoção](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Para uma compreensão completa deste tópico, leia:**

[Partilha em Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)