---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786900"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="e712a-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="e712a-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="e712a-103">Trabalhar com PowerShell ou Scripts dentro do Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="e712a-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="e712a-104">Visite os links abaixo para mais informações.</span><span class="sxs-lookup"><span data-stu-id="e712a-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="e712a-105">Começar com a SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="e712a-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="e712a-106">Ligue ao SPO PowerShell com a autenticação multifactor (MFA)</span><span class="sxs-lookup"><span data-stu-id="e712a-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="e712a-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contém uma biblioteca de comandos PowerShell que lhe permite executar ações de gestão complexas em relação ao SPO.</span><span class="sxs-lookup"><span data-stu-id="e712a-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="e712a-108">Se tiver problemas de ligação com a concha de gestão SPO, [certifique-se](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) de que atualizou a versão mais recente e tente re importar o módulo utilizando *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="e712a-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="e712a-109">Se estiver a tentar executar scripts de modelos de objetos do lado do cliente, terá de ter os [Componentes de Cliente Online do Sharepoint SDK instalados](https://www.microsoft.com/download/details.aspx?id=42038) na sua máquina local.</span><span class="sxs-lookup"><span data-stu-id="e712a-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="e712a-110">Se tiver problemas em executar scripts a partir de PowerShell, pode considerar executar o PowerShell como administrador e alterar a [Política de Execução](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="e712a-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>