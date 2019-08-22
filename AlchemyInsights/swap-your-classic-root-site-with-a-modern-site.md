---
title: Trocar o site de raiz Classic com um site Moderno
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501090"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="f5a04-102">Trocar o site de raiz Classic com um site Moderno</span><span class="sxs-lookup"><span data-stu-id="f5a04-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="f5a04-103">Se o ambiente tiver sido configurado antes de Abril de 2019, pode alterar o site de raiz para um site moderno utilizando o Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f5a04-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="f5a04-104">Se tiver um site diferente que pretende utilizar como o site de raiz, pode substituir o site de raiz (comutação) com o mesmo.</span><span class="sxs-lookup"><span data-stu-id="f5a04-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="f5a04-105">Utilize [Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para mudar a localização de um site com outro site ao arquivar o site original.</span><span class="sxs-lookup"><span data-stu-id="f5a04-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="f5a04-106">Disponível para o Site de equipa (não ligado a um grupo) e o Site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="f5a04-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="f5a04-107">Capacidades adicionais serão introduzidas mais rapidamente que lhe permitirá manter, utilizando o conteúdo no site, mas converter o site existente para um site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="f5a04-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="f5a04-108">Estas capacidades serão efectuadas gradualmente.</span><span class="sxs-lookup"><span data-stu-id="f5a04-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="f5a04-109">Continue a verificar o Centro de mensagens do Office 365 para obter actualizações.</span><span class="sxs-lookup"><span data-stu-id="f5a04-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="f5a04-110">Problemas conhecidos relacionados com sites de comutação</span><span class="sxs-lookup"><span data-stu-id="f5a04-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="f5a04-111">O site de destino poderá devolver um erro (HTTP 404) "não foi encontrado" durante um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="f5a04-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="f5a04-112">Conteúdo terá de ser pesquisado novamente para actualizar o índice de procura.</span><span class="sxs-lookup"><span data-stu-id="f5a04-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="f5a04-113">Não existe nenhum manual passo necessário - Isto será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f5a04-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="f5a04-114">Tudo depende de ligações "estáticas" (por exemplo, ficheiros de sincronização de ficheiros e o OneNote), terá de ser corrigidas manualmente.</span><span class="sxs-lookup"><span data-stu-id="f5a04-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="f5a04-115">Se o site de origem era um site de notícias sobre a organização, actualize o URL.</span><span class="sxs-lookup"><span data-stu-id="f5a04-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="f5a04-116">Obter uma lista de todos os sites de notícias sobre a organização.</span><span class="sxs-lookup"><span data-stu-id="f5a04-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="f5a04-117">Sites do Project Server poderão ter de ser validadas para garantir que são ainda associadas correctamente.</span><span class="sxs-lookup"><span data-stu-id="f5a04-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





