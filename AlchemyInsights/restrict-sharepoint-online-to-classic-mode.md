---
title: Restringir sharepoint on-line para o modo clássico
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048771"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="8cdc0-102">Restringir sharepoint on-line para o modo clássico</span><span class="sxs-lookup"><span data-stu-id="8cdc0-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="8cdc0-103">Algumas organizações ainda exigem a experiência do modo Clássico.</span><span class="sxs-lookup"><span data-stu-id="8cdc0-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="8cdc0-104">Embora não existam planos para remover o modo clássico em um nível granular, não é mais possível restringir toda uma organização (inquilino) ao modo clássico para listas e bibliotecas.</span><span class="sxs-lookup"><span data-stu-id="8cdc0-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="8cdc0-105">O administrador terá as seguintes opções para gerenciar listas individuais e bibliotecas no modo clássico usando interruptores de opt-out granulares que fornecemos nos seguintes níveis:</span><span class="sxs-lookup"><span data-stu-id="8cdc0-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="8cdc0-106">coleção do site</span><span class="sxs-lookup"><span data-stu-id="8cdc0-106">site collection</span></span>
- <span data-ttu-id="8cdc0-107">Site</span><span class="sxs-lookup"><span data-stu-id="8cdc0-107">site</span></span>
- <span data-ttu-id="8cdc0-108">Lista</span><span class="sxs-lookup"><span data-stu-id="8cdc0-108">list</span></span>
- <span data-ttu-id="8cdc0-109">Biblioteca</span><span class="sxs-lookup"><span data-stu-id="8cdc0-109">library</span></span>

<span data-ttu-id="8cdc0-110">Além disso, as listas que usam determinados recursos e personalizações que não são suportadas pelo moderno ainda serão automaticamente alteradas para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="8cdc0-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="8cdc0-111">A partir de 1º de abril de 2019, o processo para desativar o nível do locatário desativará a lista moderna e as bibliotecas começarão e continuarão até 31 de maio de 2019.</span><span class="sxs-lookup"><span data-stu-id="8cdc0-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="8cdc0-112">As listas e bibliotecas que estão em modo clássico, como resultado do inquilino opt-out será automaticamente deslocado para moderno.</span><span class="sxs-lookup"><span data-stu-id="8cdc0-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="8cdc0-113">Se você precisar de modo clássico, consulte mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e a instrução PnP Powershell [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descreva opções e ferramentas que você pode usar hoje para usar a experiência clássica do modo.</span><span class="sxs-lookup"><span data-stu-id="8cdc0-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
