---
title: SharePoint Online Throttling
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931237"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online Throttling

**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano. Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup. Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.

Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana. Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos. No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.

**Servidor 503 está um erro ocupado**

Os utilizadores podem receber um servidor 503 está um erro de trabalho quando tentam navegar para sites SharePoint ou OneDrive. 

Este erro pode ser causado por estrangulamento dentro do serviço SharePoint. O SharePoint Online utiliza o estrangulamento para manter o desempenho e a fiabilidade ideais do serviço SharePoint Online. O estrangulamento limita o número de ações do utilizador ou chamadas simultâneas (por script ou código) para evitar o uso excessivo de recursos. 

Para obter mais informações sobre o estrangulamento, [evite ser estrangulado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Se você acredita que este erro não está relacionado com estrangulamento, você pode verificar se há manutenção ativa ocorrendo no seu inquilino navegando para o centro de [mensagens](https://portal.office.com/adminportal/home#/MessageCenter).

 Por fim, certifique-se de que visita a página [de Saúde](https://portal.office.com/adminportal/home#/servicehealth) de Serviço para verificar se podem ocorrer quaisquer avisos/incidentes.

