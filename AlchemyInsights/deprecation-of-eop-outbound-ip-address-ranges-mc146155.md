---
title: 1065 Preterição dos intervalos de endereços IP de saída do EOPMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031273"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Preterição dos intervalos de endereços IP de saída do EOP

Detetamos um possível problema com a sua organização que (se não for corrigido até 26 de outubro de 2018) poderá interromper o fluxo de correio para os seus destinos no local ou externo. Conforme comunicado anteriormente, para simplificar a gestão do intervalo de endereços IP, estamos a consolidar os intervalos de endereços IP do Proteção do Exchange Online (EOP) utilizados para enviar e receber e-mail fora do Microsoft 365. A nossa análise indica que uma ou mais origens de e-mail ou destinos externos que configurou nos conectores de fluxo de correio não estão a aceitar ligações a partir dos intervalos de endereços IP aqui [apresentados.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Atua antes de 26 de outubro para garantir que estas origens e destinos aceitarão ligações de e para todos os endereços IP da [EOP publicados.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Para obter mais informações sobre esta alteração, consulte Mensagens do Centro de Mensagens [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Nota:** se tiver utilizado anteriormente a publicação de IP ou URL através de HTML, XML e RSS para atualizações de pontos finais, também deverá migrar para os novos serviços Web para automatizar estes tipos de atualizações. Para obter mais informações, consulte [Microsoft 365 de pontos finais e Microsoft 365 ENDEREÇO IP e serviço Web de URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
