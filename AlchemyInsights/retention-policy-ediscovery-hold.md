---
title: 2609-retenção ou ediscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994086"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="a84d7-102">Incapaz de excluir itens no SharePoint Online ou OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="a84d7-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="a84d7-103">Você ou seus usuários podem não poder excluir itens no SharePoint Online ou no OneDrive for Business porque uma política de retenção, rótulo de retenção ou retenção de eDiscovery é aplicada a um site Do Ponto de Compartilhamento do OneDrive ou a um item específico.</span><span class="sxs-lookup"><span data-stu-id="a84d7-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="a84d7-104">Isso inclui ser incapaz de excluir um documento, uma versão de documento, uma pasta, uma biblioteca de documentos, uma lista, um aplicativo, um site ou uma coleção de sites.</span><span class="sxs-lookup"><span data-stu-id="a84d7-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="a84d7-105">Aqui estão alguns exemplos das mensagens de erro que você pode receber se você tentar excluir um item que está sendo mantido:</span><span class="sxs-lookup"><span data-stu-id="a84d7-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="a84d7-106">"Este site não pode ser excluído porque está incluído em uma política de retenção ou retenção do eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="a84d7-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="a84d7-107">"Este site tem uma política de conformidade definida para bloquear a exclusão"</span><span class="sxs-lookup"><span data-stu-id="a84d7-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="a84d7-108">"Uma política de conformidade está bloqueando essa exclusão do site"</span><span class="sxs-lookup"><span data-stu-id="a84d7-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="a84d7-109">"Esta coleção do site não pode ser excluída porque contém sites que estão incluídos em uma política de retenção ou retenção do eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="a84d7-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="a84d7-110">"Você tem que excluir todos os itens nesta pasta antes de excluir a pasta"</span><span class="sxs-lookup"><span data-stu-id="a84d7-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="a84d7-111">"As versões deste item não podem ser excluídas porque ele está em espera ou na política de retenção"</span><span class="sxs-lookup"><span data-stu-id="a84d7-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="a84d7-112">"Item não pode ser excluído enquanto estiver em espera"</span><span class="sxs-lookup"><span data-stu-id="a84d7-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="a84d7-113">"O rótulo que é aplicado a este item impede que ele seja editado ou excluído"</span><span class="sxs-lookup"><span data-stu-id="a84d7-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="a84d7-114">"A lista não pode ser excluída enquanto estiver em espera ou na política de retenção"</span><span class="sxs-lookup"><span data-stu-id="a84d7-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="a84d7-115">"A lista não pode ser excluída se for bloqueada ou se uma política de retenção for aplicada a ela"</span><span class="sxs-lookup"><span data-stu-id="a84d7-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="a84d7-116">Para excluir itens em um desses cenários, a política de retenção, o rótulo de retenção ou a retenção do eDiscovery precisa ser removido (ou um site precisa ser excluído de uma política de retenção).</span><span class="sxs-lookup"><span data-stu-id="a84d7-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="a84d7-117">Você precisa desativar ou excluir a respectiva espera que está causando esse problema.</span><span class="sxs-lookup"><span data-stu-id="a84d7-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="a84d7-118">Depois que uma política ou uma retenção de retenção forem removidas, pode levar até 24 horas para que a alteração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="a84d7-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="a84d7-119">Para obter informações sobre os diferentes recursos de retenção e retenção que podem ser aplicados em sites do SharePoint e contas OneDrive, consulte um dos seguintes tópicos.</span><span class="sxs-lookup"><span data-stu-id="a84d7-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="a84d7-120">Visão geral das políticas de retenção</span><span class="sxs-lookup"><span data-stu-id="a84d7-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="a84d7-121">Visão geral dos rótulos de retenção</span><span class="sxs-lookup"><span data-stu-id="a84d7-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="a84d7-122">Gerenciar detém em advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="a84d7-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="a84d7-123">eDiscovery detém</span><span class="sxs-lookup"><span data-stu-id="a84d7-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="a84d7-124">Políticas de fechamento e exclusão de sites legados</span><span class="sxs-lookup"><span data-stu-id="a84d7-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
