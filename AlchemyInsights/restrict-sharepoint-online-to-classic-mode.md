---
title: Restringir o SharePoint Online ao modo clássico
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742480"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="26a96-102">Restringir o SharePoint Online ao modo clássico</span><span class="sxs-lookup"><span data-stu-id="26a96-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="26a96-103">Algumas organizações ainda requerem a experiência do modo Clássico.</span><span class="sxs-lookup"><span data-stu-id="26a96-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="26a96-104">Embora não existam planos para remover o modo clássico a um nível granular, já não é possível restringir toda uma organização (inquilino) ao modo clássico para listas e bibliotecas.</span><span class="sxs-lookup"><span data-stu-id="26a96-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="26a96-105">O administrador terá as seguintes opções para gerir listas e bibliotecas individuais em modo clássico utilizando interruptores de opt-out granular que fornecemos nos seguintes níveis:</span><span class="sxs-lookup"><span data-stu-id="26a96-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="26a96-106">coleção de site</span><span class="sxs-lookup"><span data-stu-id="26a96-106">site collection</span></span>
- <span data-ttu-id="26a96-107">site</span><span class="sxs-lookup"><span data-stu-id="26a96-107">site</span></span>
- <span data-ttu-id="26a96-108">lista</span><span class="sxs-lookup"><span data-stu-id="26a96-108">list</span></span>
- <span data-ttu-id="26a96-109">biblioteca</span><span class="sxs-lookup"><span data-stu-id="26a96-109">library</span></span>

<span data-ttu-id="26a96-110">Além disso, as listas que utilizam determinadas funcionalidades e personalizações que não são suportadas pelo moderno continuarão a ser automaticamente mudadas para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="26a96-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="26a96-111">A partir de 1 de abril de 2019, o processo de desativação do nível de inquilino opta por não lista moderna e as bibliotecas vão começar e continuar até 31 de maio de 2019.</span><span class="sxs-lookup"><span data-stu-id="26a96-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="26a96-112">As listas e bibliotecas que estão em modo clássico como resultado do opt-out do inquilino serão automaticamente transferidas para moderno.</span><span class="sxs-lookup"><span data-stu-id="26a96-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="26a96-113">Se necessitar de um modo clássico, consulte mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instrução pnP Powershell [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descreve opções e ferramentas que pode usar hoje para usar a experiência de modo clássico.</span><span class="sxs-lookup"><span data-stu-id="26a96-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
