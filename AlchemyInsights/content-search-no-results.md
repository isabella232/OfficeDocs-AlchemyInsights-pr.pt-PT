---
title: Não existem resultados de pesquisa de conteúdo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516790"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="31ce4-102">Não existem resultados de conteúdo procura/exportações</span><span class="sxs-lookup"><span data-stu-id="31ce4-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="31ce4-103">Problemas com conteúdo procura/exportações não devolver quaisquer dados podem ser devido a certas filtro de segurança de conformidade que foi configurado por um administrador específico e não a comunicar a todos os Admins.</span><span class="sxs-lookup"><span data-stu-id="31ce4-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="31ce4-104">Para resolver este problema, verifique se existem quaisquer filtros de segurança de conformidade que poderá estar a causar este:</span><span class="sxs-lookup"><span data-stu-id="31ce4-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="31ce4-105">Ligar a segurança e conformidade Centro Powershell</span><span class="sxs-lookup"><span data-stu-id="31ce4-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="31ce4-106">Execute o commandlets do seguinte:</span><span class="sxs-lookup"><span data-stu-id="31ce4-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="31ce4-107">$org = "seudomínio. com"</span><span class="sxs-lookup"><span data-stu-id="31ce4-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="31ce4-108">Get-ComplianceSecurityFilter-$org de organização</span><span class="sxs-lookup"><span data-stu-id="31ce4-108">Get-ComplianceSecurityFilter -Organization $org</span></span>