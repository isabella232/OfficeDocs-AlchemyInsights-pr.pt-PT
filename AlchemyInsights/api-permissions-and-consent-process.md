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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932072"
---
# <a name="api-permissions-and-consent-process"></a>Permissões da API e Processo de Consentimento

Para que a sua aplicação aceda aos dados no Microsoft Graph, o utilizador ou administrador tem de lhe conceder as permissões corretas através de um processo de consentimento. [A referência Graph permissões do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) lista as permissões associadas a cada conjunto principal de APIs Graph Microsoft. Também fornece orientações sobre como utilizar as permissões.

**Configurar ou atualizar principal de serviço**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Este artigo mostra-lhe como criar um novo objeto servicePrincipal.
- Criar um principal de serviço [da aplicação Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) no portal – este artigo mostra-lhe como criar uma nova aplicação e um principal de serviço do Azure Active Directory (Azure AD) que pode ser utilizado com o controlo de acesso baseado em funções.
- Aplicações & principais de serviço no [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – este artigo descreve o registo de aplicações, objetos de aplicação e principais de serviço no Azure Active Directory: o que são, como são utilizados e como estão relacionados entre si.

**Adicionar ou atualizar o registo de aplicações e fornecer autorização do administrador**

- [Criar um registo de aplicação](https://docs.microsoft.com/graph/api/application-post-applications) – este artigo mostra-lhe como criar um novo objeto de aplicação.
- [Atualizar um registo de aplicação – permissões da API](https://docs.microsoft.com/graph/api/application-update) – este artigo mostra-lhe como atualizar as propriedades de um objeto de aplicação.
- [Fornecer consentimento para administradores](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – para que o consentimento e consentimento do administrador seja geral, é necessário que um administrador conceda explicitamente o consentimento.
- [RBAC (beta) –](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) contentor de gestão de funções para definições de funções unificada e atribuições de funções Microsoft 365 para fornecedores RBAC que suportam múltiplos principais e múltiplos âmbitos numa única atribuição de funções. Isto é diferente do tipo *de recurso rbacApplication.* Microsoft Intune é um exemplo deste tipo de fornecedor de RBAC. Uma atribuição de funções no Intune pode ter uma matriz de principais e uma matriz de grupos de âmbito. **Isto está em beta, ou seja, que ainda está em desenvolvimento e não é recomendado para utilização na produção.**
