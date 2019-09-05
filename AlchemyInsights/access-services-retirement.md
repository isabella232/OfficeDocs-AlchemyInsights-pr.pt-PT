---
title: Reforma de serviços de acesso
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
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747795"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b8672-102">Reforma de serviços de acesso</span><span class="sxs-lookup"><span data-stu-id="b8672-102">Access services retirement</span></span>

<span data-ttu-id="b8672-103">Tal como foi originalmente anunciadas na MC97576, em Março de 2017 e continuaram a comunicar ao longo do ano passado, serviços de acesso estão a ser retirados do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b8672-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="b8672-104">A fase seguinte no processo será a remoção de bases de dados do Access Web que utilizam listas do SharePoint como seu armazenamento de dados subjacente.</span><span class="sxs-lookup"><span data-stu-id="b8672-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b8672-105">**Isto afecta-me?**</span><span class="sxs-lookup"><span data-stu-id="b8672-105">**How does this affect me?**</span></span>

<span data-ttu-id="b8672-106">Iniciar de 2019 Junho, iremos parar a criação de novas bases de dados do Access no SharePoint Online e encerrar o serviço e as aplicações restantes até de Abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="b8672-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b8672-107">**O que é necessário para preparar para que esta alteração?**</span><span class="sxs-lookup"><span data-stu-id="b8672-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b8672-108">Recomendamos que crie um plano de transição para a bases de dados web de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="b8672-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="b8672-109">Admins pode utilizar o [scanner de aplicação de acesso ao SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário das aplicações de acesso a sites estão a utilizar.</span><span class="sxs-lookup"><span data-stu-id="b8672-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b8672-110">Existem várias formas para migrar dados de bases de dados do Access web:</span><span class="sxs-lookup"><span data-stu-id="b8672-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b8672-111">Importar uma base de dados local do Access (. ACCDB) ou para um ficheiro Excel.</span><span class="sxs-lookup"><span data-stu-id="b8672-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b8672-112">Recomendamos também explorar Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócio sem código para a web e dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="b8672-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>