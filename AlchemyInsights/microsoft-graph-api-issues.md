---
title: Problemas com Graph API do Microsoft Graph Microsoft
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975904"
---
# <a name="microsoft-graph-api-issues"></a>Problemas com Graph API do Microsoft Graph Microsoft

Este tópico também pode aplicar-se aos programadores que ainda utilizam a Azure AD Graph API. No entanto, **recomendamos vivamente que** utilize o Microsoft Graph para todos os cenários de gestão de diretórios, identidades e acesso.

**Problemas de autenticação ou autorização**

- Se a sua aplicação não conseguir adquirir **tokens** para ligar para o Microsoft Graph, escolha Problema ao obter uma categoria de **token** de acesso (Autenticação) do Microsoft Graph para obter ajuda e suporte mais específicos sobre este tópico.
- Se a sua aplicação estiver a receber erros de autorização **401 ou 403** ao ligar para o Microsoft Graph, escolha a categoria Obter um erro de acesso negado **(Autorização)** da API do Microsoft Graph para obter ajuda e suporte mais específicos sobre este tópico.

**Quero utilizar o Microsoft Graph, mas não tenho a certeza por onde começar**

- [Visão geral do Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Overview of Identity and Access Management in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Começar a criar aplicações microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer -** Teste as APIs do Microsoft Graph no seu inquilino ou um inquilino de demonstração

**Quero utilizar o Microsoft Graph, mas suporta as APIs do diretório v1.0 de que preciso?**

O Microsoft Graph é a API recomendada para a gestão de diretórios, identidades e acessos. No entanto, ainda existem alguns intervalos entre o que é possível fazer no Azure AD Graph Microsoft Graph. Reveja os seguintes artigos, que destacam as diferenças mais recentes para ajudar na sua escolha:

- [Diferenças de tipo de recurso entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferenças de propriedades entre o Azure AD Graph e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferenças de métodos entre o Azure AD e o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**A API para a qual estou a ligar não funciona, onde posso fazer mais testes?**

**Microsoft Graph Explorer** - Teste as APIs do Microsoft Graph no seu inquilino  ou um inquilino de demonstração e consulte também as consultas de exemplo no Microsoft Graph Explorer.

**A minha aplicação é demasiado lenta e também está a ser pequena. Que melhorias posso fazer?**

Dependendo do seu cenário, existe uma variedade de opções à sua disposição para tornar a sua aplicação mais eficaz e, em alguns casos, menos promissora a ser reestaurada pelo serviço (quando faz demasiadas chamadas).

- [Melhores Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Pedidos de lote](https://docs.microsoft.com/graph/json-batching)
- [Controlar alterações através de uma consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Receber notificações de alterações através de Webhooks](https://docs.microsoft.com/graph/webhooks)
- [Orientação da ressarceção de ajuda](https://docs.microsoft.com/graph/throttling)

**Onde posso encontrar mais informações sobre erros e problemas conhecidos?**

- [Informação Graph resposta a erros do Microsoft Graph Microsoft](https://docs.microsoft.com/graph/errors)
- [Problemas conhecidos do Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Onde posso verificar o estado da disponibilidade do serviço e da conectividade?**

A disponibilidade do serviço e a conectividade dos serviços submetidos que podem ser acededos através do Microsoft Graph pode afetar a disponibilidade geral e o desempenho do Microsoft Graph.

- Para Azure Active Directory estado de serviço, verifique o estado dos serviços **de Segurança e Identidade** listados na página de estado do [Azure.](https://azure.microsoft.com/status/)
- Para Office serviços que contribuem para o Microsoft Graph, verifique o estado dos serviços listados [no Dashboard](https://portal.office.com/adminportal/home#/servicehealth)Office Estado de Serviço.

Os Graph de autorização do Microsoft Graph podem ser resultantes de vários problemas diferentes, a maioria dos quais geram um erro 401 ou 403. Por exemplo, o seguinte pode levar a erros de autorização:

- [Fluxos de aquisição de token de acesso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) incorreto
- [Âmbitos de permissão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurados
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Fim do suporte da API Azure Active Directory ADAL (ADAL) e da API de AD Graph AAD (AAD Graph)***

**A partir de 30 de junho de 2020,** deixaremos de adicionar novas funcionalidades à ADAL e ao Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

A **partir de 30 de junho de 2022,** o suporte da ADAL e do Azure AD Graph deixará de fornecer suporte técnico ou atualizações de segurança.

As aplicações que utilizem a ADAL em versões existentes do SO continuarão a funcionar após essa hora, mas não obterão suporte técnico *ou atualizações de segurança.*

As aplicações que utilizam o Azure AD Graph após este período de tempo poderão já não receber respostas do ponto final do Azure AD Graph atualização.

**Migração ADAL**

Recomendamos que atualize para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem as funcionalidades e atualizações de segurança mais recentes.

Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está no processo de migração das aplicações para o MSAL até ao fim do prazo de suporte, assegurando que beneficiarão das melhorias contínuas de funcionalidades e segurança da MSAL.

1. [Consulte as FAQ da ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba mais sobre como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se precisar de ajuda para compreender que aplicações utilizam a ADAL, recomendamos que reveja o código fonte de todas as suas aplicações e, se aplicável, contacte quaisquer ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.

**Migração do AAD Graph**

Para as aplicações que utilizam o Azure AD Graph, siga as nossas orientações para migrar as [aplicações Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)para o Microsoft Graph .

1. [A nossa lista de verificação de migração inclui um ponto sobre introdução](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph. Recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todos os serviços de utilização Graph AAD no seu inquilino.
3. Para que a sua aplicação aceda aos dados no Microsoft Graph, o utilizador ou administrador tem de lhe conceder as permissões corretas através de um processo de consentimento. O [Microsoft Graph de permissões lista](https://docs.microsoft.com/graph/permissions-reference) as permissões associadas a cada conjunto principal de APIs microsoft Graph. Também fornece orientações sobre como utilizar as permissões.
