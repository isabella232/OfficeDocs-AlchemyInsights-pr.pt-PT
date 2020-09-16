---
title: Restringir o SharePoint Online ao modo clássico
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751433"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="aed8f-102">Restringir o SharePoint Online ao modo clássico</span><span class="sxs-lookup"><span data-stu-id="aed8f-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="aed8f-103">Algumas organizações ainda requerem a experiência do modo Clássico.</span><span class="sxs-lookup"><span data-stu-id="aed8f-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="aed8f-104">Embora não existam planos para remover o modo clássico a nível granular, já não é possível restringir toda uma organização (inquilino) ao modo clássico para listas e bibliotecas.</span><span class="sxs-lookup"><span data-stu-id="aed8f-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="aed8f-105">O administrador terá as seguintes opções para gerir listas individuais e bibliotecas em modo clássico utilizando interruptores de opt-out granular que fornecemos nos seguintes níveis:</span><span class="sxs-lookup"><span data-stu-id="aed8f-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="aed8f-106">coleção de site</span><span class="sxs-lookup"><span data-stu-id="aed8f-106">site collection</span></span>
- <span data-ttu-id="aed8f-107">site</span><span class="sxs-lookup"><span data-stu-id="aed8f-107">site</span></span>
- <span data-ttu-id="aed8f-108">lista</span><span class="sxs-lookup"><span data-stu-id="aed8f-108">list</span></span>
- <span data-ttu-id="aed8f-109">biblioteca</span><span class="sxs-lookup"><span data-stu-id="aed8f-109">library</span></span>

<span data-ttu-id="aed8f-110">Além disso, as listas que usam certas funcionalidades e personalizações que não são suportadas pelo moderno ainda serão automaticamente mudadas para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="aed8f-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="aed8f-111">A partir de 1 de abril de 2019, o processo de desativação do nível de inquilino opta por sair da lista moderna e as bibliotecas vão começar e continuar até 31 de maio de 2019.</span><span class="sxs-lookup"><span data-stu-id="aed8f-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="aed8f-112">As listas e bibliotecas que estão em modo clássico como resultado do opt-out do inquilino serão automaticamente transferidas para modernas.</span><span class="sxs-lookup"><span data-stu-id="aed8f-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="aed8f-113">Se necessitar de modo clássico, consulte mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instruções PnP Powershell [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descrevem opções e ferramentas que pode usar hoje para usar a experiência clássica do modo.</span><span class="sxs-lookup"><span data-stu-id="aed8f-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
