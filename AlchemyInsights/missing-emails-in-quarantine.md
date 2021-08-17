---
title: E-mails em falta na quarentena
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892058"
---
# <a name="missing-emails-in-quarantine"></a>E-mails em falta na quarentena

Os [administradores podem ver, libertar ou eliminar estas mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

No portal Microsoft 365 Defender, em <https://security.microsoft.com> , vá para Rever  \> **Quarentena**. Ou, para ir diretamente para a página **Quarentena,** utilize <https://security.microsoft.com/quarantine> .  

Para obter mais informações sobre os valores de pesquisa/filtro que pode utilizar, consulte Gerir mensagens e [ficheiros em quarentena](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)como um administrador na EOP.

Os cmdlets que utiliza para ver e gerir mensagens e ficheiros na quarentena são:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pré-visualização-QuarentenaMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): tenha em atenção que este cmdlet é apenas para mensagens e não para ficheiros do Cofre Anexos do SharePoint, OneDrive ou Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
