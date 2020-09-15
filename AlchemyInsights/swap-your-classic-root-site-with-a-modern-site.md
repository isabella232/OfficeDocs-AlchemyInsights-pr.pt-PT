---
title: Troque o seu site de raiz clássico por um site moderno
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691190"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="80e24-102">Troque o seu site de raiz clássico por um site moderno</span><span class="sxs-lookup"><span data-stu-id="80e24-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="80e24-103">Se o seu ambiente foi configurado antes de abril de 2019, pode alterar o seu site de raiz para um site moderno utilizando o Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="80e24-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="80e24-104">Se tiver um site diferente que pretende utilizar como seu site de raiz, pode substituir [(trocar) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) por ele.</span><span class="sxs-lookup"><span data-stu-id="80e24-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="80e24-105">Utilize [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site por outro site enquanto arquiva o site original.</span><span class="sxs-lookup"><span data-stu-id="80e24-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="80e24-106">Disponível para o Site de Equipa (não ligado a um grupo) e site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="80e24-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="80e24-107">Em breve serão introduzidas capacidades adicionais que lhe permitirão continuar a utilizar o conteúdo do site, mas converter o site existente num site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="80e24-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="80e24-108">Estas capacidades serão lançadas gradualmente.</span><span class="sxs-lookup"><span data-stu-id="80e24-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="80e24-109">Continue a verificar as atualizações do Centro de Mensagens.</span><span class="sxs-lookup"><span data-stu-id="80e24-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="80e24-110">Problemas conhecidos com sites de troca</span><span class="sxs-lookup"><span data-stu-id="80e24-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="80e24-111">O local alvo pode devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="80e24-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="80e24-112">O conteúdo terá de ser recrawlado para atualizar o índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="80e24-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="80e24-113">Não é necessário um passo manual - isto será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="80e24-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="80e24-114">Qualquer coisa dependente de ligações "estáticas" (como ficheiros File Sync e OneNote) terá de ser corrigida manualmente.</span><span class="sxs-lookup"><span data-stu-id="80e24-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="80e24-115">Se o site de origem foi um site de notícias organizacional, atualize o URL.</span><span class="sxs-lookup"><span data-stu-id="80e24-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="80e24-116">Obtenha uma lista de todos os sites de notícias organizacionais.</span><span class="sxs-lookup"><span data-stu-id="80e24-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="80e24-117">Os sites do Project Server podem ter de ser validados para garantir que ainda estão corretamente associados.</span><span class="sxs-lookup"><span data-stu-id="80e24-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
