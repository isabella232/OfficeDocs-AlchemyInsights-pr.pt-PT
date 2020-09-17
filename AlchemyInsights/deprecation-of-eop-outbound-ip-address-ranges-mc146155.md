---
title: 1065 Depreciação dos intervalos de endereço IP de saída do EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806806"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Depreciação dos intervalos de endereços IP de saída da EOP

Detetamos um problema potencial com a sua organização que (se não for corrigido até 26 de outubro de 2018) pode quebrar o fluxo de correio para os seus destinos no local ou destinos externos. Como anteriormente comunicado, para simplificar a gestão do intervalo de alcance de endereços IP, estamos a consolidar os intervalos de endereços IP exchange online protection (EOP) que são usados para enviar e receber e-mails fora da Microsoft 365. A nossa análise indica que uma ou mais das fontes ou destinos externos de e-mail que configuraste nos conectores de fluxo de correio não estão a aceitar ligações a partir dos intervalos de endereços IP mostrados [aqui.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Agirá antes de 26 de outubro para garantir que estas fontes e destinos aceitarão ligações de e para todos os [endereços IP EOP publicados.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Para mais informações sobre esta alteração, consulte os posts do Message Center [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Nota:** Se já utilizou a publicação de IP ou URL através de HTML, XML e RSS para atualizações de ponto final, também deverá migrar para os novos serviços web para automatizar este tipo de atualizações. Para obter mais informações, consulte [as categorias de pontos finais do Microsoft 365 e o Microsoft 365 IP Address e o serviço web URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
