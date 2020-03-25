---
title: Dicas políticas dlp não funcionam
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932597"
---
# <a name="dlp-policy-tip-issues"></a>DLP Questões de Ponta Política

**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano. Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup. Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.

Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana. Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos. No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.

**Dicas políticas dlp**

Ao utilizar **as políticas dLP,** os utilizadores podem ser notificados de uma violação de política com dicas de **política.** Os administradores podem configurar dicas de política para exibir enquanto testam a sua política dLP ou quando a política está em pleno modo de execução.
  
Para configurar as dicas de política na sua política dLP no centro de segurança e conformidade em modo de execução completo, faça o seguinte:
  
- Certifique-se de que as dicas de política foram **ativadas** na regra DLP utilizando os passos [aqui .](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)

- Certifique-se de que o seu **conteúdo corresponde** ao **necessário** para desencadear a regra descrita neste artigo [aqui](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Exibição de dicas de política tanto no OWA como no Outlook. No entanto, ao utilizar **o Outlook 2013 ou mais tarde,** as dicas de política só são apresentadas em determinadas condições. Estas condições estão listadas aqui: [Condições suportadas para o Outlook 2013 ou mais tarde para exibir Dicas](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions) políticas

Para obter informações adicionais sobre as dicas políticas do DLP, consulte: [Mostrar dicas políticas para políticas de DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  