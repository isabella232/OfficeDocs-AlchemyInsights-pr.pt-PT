---
title: Nenhum resultado devolvido durante a Pesquisa/Exportação de Conteúdos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727234"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="d8b4e-102">Nenhum resultado devolvido durante a Pesquisa/Exportação de Conteúdos</span><span class="sxs-lookup"><span data-stu-id="d8b4e-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="d8b4e-103">Se estiver a ter problemas com os seguintes cenários eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="d8b4e-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="d8b4e-104">Pesquisa/Exportação de conteúdos não devolve dados ou dados inesperados</span><span class="sxs-lookup"><span data-stu-id="d8b4e-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="d8b4e-105">falha na pesquisa ou exportação de eDiscovery</span><span class="sxs-lookup"><span data-stu-id="d8b4e-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="d8b4e-106">Isto pode dever-se a certos filtros de segurança de conformidade que foram configurados por um administrador específico e não foram comunicados a todos os Administradores.</span><span class="sxs-lookup"><span data-stu-id="d8b4e-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="d8b4e-107">Para resolver isto, verifique se existem filtros de segurança de conformidade que possam estar a causar estes problemas:</span><span class="sxs-lookup"><span data-stu-id="d8b4e-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="d8b4e-108">Ligue-se ao Centro de Segurança e Conformidade Powershell</span><span class="sxs-lookup"><span data-stu-id="d8b4e-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="d8b4e-109">Executar os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d8b4e-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="d8b4e-110">Para obter informações adicionais sobre filtros de segurança de conformidade, consulte [permissões de filtragem para pesquisa de conteúdo](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="d8b4e-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
