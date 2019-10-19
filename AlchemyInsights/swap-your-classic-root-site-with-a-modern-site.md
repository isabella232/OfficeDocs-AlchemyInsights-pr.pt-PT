---
title: Troque seu site raiz clássico com um site moderno
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749271"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="77698-102">Troque seu site raiz clássico com um site moderno</span><span class="sxs-lookup"><span data-stu-id="77698-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="77698-103">Se seu ambiente foi configurado antes de abril de 2019, você pode alterar seu site raiz para um site moderno usando o Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="77698-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="77698-104">Se você tiver um site diferente que você deseja usar como seu site raiz, você pode substituir [(swap) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) com ele.</span><span class="sxs-lookup"><span data-stu-id="77698-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="77698-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site com outro site ao arquivar o site original.</span><span class="sxs-lookup"><span data-stu-id="77698-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="77698-106">Disponível para o site de equipe (não conectado a um grupo) e o site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="77698-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="77698-107">Recursos adicionais serão introduzidos em breve que permitirão que você continue usando o conteúdo no site, mas converta o site existente em um site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="77698-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="77698-108">Esses recursos serão lançados gradualmente.</span><span class="sxs-lookup"><span data-stu-id="77698-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="77698-109">Continue a verificar o Office 365 Message Center para obter atualizações.</span><span class="sxs-lookup"><span data-stu-id="77698-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="77698-110">Problemas conhecidos com a troca de sites</span><span class="sxs-lookup"><span data-stu-id="77698-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="77698-111">O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="77698-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="77698-112">O conteúdo precisará ser rastreado para atualizar o índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="77698-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="77698-113">Não há nenhuma etapa manual exigida-isto será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="77698-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="77698-114">Qualquer coisa dependente de links "estáticos" (como arquivos de sincronização de arquivo e OneNote) precisará ser corrigido manualmente.</span><span class="sxs-lookup"><span data-stu-id="77698-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="77698-115">Se o site de origem for um site de notícias organizacionais, atualize a URL.</span><span class="sxs-lookup"><span data-stu-id="77698-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="77698-116">Obtenha uma lista de todos os sites de notícias organizacionais.</span><span class="sxs-lookup"><span data-stu-id="77698-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="77698-117">Sites do Project Server talvez precise ser validado para garantir que eles ainda estão associados corretamente.</span><span class="sxs-lookup"><span data-stu-id="77698-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





