---
title: Estrangulamento online sharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931453"
---
# <a name="sharepoint-online-throttling"></a>Estrangulamento online sharePoint

**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano. Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup. Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.

Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana. Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos. No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.

**Estrangulamento online sharePoint**

O SharePoint Online utiliza o estrangulamento para manter o desempenho e a fiabilidade ideais do serviço SharePoint Online. O estrangulamento limita o número de ações do utilizador ou chamadas simultâneas (por script ou código) para evitar o uso excessivo de recursos. Para mais informações, visite os links abaixo.

- [Evite ser estrangulado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Migração de dados e estrangulamento do SPO](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [SharePoint Online e OneDrive Velocidade de migração](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [Manuseie o estrangulamento online do SharePoint através da utilização de back off exponencial](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [Planeamento de capacidade e testes de carga SharePoint Online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

