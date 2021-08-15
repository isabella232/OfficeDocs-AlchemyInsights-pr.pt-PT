---
title: Problemas de desenvolvimento de aplicações
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013435"
---
# <a name="issues-developing-applications"></a>Problemas de desenvolvimento de aplicações

Para resolver os problemas mais comuns ao criar aplicações Azure Active Directory (AD), consulte os seguintes artigos:

- [Estou a ter problemas a entrar em aplicações apenas com o browser Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Não sei como alterar as predefinições da duração do token para a minha aplicação](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Estou confuso com o funcionamento do consentimento da aplicação](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Não sei como conceder permissões à minha aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Não compreendo a diferença entre permissões delegadas e de aplicações](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Fim do suporte da API Azure Active Directory ADAL (ADAL) e da API de AD Graph AAD (AAD Graph)***

- Desde 30 de junho de 2020, deixámos de adicionar novas funcionalidades à Biblioteca de Autenticação do Active Directory (ADAL) e à API do Azure AD Graph (AAD Graph). Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

- A partir de 30 de junho de 2022, iremos terminar o suporte para o ADAL e para o AAD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança. Como resultado desta condição, seguem-se as implicações:

    - As aplicações que utilizam o ADAL em versões existentes do SO continuarão a funcionar após esta data mas não terão suporte técnico ou atualizações de segurança.

    - As aplicações que Graph AAD poderão deixar de receber respostas do ponto Graph AAD

**Migração ADAL**

Se estiver a utilizar aplicações da Microsoft, recomendamos que atualize para a Biblioteca de Autenticação da Microsoft (MSAL), que tem as funcionalidades e atualizações de segurança mais recentes. Esta recomendação está no contexto de a Microsoft iniciar o processo de migração das aplicações para o MSAL até ao fim do prazo de suporte. 

A migração das aplicações da Microsoft para o MSAL garante que as aplicações beneficiam das melhorias contínuas de funcionalidades e segurança da MSAL.

1. [Consulte as FAQ da ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Saiba mais sobre como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Se precisar de ajuda para compreender que aplicações utilizam a ADAL, recomendamos que reveja o código fonte de todas as suas aplicações e, se aplicável, contacte fornecedores de software independentes (ISVs) ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.

**Migração do AAD Graph**

Para as aplicações que utilizam o AAD Graph, siga as nossas orientações para migrar as aplicações do AAD Graph para o Microsoft Graph:

1. [A nossa lista de verificação de migração inclui um ponto sobre introdução](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph. Recomendamos que reveja o código fonte de todas as suas aplicações e, se aplicável, contacte fornecedores de software independentes (ISVs) ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe informações sobre a utilização Graph AAD no seu inquilino.







