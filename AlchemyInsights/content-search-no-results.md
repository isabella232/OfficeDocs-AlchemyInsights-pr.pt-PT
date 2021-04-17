---
title: Pesquisa de conteúdo Sem Resultados
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816859"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="b327a-102">Sem resultados de Pesquisa/Exportações de Conteúdos</span><span class="sxs-lookup"><span data-stu-id="b327a-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="b327a-103">Problemas com a Pesquisa/Exportações de Conteúdo que não devolvam quaisquer dados podem dever-se a um certo Filtro de Segurança de Conformidade que foi configurado por um Administrador específico e não os comunicando a todos os Administradores.</span><span class="sxs-lookup"><span data-stu-id="b327a-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="b327a-104">Para resolver isto, verifique se existem filtros de segurança de conformidade que possam estar a causar isto:</span><span class="sxs-lookup"><span data-stu-id="b327a-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="b327a-105">Ligue-se ao Centro de Segurança e Conformidade Powershell</span><span class="sxs-lookup"><span data-stu-id="b327a-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="b327a-106">Executar os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="b327a-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="b327a-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="b327a-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="b327a-108">Get-ComplianceSecurityFilter -Organização $org</span><span class="sxs-lookup"><span data-stu-id="b327a-108">Get-ComplianceSecurityFilter -Organization $org</span></span>