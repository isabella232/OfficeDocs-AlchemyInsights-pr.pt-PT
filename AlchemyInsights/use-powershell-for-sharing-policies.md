---
title: Utilizar o PowerShell para Partilhar políticas e relações da Organização
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998478"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Utilizar o PowerShell para Partilhar políticas e relações da Organização


Para relações da Organização, consulte a sintaxe detalhada e informação sobre parâmetros para : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  E  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Para criar uma política de partilha, utilize [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Para  [aplicar uma política de partilha a uma caixa de correio ou utilizador](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  tem de utilizar uma combinação de  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) e [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) com a política recém-criada. Para  [modificar, desativar ou remover uma política de partilha](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  tem de utilizar  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) e [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Para compreender este tópico de forma aprofundada, consulte:**

[Partilhar no Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)