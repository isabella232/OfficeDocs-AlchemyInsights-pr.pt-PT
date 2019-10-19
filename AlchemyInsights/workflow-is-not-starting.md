---
title: Fluxo de trabalho não está iniciando
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738100"
---
# <a name="workflow-is-not-starting"></a>Fluxo de trabalho não está iniciando

- Fluxos de trabalho do SharePoint 2010 e SharePoint 2013 não estão iniciando.

    - Se o fluxo de trabalho não estiver iniciando, pode haver um problema de serviço temporário em que os usuários podem enfrentar atrasos intermitentes com o andamento do fluxo de trabalho. Verifique o [painel de integridade do serviço](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização foi afetada.

    - Se mais de 24 horas se passaram desde que você viu este problema pela primeira vez, por favor, registre um ticket de suporte. Em muitos casos, já estamos trabalhando em uma solução. Por favor, dê-nos pelo menos 24 horas para completar uma solução.

- Fluxos de trabalho do SharePoint 2010 atrasados no início.

    - Isso ocorre se o fluxo de trabalho é acionado em lotes grandes. (por exemplo, quando vários itens são adicionados de uma só vez).

    - Fluxos de trabalho não são projetados para executar em tempo real, portanto, um atraso é o comportamento de design.

   -  Se o fluxo de trabalho é complexo Extensible Object Markup Language (XMOL), compilação pode ser lenta. Verifique [este](https://support.microsoft.com//kb/3043697) artigo.

    - Você deve simplificar o fluxo de trabalho ou reformulá-lo usando o tipo de plataforma Microsoft SharePoint 2013 Workflow.

    - Se o histórico de fluxo de trabalho cresceu grande, convém limpar os itens ou criar uma nova lista de histórico.

        Mais informações: [Limpar histórico de fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Deseja experimentar o Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e fluxo](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


