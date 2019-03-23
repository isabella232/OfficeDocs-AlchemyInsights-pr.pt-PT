---
title: 1065 descontinuação de IP de saída EOP endereço rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777282"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Descontinuação de intervalos de endereços IP saídas EOP

Foram detectadas uma potencial questão com a sua organização que (se não corrigida pelo 26ª de Outubro de 2018) poderá interromper o fluxo de correio para o local ou a destinos externos. Como anteriormente comunicados, para simplificar a gestão de intervalo de endereços IP, vamos estiver a consolidar os intervalos de endereços IP do Exchange Online protecção (EOP) que são utilizados para enviar e receber correio electrónico fora do Office 365. A nossa análise indica que um ou mais origens de correio electrónico externo ou destinos configurado conectores de fluxo de correio não estão a aceitar ligações a partir do IP endereço intervalos mostrado [aqui](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Agir antes de Outubro de 26ª para garantir que estas origens e destinos aceitará ligações de e para todos os [endereços IP de EOP de publicado](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Para mais informações sobre esta alteração, consulte que Centro de mensagens regista [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Nota**: Se tiver utilizado a colocação de IP ou o URL através do HTML, XML e RSS para actualizações de ponto final, também deverá migrar para os novos serviços web para automatizar estes tipos de actualizações. Para mais informações, consulte as [categorias de ponto final do Office 365 e o endereço de IP do Office 365 e o serviço web de URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

