---
title: Problemas com bibliotecas de autenticação
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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063641"
---
# <a name="issues-with-authentication-libraries"></a>Problemas com bibliotecas de autenticação

1. [As bibliotecas](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) de autenticação da plataforma de identidade da Microsoft listam bibliotecas de clientes e middleware suportadas pela Microsoft e compatíveis.
2. A Microsoft Authentication Library (MSAL) suporta vários [fluxos de autenticação](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) para utilização em diferentes cenários de aplicação.
3. Para autenticar e adquirir fichas, inicializa uma nova aplicação de cliente pública ou confidencial no seu código. Pode definir várias opções de configuração quando rubricar a aplicação do cliente na Biblioteca de Autenticação do Microsoft (MSAL). Para saber mais, consulte [as opções de configuração de aplicação](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Fim do suporte para Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**

**A partir de 30 de junho de 2020,** deixaremos de adicionar novidades ao ADAL e ao Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

**A partir de 30 de junho de 2022,** terminaremos o suporte ao ADAL e ao Azure AD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.

As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não *receberão qualquer suporte técnico ou atualizações de segurança.*

As aplicações que utilizam o Azure AD Graph após este tempo podem deixar de receber respostas do ponto final do Azure AD Graph.

**Migração ADAL**

Recomendamos que atualize para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem as funcionalidades e atualizações de segurança mais recentes.

Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está em processo de migrar as suas aplicações para o MSAL até ao fim do prazo de suporte, garantindo que beneficiará das melhorias de segurança e funcionalidades em curso da MSAL.

Para mais informações, consulte:

1. [Consulte as FAQ da ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saiba mais sobre como migrar aplicações por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se precisar de ajuda para entender quais das suas aplicações usam ADAL, recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.

**Migração do AAD Graph**

Para aplicações que estão a usar o Azure AD Graph, siga as nossas orientações para [migrar aplicações AD AD para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [A nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph. Recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todos os usos de gráficos AAD no seu inquilino.
3. Para que a sua aplicação aceda a dados no Microsoft Graph, o utilizador ou administrador deve conceder-lhe as permissões corretas através de um processo de consentimento. As [permissões de referência do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listam as permissões associadas a cada conjunto principal de APIs do Gráfico microsoft. Também fornece orientações sobre como usar as permissões.
