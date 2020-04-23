---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764272"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Trabalhar com powerShell ou Scripts dentro do Sharepoint Online? Visite os links abaixo para mais informações.
- [Começar com a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Ligue-se ao SPO PowerShell com a autenticação multifactor (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Os Padrões e Práticas do SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contém uma biblioteca de comandos PowerShell que lhe permite realizar ações de gestão complexas em relação ao SPO.

> [!NOTE]
> - Se estiver a ter problemas de ligação com a concha de gestão SPO, [certifique-se](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) de que atualizou para a versão mais recente e tente reimportar o módulo utilizando *o "Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Se estiver a tentar executar scripts de modelos de objetos do lado do cliente, terá de ter o [SDK](https://www.microsoft.com/download/details.aspx?id=42038) de Componentes de Cliente Online sharepoint instalado na sua máquina local.
> - Se estiver a ter problemas em executar scripts a partir do PowerShell, talvez deva considerar executar a PowerShell como administrador e alterar a Política de [Execução.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)