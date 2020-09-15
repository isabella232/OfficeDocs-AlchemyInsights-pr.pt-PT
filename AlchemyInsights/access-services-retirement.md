---
title: Aposentadoria de serviços de acesso
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698693"
---
# <a name="access-services-retirement"></a><span data-ttu-id="ee8b9-102">Aposentadoria de serviços de acesso</span><span class="sxs-lookup"><span data-stu-id="ee8b9-102">Access services retirement</span></span>

<span data-ttu-id="ee8b9-103">Como inicialmente anunciado no MC97576, em março de 2017, e continuamos a comunicar ao longo do ano passado, os Serviços de Acesso estão a ser reformados.</span><span class="sxs-lookup"><span data-stu-id="ee8b9-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="ee8b9-104">A próxima fase deste processo será a remoção de Bases de Dados Web de Acesso que utilizam as listas do SharePoint como o seu armazenamento de dados subjacente.</span><span class="sxs-lookup"><span data-stu-id="ee8b9-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="ee8b9-105">**Como é que isto me afeta?**</span><span class="sxs-lookup"><span data-stu-id="ee8b9-105">**How does this affect me?**</span></span>

<span data-ttu-id="ee8b9-106">A partir de junho de 2019, vamos parar a criação de novas bases de dados de Acesso no SharePoint Online e encerrar o serviço e quaisquer aplicações restantes até abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="ee8b9-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="ee8b9-107">**O que preciso de fazer para me preparar para esta mudança?**</span><span class="sxs-lookup"><span data-stu-id="ee8b9-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="ee8b9-108">Encorajamo-lo a criar um plano de transição para as bases de dados web access da sua organização.</span><span class="sxs-lookup"><span data-stu-id="ee8b9-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="ee8b9-109">Os administradores podem usar o scanner de [aplicações SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário das aplicações Access que os sites estão a usar.</span><span class="sxs-lookup"><span data-stu-id="ee8b9-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="ee8b9-110">Existem várias formas de migrar os dados das bases de dados do Access Web:</span><span class="sxs-lookup"><span data-stu-id="ee8b9-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="ee8b9-111">Importando para uma base de dados de acesso local (. ACCDB) ou para um ficheiro Excel.</span><span class="sxs-lookup"><span data-stu-id="ee8b9-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="ee8b9-112">Recomendamos também explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócio sem código para dispositivos web e móveis.</span><span class="sxs-lookup"><span data-stu-id="ee8b9-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>