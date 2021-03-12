---
title: Problemas de API do Microsoft Graph
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714156"
---
# <a name="microsoft-graph-api-issues"></a>Problemas de API do Microsoft Graph

Este tópico também pode aplicar-se aos desenvolvedores que ainda utilizam AZure AD Graph API. No entanto, recomenda-se **vivamente** que utilize o Microsoft Graph para todos os cenários de gestão de diretórios, identidades e acessos.

**Questões de autenticação ou autorização**

- Se a sua aplicação **não conseguir adquirir fichas** para ligar para o Microsoft Graph, escolha **Problema com a obtenção de um token de acesso (Autenticação)** da categoria Microsoft Graph para obter ajuda e suporte mais específicos sobre este tópico.
- Se a sua aplicação estiver **a receber erros de autorização de 401 ou 403** ao ligar para o Microsoft Graph, escolha a categoria **API de um erro negado de acesso (Autorização)** da Microsoft para obter ajuda e suporte mais específicos sobre este tópico.

**Quero usar o Microsoft Graph, mas não sei por onde começar.**

- [Visão geral do Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Visão geral da gestão de identidade e acesso no Gráfico do Microsoft](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Começar a construir aplicativos Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Teste ApIs de Gráfico microsoft no seu inquilino ou inquilino de demonstração

**Quero usar o Microsoft Graph, mas suporta as APIs do diretório v1.0 que preciso?**

O Microsoft Graph é a API recomendada para a gestão de diretórios, identidades e acessos. No entanto, existem ainda algumas lacunas entre o que é possível no Azure AD Graph e microsoft Graph. Reveja os seguintes artigos, que destacam as diferenças mais atualizadas para ajudar na sua escolha:

- [Diferenças de tipo de recurso entre gráfico AD Ad Azure e Gráfico microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferenças de propriedade entre O Gráfico AD AZure e Gráfico microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferenças de método entre Azure AD e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**A API que estou a ligar não funciona, onde posso fazer mais testes?**

**Microsoft Graph Explorer** - Teste APIs do Microsoft Graph no seu inquilino ou inquilino de demonstração e também confira as consultas de **amostra** no Microsoft Graph Explorer.

**A minha aplicação é muito lenta e também está a ser estrangulada. Que melhorias posso fazer?**

Dependendo do seu cenário, existem várias opções à sua disposição para tornar a sua aplicação mais performante e, em alguns casos, menos propensa a ser estrangulada pelo serviço (quando está a fazer demasiadas chamadas).

- [As melhores práticas do Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Pedidos de loteamento](https://docs.microsoft.com/graph/json-batching)
- [Mudanças de faixa através da consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Ser notificado das alterações através de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Orientação de estrangulamento](https://docs.microsoft.com/graph/throttling)

**Onde posso encontrar mais informações sobre erros e questões conhecidas?**

- [Informações de resposta a erros do Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemas conhecidos com o Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Onde posso verificar o estado da disponibilidade de serviço e conectividade?**

A disponibilidade de serviço e conectividade dos serviços subjacentes que podem ser acedidos através do Microsoft Graph podem ter impacto na disponibilidade e desempenho globais do Microsoft Graph.

- Para a saúde do serviço de diretório ativo Azure, verifique o estado dos serviços de **Segurança + Identidade** listados na página de estado do [Azure](https://azure.microsoft.com/status/).
- Para os serviços do Office que contribuem para o Microsoft Graph, verifique o estado dos serviços listados no [Painel de Saúde do Office Service](https://portal.office.com/adminportal/home#/servicehealth).

Os erros de autorização do Microsoft Graph podem ser resultado de vários problemas diferentes, a maioria dos quais geram um erro de 401 ou 403. Por exemplo, todos os seguintes podem levar a erros de autorização:

- [Fluxos de aquisição de token de acesso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) incorreto
- [Âmbitos de permissão](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurados
- Falta de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Fim do suporte da Biblioteca de Autenticação do Active Directory (ADAL) e da API do Azure AD Graph (AAD Graph)_* _

_*A partir de 30 de junho de 2020**, não adicionaremos mais novidades ao ADAL e Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

**A partir de 30 de junho de 2022,** terminaremos o suporte ao ADAL e ao Azure AD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.

As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não *receberão qualquer suporte técnico ou atualizações de segurança.*

As aplicações que utilizam o Azure AD Graph após este tempo podem deixar de receber respostas do ponto final do Azure AD Graph.

**Migração ADAL**

Recomendamos que atualize para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem as funcionalidades e atualizações de segurança mais recentes.

Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está em processo de migrar as suas aplicações para o MSAL até ao fim do prazo de suporte, garantindo que beneficiará da segurança contínua da MSAL e das melhorias de funcionalidades.

1. [Consulte as FAQ da ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba mais sobre como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se precisar de ajuda para entender quais das suas aplicações usam ADAL, recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.

**Migração do AAD Graph**

Para aplicações que estão a usar o Azure AD Graph, siga as nossas orientações para [migrar aplicações AD AD para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [A nossa lista de verificação de migração inclui um ponto sobre introdução](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph. Recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todos os usos de gráficos AAD no seu inquilino.
3. Para que a sua aplicação aceda a dados no Microsoft Graph, o utilizador ou administrador deve conceder-lhe as permissões corretas através de um processo de consentimento. As [permissões de referência do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listam as permissões associadas a cada conjunto principal de APIs do Gráfico microsoft. Também fornece orientações sobre como usar as permissões.
