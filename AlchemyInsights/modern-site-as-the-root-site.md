---
title: Local moderno como o local de raiz
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713802"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="aee36-102">Local moderno como local de raiz</span><span class="sxs-lookup"><span data-stu-id="aee36-102">Modern site as root site</span></span>

<span data-ttu-id="aee36-103">Começamos a lançar uma nova funcionalidade que lhe permitirá [trocar o seu site clássico com um site moderno.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="aee36-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="aee36-104">Utilize o [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site por outro site enquanto arquiva o site original.</span><span class="sxs-lookup"><span data-stu-id="aee36-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="aee36-105">Disponível tanto para o Site da Equipa (não ligado a um grupo) como para o Site de Comunicação.</span><span class="sxs-lookup"><span data-stu-id="aee36-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="aee36-106">Não elimine o seu site de raiz clássico para criar um site de comunicação moderno.</span><span class="sxs-lookup"><span data-stu-id="aee36-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="aee36-107">Isto não é suportado pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="aee36-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="aee36-108">A eliminação do site raiz tornará inacessíveis todos os sites do SharePoint na sua organização a todos os utilizadores, até que restaure o site ou crie um novo site no mesmo URL.</span><span class="sxs-lookup"><span data-stu-id="aee36-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="aee36-109">Vamos comunicar esta funcionalidade através do centro de mensagens.</span><span class="sxs-lookup"><span data-stu-id="aee36-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="aee36-110">Deve esperar que a funcionalidade seja ligada no seu inquilino em breve.</span><span class="sxs-lookup"><span data-stu-id="aee36-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="aee36-111">Questões conhecidas com sites de troca</span><span class="sxs-lookup"><span data-stu-id="aee36-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="aee36-112">O local-alvo pode devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="aee36-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="aee36-113">O conteúdo terá de ser reescrito para atualizar o índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="aee36-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="aee36-114">Não é necessário um passo manual aqui, isto será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="aee36-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="aee36-115">Qualquer coisa dependente de links "estáticos" (como ficheiros Sync e OneNote) terá de ser corrigido manualmente.</span><span class="sxs-lookup"><span data-stu-id="aee36-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="aee36-116">Os sites do Project Server podem ter de ser validados para garantir que ainda estão corretamente associados.</span><span class="sxs-lookup"><span data-stu-id="aee36-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
