---
title: O fluxo de trabalho não está a iniciar
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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907749"
---
# <a name="workflow-is-not-starting"></a>O fluxo de trabalho não está a iniciar

- Os fluxos de trabalho do SharePoint 2010 e SharePoint 2013 não estão a iniciar.

    - Se o seu fluxo de trabalho não estiver a iniciar, poderá haver um problema de serviço temporário em que os utilizadores podem detetá-los com atrasos intermitentes com o progresso do fluxo de trabalho. Consulte o [Dashboard do Estado de Estado de](https://admin.microsoft.com/AdminPortal/Home/servicehealth) Trabalho para ver se a sua organização é afetada.

    - Se já passaram mais de 24 horas desde que viu este problema pela primeira vez, remova um bilhete de suporte. Em muitos casos, estamos a trabalhar numa solução. Dê-nos, pelo menos, 24 horas para concluir a solução.

- Os fluxos de trabalho do SharePoint 2010 foram adiados no início.

    - Isto ocorre se o fluxo de trabalho for ativado em lotes grandes. (por exemplo, quando são adicionados vários itens de uma só vez).

    - Os fluxos de trabalho não foram concebidos para ser executados em tempo real, pelo que um atraso é o comportamento estruturado.

   -  Se o Fluxo de Trabalho for uma linguagem XMOL (Extensible Object Markup Language) complexa, a compilação pode ser lenta. Consulte [este](https://support.microsoft.com//kb/3043697) artigo.

    - Deve simplificar o fluxo de trabalho ou redesenha-lo utilizando o tipo de plataforma Fluxo de Trabalho do Microsoft SharePoint 2013.

    - Se o histórico do seu fluxo de trabalho cresceu grande, poderá querer remova os itens ou crie uma nova lista do histórico.

        Mais Informações: Limpar [histórico de fluxos de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tópicos relacionados
Pretende experimentar o Microsoft Flow SharePoint Online?
- [Criar Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
