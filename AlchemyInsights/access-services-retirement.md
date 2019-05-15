---
title: Reforma de serviços de acesso
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973940"
---
# <a name="access-services-retirement"></a><span data-ttu-id="c961a-102">Reforma de serviços de acesso</span><span class="sxs-lookup"><span data-stu-id="c961a-102">Access services retirement</span></span>

<span data-ttu-id="c961a-103">Tal como foi originalmente anunciadas na MC97576, em Março de 2017 e continuaram a comunicar ao longo do ano passado, serviços de acesso estão a ser retirados do Office 365.</span><span class="sxs-lookup"><span data-stu-id="c961a-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="c961a-104">A fase seguinte no processo será a remoção de bases de dados do Access Web que utilizam listas do SharePoint como seu armazenamento de dados subjacente.</span><span class="sxs-lookup"><span data-stu-id="c961a-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="c961a-105">Isto afecta-me?</span><span class="sxs-lookup"><span data-stu-id="c961a-105">How does this affect me?</span></span>

<span data-ttu-id="c961a-106">Iniciar de 2019 Junho, iremos parar a criação de novas bases de dados do Access no SharePoint Online e encerrar o serviço e as aplicações restantes até de Abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="c961a-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="c961a-107">O que é necessário para preparar para que esta alteração?</span><span class="sxs-lookup"><span data-stu-id="c961a-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="c961a-108">Recomendamos que crie um plano de transição para a bases de dados web de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c961a-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="c961a-109">Admins pode utilizar o [scanner de aplicação de acesso ao SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) para obter um inventário das aplicações de acesso a sites estão a utilizar.</span><span class="sxs-lookup"><span data-stu-id="c961a-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="c961a-110">Existem várias formas para migrar dados de bases de dados do Access web:</span><span class="sxs-lookup"><span data-stu-id="c961a-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="c961a-111">Importar uma base de dados local do Access (. ACCDB) ou para um ficheiro Excel.</span><span class="sxs-lookup"><span data-stu-id="c961a-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="c961a-112">Recomendamos também explorar Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócio sem código para a web e dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="c961a-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>