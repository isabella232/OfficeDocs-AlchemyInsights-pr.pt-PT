---
title: O fluxo de trabalho não está a começar
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766108"
---
# <a name="workflow-is-not-starting"></a>O fluxo de trabalho não está a começar

- Os fluxos de trabalho sharePoint 2010 e SharePoint 2013 não estão a começar.

    - Se o seu fluxo de trabalho não estiver a começar, pode haver um problema de serviço temporário onde os utilizadores podem sofrer atrasos intermitentes com o progresso do fluxo de trabalho. Verifique o Dashboard de [Saúde](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) de Serviço para ver se a sua organização está afetada.

    - Se passaram mais de 24 horas desde que viu este problema pela primeira vez, por favor, faça um bilhete de apoio. Em muitos casos, já estamos a trabalhar numa solução. Por favor, dê-nos pelo menos 24 horas para completar uma solução.

- Os fluxos de trabalho do SharePoint 2010 atrasaram-se no início.

    - Isto ocorre se o fluxo de trabalho for acionado em grandes lotes. (por exemplo, quando vários itens são adicionados ao mesmo tempo).

    - Os fluxos de trabalho não são projetados para funcionar em tempo real, por isso um atraso é o comportamento de by-design.

   -  Se o Fluxo de Trabalho for complexo extensível linguagem de marcação de objetos extensíveis (XMOL), a compilação pode ser lenta. Verifique [este](https://support.microsoft.com//kb/3043697) artigo.

    - Deve simplificar o fluxo de trabalho ou redesenhar utilizando o tipo de plataforma de Workflow Microsoft SharePoint 2013.

    - Se o seu histórico de fluxos de trabalho cresceu grande, pode querer expurgar os itens ou criar uma nova lista de história.

        Mais informações : [Limpar a história do fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Quer experimentar o Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


