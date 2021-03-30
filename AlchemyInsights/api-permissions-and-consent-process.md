---
title: Permissões da API e Processo de Consentimento
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405437"
---
# <a name="api-permissions-and-consent-process"></a>Permissões da API e Processo de Consentimento

Para que a sua aplicação aceda a dados no Microsoft Graph, o utilizador ou administrador deve conceder-lhe as permissões corretas através de um processo de consentimento. [As permissões de referência do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listam as permissões associadas a cada conjunto principal de APIs do Gráfico microsoft. Também fornece orientações sobre como usar as permissões.

**Configurar ou atualizar o principal do serviço**

- [Criar serviçoprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Este artigo mostra-lhe como criar um novo objeto de serviçoPrincipal.
- [Criar uma aplicação AD AD & principal no portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - Este artigo mostra-lhe como criar uma nova aplicação e principal de serviço Azure Ative Directory (Azure AD) que pode ser usado com o controlo de acesso baseado em funções.
- [Aplicações & os principais do serviço em Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - Este artigo descreve o registo de aplicações, objetos de aplicação e diretores de serviço no Azure Ative Directory: o que são, como são usados e como estão relacionados uns com os outros.

**Adicionar ou atualizar o registo de aplicações e fornecer consentimento administrativo**

- [Criar um registo de aplicações](https://docs.microsoft.com/graph/api/application-post-applications) - Este artigo mostra-lhe como criar um novo objeto de aplicação.
- [Atualizar um registo de aplicações - permissões API](https://docs.microsoft.com/graph/api/application-update) - Este artigo mostra-lhe como atualizar as propriedades de um objeto de aplicação.
- [Fornecer consentimento administrativo](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Para consentimento administrativo e consentimento em geral, exigimos que um administrador conceda explicitamente o consentimento.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Recipiente de gestão de funções para definições de funções unificadas e atribuições de funções para fornecedores RBAC microsoft 365 que suportam múltiplos principais e múltiplos âmbitos numa única atribuição de funções. Isto é diferente do tipo de recurso *rbacApplication.* O Microsoft Intune é um exemplo de tal fornecedor de RBAC. Uma atribuição de papel em Intune pode ter uma variedade de principais e uma variedade de grupos de âmbito. **Isto está em versão beta, o que significa que ainda está em desenvolvimento e não é recomendado para utilização na produção.**
