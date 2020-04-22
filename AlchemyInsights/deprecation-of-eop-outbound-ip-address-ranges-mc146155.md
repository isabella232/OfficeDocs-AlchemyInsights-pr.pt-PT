---
title: 1065 Deprecation of EOP outbound IP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704608"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="40583-102">Deprecation das gamas de endereços IP de saída do EOP</span><span class="sxs-lookup"><span data-stu-id="40583-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="40583-103">Detetámos um problema potencial com a sua organização que (se não for corrigido até 26 de outubro de 2018) pode quebrar o fluxo de correio para os seus destinos ou destinos externos.</span><span class="sxs-lookup"><span data-stu-id="40583-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="40583-104">Como previamente comunicado, para simplificar a gestão da gama de endereços IP, estamos a consolidar as gamas de endereços IP exchange Online Protection (EOP) que são usadas para enviar e receber e-mails fora do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="40583-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="40583-105">A nossa análise indica que uma ou mais das fontes de e-mail ou destinos externos que configuraram nos conectores de fluxo de correio não estão a aceitar ligações das gamas de endereços IP mostradas [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="40583-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="40583-106">Agir até 26 de outubro para garantir que estas fontes e destinos aceitarão ligações de e para todos os [endereços IP do EOP publicados.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="40583-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="40583-107">Para mais informações sobre esta alteração, consulte os posts do Message Center [MC146155 ,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="40583-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="40583-108">**Nota**: Se já utilizou a publicação ip ou URL através de HTML, XML e RSS para atualizações de pontofinal, também deverá migrar para os novos serviços web para automatizar este tipo de atualizações.</span><span class="sxs-lookup"><span data-stu-id="40583-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="40583-109">Para mais informações, consulte as categorias de [ponto final da Microsoft 365 e o Microsoft 365 IP Address e o serviço web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="40583-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
