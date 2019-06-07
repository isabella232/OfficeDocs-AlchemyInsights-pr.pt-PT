---
title: 1065 descontinuação de IP de saída EOP endereço rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752966"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="00d97-102">Descontinuação de intervalos de endereços IP saídas EOP</span><span class="sxs-lookup"><span data-stu-id="00d97-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="00d97-103">Foram detectadas uma potencial questão com a sua organização que (se não corrigida pelo 26ª de Outubro de 2018) poderá interromper o fluxo de correio para o local ou a destinos externos.</span><span class="sxs-lookup"><span data-stu-id="00d97-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="00d97-104">Como anteriormente comunicados, para simplificar a gestão de intervalo de endereços IP, vamos estiver a consolidar os intervalos de endereços IP do Exchange Online protecção (EOP) que são utilizados para enviar e receber correio electrónico fora do Office 365.</span><span class="sxs-lookup"><span data-stu-id="00d97-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="00d97-105">A nossa análise indica que um ou mais origens de correio electrónico externo ou destinos configurado conectores de fluxo de correio não estão a aceitar ligações a partir do IP endereço intervalos mostrado [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="00d97-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="00d97-106">Agir antes de Outubro de 26ª para garantir que estas origens e destinos aceitará ligações de e para todos os [endereços IP de EOP de publicado](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="00d97-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="00d97-107">Para mais informações sobre esta alteração, consulte que Centro de mensagens regista [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="00d97-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="00d97-108">**Nota**: Se tiver utilizado a colocação de IP ou o URL através do HTML, XML e RSS para actualizações de ponto final, também deverá migrar para os novos serviços web para automatizar estes tipos de actualizações.</span><span class="sxs-lookup"><span data-stu-id="00d97-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="00d97-109">Para mais informações, consulte as [categorias de ponto final do Office 365 e o endereço de IP do Office 365 e o serviço web de URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="00d97-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
