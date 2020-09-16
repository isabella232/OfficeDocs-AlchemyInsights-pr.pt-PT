---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770850"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Trabalhar com PowerShell ou Scripts dentro do Sharepoint Online? Visite os links abaixo para mais informações.
- [Começar com a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Ligue ao SPO PowerShell com a autenticação multifactor (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contém uma biblioteca de comandos PowerShell que lhe permite executar ações de gestão complexas em relação ao SPO.

> [!NOTE]
> - Se tiver problemas de ligação com a concha de gestão SPO, [certifique-se](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) de que atualizou a versão mais recente e tente re importar o módulo utilizando *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Se estiver a tentar executar scripts de modelos de objetos do lado do cliente, terá de ter os [Componentes de Cliente Online do Sharepoint SDK instalados](https://www.microsoft.com/download/details.aspx?id=42038) na sua máquina local.
> - Se tiver problemas em executar scripts a partir de PowerShell, pode considerar executar o PowerShell como administrador e alterar a [Política de Execução](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).