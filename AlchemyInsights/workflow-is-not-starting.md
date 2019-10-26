---
title: O fluxo de trabalho não está a começar
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738100"
---
# <a name="workflow-is-not-starting"></a>O fluxo de trabalho não está a começar

- Os fluxos de trabalho do SharePoint 2010 e do SharePoint 2013 não estão começando.

    - Se o seu fluxo de trabalho não estiver a começar, poderá haver um problema de serviço temporário em que os utilizadores podem sofrer atrasos intermitentes com o progresso do fluxo de trabalho. Verifique o Painel de Saúde do [Serviço](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização está afetada.

    - Se mais de 24 horas se passaram desde que você viu pela primeira vez este problema, por favor, registre um bilhete de suporte. Em muitos casos, já estamos trabalhando em uma solução. Por favor, dê-nos pelo menos 24 horas para completar uma solução.

- Os fluxos de trabalho do SharePoint 2010 atrasaram no início.

    - Isso ocorre se o fluxo de trabalho for acionado em grandes lotes. (por exemplo, quando vários itens são adicionados ao mesmo tempo).

    - Os fluxos de trabalho não são projetados para serem executados em tempo real, então um atraso é o comportamento de design por ação.

   -  Se o fluxo de trabalho for complexo da Linguagem de Marcação de Objetoextensível (XMOL), a compilação pode ser lenta. Confira [este](https://support.microsoft.com//kb/3043697) artigo.

    - Você deve simplificar o fluxo de trabalho ou reprojetá-lo usando o tipo de plataforma de fluxo de trabalho Microsoft SharePoint 2013.

    - Se o seu histórico de fluxo de trabalho cresceu, você pode querer limpar os itens ou criar uma nova lista de história.

        Mais informações: [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Quer experimentar o Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


