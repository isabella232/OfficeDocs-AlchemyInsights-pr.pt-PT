---
title: Troque o seu site de raiz clássico com um site moderno
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741555"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="77399-102">Troque o seu site de raiz clássico com um site moderno</span><span class="sxs-lookup"><span data-stu-id="77399-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="77399-103">Se o seu ambiente foi criado antes de abril de 2019, pode mudar o seu site de raiz para um site moderno usando o Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="77399-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="77399-104">Se tiver um site diferente que deseja utilizar como site raiz, pode substituir [(trocar) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) por ele.</span><span class="sxs-lookup"><span data-stu-id="77399-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="77399-105">Utilize o [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site por outro site enquanto arquiva o site original.</span><span class="sxs-lookup"><span data-stu-id="77399-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="77399-106">Disponível tanto para o Site da Equipa (não ligado a um grupo) como para o Site de Comunicação.</span><span class="sxs-lookup"><span data-stu-id="77399-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="77399-107">Em breve serão introduzidas capacidades adicionais que lhe permitirão continuar a utilizar o conteúdo no site, mas converter o site existente num site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="77399-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="77399-108">Estas capacidades serão lançadas gradualmente.</span><span class="sxs-lookup"><span data-stu-id="77399-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="77399-109">Continue a verificar se o Centro de Mensagens está a ver se há novidades.</span><span class="sxs-lookup"><span data-stu-id="77399-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="77399-110">Questões conhecidas com sites de troca</span><span class="sxs-lookup"><span data-stu-id="77399-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="77399-111">O local-alvo pode devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="77399-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="77399-112">O conteúdo terá de ser reescrito para atualizar o índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="77399-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="77399-113">Não é necessário um passo manual - isto será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="77399-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="77399-114">Qualquer coisa dependente de links "estáticos" (como ficheiros Sync e OneNote) terá de ser corrigido manualmente.</span><span class="sxs-lookup"><span data-stu-id="77399-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="77399-115">Se o site de origem fosse um site de notícias organizacional, atualize o URL.</span><span class="sxs-lookup"><span data-stu-id="77399-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="77399-116">Obtenha uma lista de todos os sites de notícias organizacionais.</span><span class="sxs-lookup"><span data-stu-id="77399-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="77399-117">Os sites do Project Server podem ter de ser validados para garantir que ainda estão corretamente associados.</span><span class="sxs-lookup"><span data-stu-id="77399-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
