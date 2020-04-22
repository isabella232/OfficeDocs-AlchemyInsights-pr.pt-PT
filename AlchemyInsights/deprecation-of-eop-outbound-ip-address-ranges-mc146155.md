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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation das gamas de endereços IP de saída do EOP

Detetámos um problema potencial com a sua organização que (se não for corrigido até 26 de outubro de 2018) pode quebrar o fluxo de correio para os seus destinos ou destinos externos. Como previamente comunicado, para simplificar a gestão da gama de endereços IP, estamos a consolidar as gamas de endereços IP exchange Online Protection (EOP) que são usadas para enviar e receber e-mails fora do Microsoft 365. A nossa análise indica que uma ou mais das fontes de e-mail ou destinos externos que configuraram nos conectores de fluxo de correio não estão a aceitar ligações das gamas de endereços IP mostradas [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Agir até 26 de outubro para garantir que estas fontes e destinos aceitarão ligações de e para todos os [endereços IP do EOP publicados.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Para mais informações sobre esta alteração, consulte os posts do Message Center [MC146155 ,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Nota**: Se já utilizou a publicação ip ou URL através de HTML, XML e RSS para atualizações de pontofinal, também deverá migrar para os novos serviços web para automatizar este tipo de atualizações. Para mais informações, consulte as categorias de [ponto final da Microsoft 365 e o Microsoft 365 IP Address e o serviço web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
