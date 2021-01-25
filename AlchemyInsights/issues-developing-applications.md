---
title: Questões que desenvolvem aplicações
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974771"
---
# <a name="issues-developing-applications"></a>Questões que desenvolvem aplicações

Para resolver os problemas mais comuns ao construir aplicações Azure Ative Directory (AD), consulte os seguintes artigos:

- [Estou a ver problemas em iniciar sessão para aplicações usando apenas o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Não sei como alterar os incumprimentos de toda a vida para a minha aplicação.](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Estou confuso sobre como funciona o consentimento da candidatura](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Não sei como conceder permissões à minha candidatura.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Não entendo a diferença entre permissões de candidaturas delegadas.](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Fim do suporte para Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)** _

- A partir de 30 de junho de 2020, deixaremos de adicionar quaisquer novidades à Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph). Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

- A partir de 30 de junho de 2022, terminaremos o suporte para o ADAL e a AAD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança. Como resultado desta condição, as seguintes são as implicações:

    - As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não receberão qualquer suporte técnico ou atualizações de segurança.

    - As aplicações que utilizam o Gráfico AAD após este tempo podem deixar de receber respostas do ponto final do Gráfico AAD

_ *Migração ADAL**

Se estiver a utilizar aplicações da Microsoft, recomendamos a atualização para a Microsoft Authentication Library (MSAL), que tem as mais recentes funcionalidades e atualizações de segurança. Esta recomendação encontra-se no contexto de a Microsoft iniciar o processo de migração das suas apps para a MSAL até ao fim do prazo de suporte. 

A migração pela Microsoft das suas apps para o MSAL garante que as aplicações beneficiam da segurança contínua da MSAL e das melhorias de funcionalidades.

1. [Leia as FAQ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Saiba como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Se precisar de ajuda para entender qual das suas aplicações usa ODAL, recomendamos que reveja todo o código fonte das suas aplicações e, se for caso disso, contacte quaisquer fornecedores de software independentes (ISV) ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações ADAL não-Microsoft no seu inquilino.

**Migração de gráficos AAD**

Para aplicações que estão a usar o AAD Graph, siga a nossa orientação para migrar aplicações AAD Graph para o Microsoft Graph:

1. [A nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
2. O portal de registo de aplicações Azure mostra quais as aplicações que estão a utilizar o AAD Graph. Recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer fornecedores de software independentes (ISV) ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe informações sobre o uso do AAD Graph no seu inquilino.







