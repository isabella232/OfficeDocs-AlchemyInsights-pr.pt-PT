---
title: Restringir SharePoint Online para o modo clássico
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369784"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="d0820-102">Restringir SharePoint Online para o modo clássico</span><span class="sxs-lookup"><span data-stu-id="d0820-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="d0820-103">Algumas organizações necessitam da experiência de modo clássico.</span><span class="sxs-lookup"><span data-stu-id="d0820-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="d0820-104">Enquanto não existem planos para remover de modo clássico a um nível granular, já não é possível restringir toda uma organização (tenant) para o modo clássico para listas e bibliotecas.</span><span class="sxs-lookup"><span data-stu-id="d0820-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="d0820-105">O administrador terá as seguintes opções para gerir listas e bibliotecas na utilizando parâmetros de cancelamento granulares que fornecemos aos seguintes níveis de modo clássico individuais:</span><span class="sxs-lookup"><span data-stu-id="d0820-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="d0820-106">colecção de sites</span><span class="sxs-lookup"><span data-stu-id="d0820-106">site collection</span></span>
- <span data-ttu-id="d0820-107">site</span><span class="sxs-lookup"><span data-stu-id="d0820-107">site</span></span>
- <span data-ttu-id="d0820-108">lista</span><span class="sxs-lookup"><span data-stu-id="d0820-108">list</span></span>
- <span data-ttu-id="d0820-109">biblioteca</span><span class="sxs-lookup"><span data-stu-id="d0820-109">library</span></span>

<span data-ttu-id="d0820-110">Além disso, listas utilizam determinadas funcionalidades e personalizações que não são suportadas pelo moderno serão ainda ser mudadas automaticamente para o modo clássico.</span><span class="sxs-lookup"><span data-stu-id="d0820-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="d0820-111">Início de Abril de 1 de Maio de 2019, o processo para desactivar o nível de Tenants activamente por não lista moderna e bibliotecas inicia e continue a 31 de Maio de 2019.</span><span class="sxs-lookup"><span data-stu-id="d0820-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="d0820-112">As listas e bibliotecas que se encontram no modo clássico na sequência de Tenants opt-out serão automaticamente transferidas para modernas.</span><span class="sxs-lookup"><span data-stu-id="d0820-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="d0820-113">Se necessitar de modo clássico mais informações, consulte [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instruções de PnP Powershell [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descreve as opções e ferramentas que pode utilizar hoje para utilizarem a experiência de modo clássico.</span><span class="sxs-lookup"><span data-stu-id="d0820-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
