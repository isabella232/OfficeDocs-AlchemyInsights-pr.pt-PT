---
title: Aposentadoria dos serviços de acesso
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747795"
---
# <a name="access-services-retirement"></a><span data-ttu-id="66cae-102">Aposentadoria dos serviços de acesso</span><span class="sxs-lookup"><span data-stu-id="66cae-102">Access services retirement</span></span>

<span data-ttu-id="66cae-103">Como anunciamos originalmente em MC97576, em março de 2017, e continuamos a se comunicar no ano passado, os Serviços de Acesso estão sendo aposentados do Office 365.</span><span class="sxs-lookup"><span data-stu-id="66cae-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="66cae-104">A próxima fase desse processo será a remoção dos bancos de dados da Access Web que usam as listas do SharePoint como armazenamento de dados subjacente.</span><span class="sxs-lookup"><span data-stu-id="66cae-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="66cae-105">**Como isso me afeta?**</span><span class="sxs-lookup"><span data-stu-id="66cae-105">**How does this affect me?**</span></span>

<span data-ttu-id="66cae-106">A partir de junho de 2019, vamos parar a criação de novos bancos de dados de acesso no SharePoint Online e encerrar o serviço e quaisquer aplicativos restantes até abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="66cae-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="66cae-107">**O que preciso fazer para me preparar para essa mudança?**</span><span class="sxs-lookup"><span data-stu-id="66cae-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="66cae-108">Nós encorajamos você a criar um plano de transição para os bancos de dados da web Access da sua organização.</span><span class="sxs-lookup"><span data-stu-id="66cae-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="66cae-109">Os administradores podem usar o scanner de [aplicativos SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário dos aplicativos de acesso que os sites estão usando.</span><span class="sxs-lookup"><span data-stu-id="66cae-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="66cae-110">Existem várias maneiras de migrar dados de bancos de dados da web access:</span><span class="sxs-lookup"><span data-stu-id="66cae-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="66cae-111">Importação para um banco de dados de acesso local (. ACCDB) ou para um arquivo Excel.</span><span class="sxs-lookup"><span data-stu-id="66cae-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="66cae-112">Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócios sem código para dispositivos web e móveis.</span><span class="sxs-lookup"><span data-stu-id="66cae-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>