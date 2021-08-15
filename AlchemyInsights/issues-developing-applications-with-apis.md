---
title: Problemas de desenvolvimento de aplicações com APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013471"
---
# <a name="issues-developing-applications-with-apis"></a>Problemas de desenvolvimento de aplicações com APIs

Para começar a utilizar a API do Azure Active Directory Graph, consulte o Guia de início rápido da API do [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ou consulte a documentação de referência da API interativa do [Azure AD Graph API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Fim do suporte da API Azure Active Directory ADAL (ADAL) e da API de AD Graph AAD (AAD Graph)**

**A partir de 30 de junho de 2020,** deixaremos de adicionar novas funcionalidades à ADAL e ao Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

A **partir de 30 de junho de 2022,** o suporte da ADAL e do Azure AD Graph deixará de fornecer suporte técnico ou atualizações de segurança.

As aplicações que utilizam o ADAL em versões existentes do SO continuarão a funcionar após esta data mas não terão suporte técnico ou atualizações de segurança.

As aplicações que utilizam o Azure AD Graph após este período de tempo poderão já não receber respostas do ponto final do Azure AD Graph atualização.

**Migração ADAL**

Recomendamos que atualize para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem as funcionalidades e atualizações de segurança mais recentes.

Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está no processo de migração das respassões para o MSAL até ao fim do prazo de suporte, assegurando que beneficiarão das melhorias contínuas de funcionalidades e segurança da MSAL.

1. [Leia as FAQ do ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Saiba mais sobre como migrar aplicações numa base por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Se precisar de ajuda para compreender que aplicações utilizam a ADAL, recomendamos que reveja o código fonte de todas as suas aplicações e, se aplicável, contacte quaisquer ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.

**Migração do AAD Graph**

Para as aplicações que utilizam o Azure AD Graph, siga as nossas orientações para migrar as [aplicações Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)para o Microsoft Graph .

1. [A nossa lista de verificação de migração inclui um ponto sobre introdução](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph. Recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os ISVs ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todos os serviços de utilização Graph AAD no seu inquilino.
1. Para que a sua aplicação aceda aos dados no Microsoft Graph, o utilizador ou administrador tem de lhe conceder as permissões corretas através de um processo de consentimento. O [Microsoft Graph de permissões lista](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) as permissões associadas a cada conjunto principal de APIs microsoft Graph. Também fornece orientações sobre como utilizar as permissões.
