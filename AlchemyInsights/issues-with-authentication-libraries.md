---
title: Problemas com as Bibliotecas de Autenticação
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028015"
---
# <a name="issues-with-authentication-libraries"></a>Problemas com as Bibliotecas de Autenticação

1. [plataforma de identidades da Microsoft bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lista bibliotecas de cliente e de middleware compatíveis com a Microsoft.
2. A Biblioteca de Autenticação da Microsoft (MSAL) suporta vários fluxos de autenticação para utilização em [cenários](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) de aplicação diferentes.
3. Para autenticar e adquirir tokens, tem de inicializar uma nova aplicação de cliente pública ou confidencial no seu código. Pode definir várias opções de configuração ao inicializar a aplicação cliente na Biblioteca de Autenticação da Microsoft (MSAL). Para saber mais, consulte Opções [de configuração da aplicação.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Fim do suporte da API Azure Active Directory ADAL (ADAL) e da API de AD Graph AAD (AAD Graph)**

**A partir de 30 de junho de 2020,** deixaremos de adicionar novas funcionalidades à ADAL e ao Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

A **partir de 30 de junho de 2022,** o suporte da ADAL e do Azure AD Graph deixará de fornecer suporte técnico ou atualizações de segurança.

As aplicações que utilizem a ADAL em versões existentes do SO continuarão a funcionar após essa hora, mas não obterão suporte técnico *ou atualizações de segurança.*

As aplicações que utilizam o Azure AD Graph após este período de tempo poderão já não receber respostas do ponto final do Azure AD Graph atualização.

**Migração ADAL**

Recomendamos que atualize para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem as funcionalidades e atualizações de segurança mais recentes.

Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está no processo de migração das aplicações para o MSAL até ao fim do prazo de suporte, assegurando que irão beneficiar das melhorias contínuas de funcionalidades e segurança da MSAL.

Para mais informações, consulte:

1. [Consulte as FAQ da ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba mais sobre como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se precisar de ajuda para compreender que aplicações utilizam a ADAL, recomendamos que reveja o código fonte de todas as suas aplicações e, se aplicável, contacte quaisquer ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.

**Migração do AAD Graph**

Para as aplicações que utilizam o Azure AD Graph, siga as nossas orientações para migrar as [aplicações Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)para o Microsoft Graph .

1. [A nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph. Recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todos os serviços de utilização Graph AAD no seu inquilino.
3. Para que a sua aplicação aceda aos dados no Microsoft Graph, o utilizador ou administrador tem de lhe conceder as permissões corretas através de um processo de consentimento. O [Microsoft Graph de permissões lista](https://docs.microsoft.com/graph/permissions-reference) as permissões associadas a cada conjunto principal de APIs microsoft Graph. Também fornece orientações sobre como utilizar as permissões.
