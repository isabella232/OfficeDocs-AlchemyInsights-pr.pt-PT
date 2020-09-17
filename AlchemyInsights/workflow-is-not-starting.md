---
title: O fluxo de trabalho não está a começar
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794778"
---
# <a name="workflow-is-not-starting"></a>O fluxo de trabalho não está a começar

- Os fluxos de trabalho do SharePoint 2010 e do SharePoint 2013 não estão a começar.

    - Se o seu fluxo de trabalho não estiver a começar, pode haver um problema de serviço temporário onde os utilizadores podem sofrer atrasos intermitentes com o progresso do fluxo de trabalho. Consulte o [Painel de Saúde](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) do Serviço para ver se a sua organização está com impacto.

    - Se passaram mais de 24 horas desde que viu este problema pela primeira vez, por favor, faça um bilhete de apoio. Em muitos casos, já estamos a trabalhar numa solução. Por favor, dê-nos pelo menos 24 horas para completar uma solução.

- Fluxos de trabalho sharePoint 2010 adiados no início.

    - Isto ocorre se o fluxo de trabalho for acionado em grandes lotes. (por exemplo, quando vários itens são adicionados ao mesmo tempo).

    - Os fluxos de trabalho não são projetados para funcionar em tempo real, por isso um atraso é o comportamento por design.

   -  Se o fluxo de trabalho for complexo lingueta de marcação de objetos extensíveis (XMOL), a compilação pode ser lenta. Veja [este](https://support.microsoft.com//kb/3043697) artigo.

    - Deve simplificar o fluxo de trabalho ou redesenhar-o utilizando o tipo de plataforma de fluxo de trabalho Microsoft SharePoint 2013.

    - Se o seu histórico de fluxo de trabalho cresceu, pode querer purgar os itens ou criar uma nova lista de histórias.

        Mais informações : [Purgar a história do fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Quer experimentar o Microsoft Flow no SharePoint Online?
- [Criar Fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


