---
title: Site moderna, tal como o site de raiz
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543864"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="376be-102">Moderno site como site de raiz</span><span class="sxs-lookup"><span data-stu-id="376be-102">Modern site as root site</span></span>

<span data-ttu-id="376be-103">Vamos ter começado a fase de instalação uma nova funcionalidade que permite-lhe trocar o site de raiz clássico de site com um site Moderno.</span><span class="sxs-lookup"><span data-stu-id="376be-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="376be-104">Utilize [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para mudar a localização de um site com outro site ao arquivar o site original.</span><span class="sxs-lookup"><span data-stu-id="376be-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="376be-105">Disponível para o Site de equipa (não ligado a um grupo) e o Site de comunicação.</span><span class="sxs-lookup"><span data-stu-id="376be-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="376be-106">Não elimine o site de raiz clássico para criar um Site de comunicação modernos.</span><span class="sxs-lookup"><span data-stu-id="376be-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="376be-107">Não é suportada pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="376be-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="376be-108">Eliminar o site de raiz fará com que todos os sites SharePoint da sua organização inacessíveis a todos os utilizadores, até que restaure o site ou crie um novo site com o mesmo URL.</span><span class="sxs-lookup"><span data-stu-id="376be-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="376be-109">A Microsoft vai estar a comunicar esta funcionalidade através do Centro de mensagem.</span><span class="sxs-lookup"><span data-stu-id="376be-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="376be-110">Deve esperar a funcionalidade para ser activado no seu tenant dentro em breve.</span><span class="sxs-lookup"><span data-stu-id="376be-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="376be-111">Problemas conhecidos relacionados com sites de comutação</span><span class="sxs-lookup"><span data-stu-id="376be-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="376be-112">O site de destino poderá devolver um erro (HTTP 404) "não foi encontrado" durante um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="376be-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="376be-113">Conteúdo terá de ser pesquisado novamente para actualizar o índice de procura.</span><span class="sxs-lookup"><span data-stu-id="376be-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="376be-114">Não existe nenhum passo manual necessário aqui, isto será feito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="376be-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="376be-115">Tudo depende de ligações "estáticas" (por exemplo, ficheiros de sincronização de ficheiros e o OneNote), terá de ser corrigidas manualmente.</span><span class="sxs-lookup"><span data-stu-id="376be-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="376be-116">Sites do Project Server poderão ter de ser validadas para garantir que são ainda associadas correctamente.</span><span class="sxs-lookup"><span data-stu-id="376be-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
