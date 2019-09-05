---
title: Não está a iniciar o fluxo de trabalho
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
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738100"
---
# <a name="workflow-is-not-starting"></a>Não está a iniciar o fluxo de trabalho

- Fluxos de trabalho do SharePoint 2010 e 2013 do SharePoint não estão a iniciar.

    - Se não estiver a iniciar o fluxo de trabalho, poderá existir um problema de serviço temporária onde os utilizadores poderão verificar atrasos intermitentes com o progresso de fluxo de trabalho. Verifique se o [Serviço de saúde Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se a sua organização é afectada.

    - Se tiverem passado mais de 24 horas desde que a visualizou pela primeira vez a este problema, inicie uma permissão de suporte. Em muitos casos, a Microsoft já estiver a trabalhar numa solução. Forneça pelo menos 24 horas para concluir uma solução.

- Fluxos de trabalho do SharePoint 2010 atrasada no início.

    - Isto ocorre se o fluxo de trabalho é accionado em grandes lotes. (por exemplo, quando vários itens são adicionados ao mesmo tempo).

    - Fluxos de trabalho não foram concebidos para funcionar em tempo real, por isso um atraso é o comportamento de design.

   -  Se o fluxo de trabalho complexos Extensible objecto Markup Language (XMOL), compilação pode ser lenta. Consulte [Este](https://support.microsoft.com//kb/3043697) artigo.

    - Deve simplificar o fluxo de trabalho ou adaptá-lo utilizando o tipo de plataforma de fluxo de trabalho do Microsoft SharePoint 2013.

    - Se tiver aumentado o histórico de fluxo de trabalho, poderá pretender remover os itens ou criar uma nova lista do histórico.

        Obter mais informações: [Limpar o histórico de fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Pretende tentar Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Fluxo e do SharePoint](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


