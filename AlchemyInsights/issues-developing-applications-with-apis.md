---
title: Questões que desenvolvem aplicações com APIs
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975014"
---
# <a name="issues-developing-applications-with-apis"></a>Questões que desenvolvem aplicações com APIs

Para começar a utilizar o Azure Ative Directory Graph API, consulte o [guia de arranque rápido Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , ou veja a [documentação de referência interativa AZure AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Fim do suporte para Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**

**A partir de 30 de junho de 2020,** deixaremos de adicionar novidades ao ADAL e ao Azure AD Graph. Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.

**A partir de 30 de junho de 2022,** terminaremos o suporte ao ADAL e ao Azure AD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.

As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não receberão qualquer suporte técnico ou atualizações de segurança.

As aplicações que utilizam o Azure AD Graph após este tempo podem deixar de receber respostas do ponto final do Azure AD Graph.

**Migração ADAL**

Recomendamos a atualização para a Biblioteca de Autenticação da [Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)que possui as mais recentes funcionalidades e atualizações de segurança.

Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está em processo de migrar as suas aplicações para o MSAL até ao fim do prazo de suporte, garantindo que beneficiará da segurança contínua da MSAL e das melhorias de funcionalidades.

1. [Leia as FAQ ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Saiba como migrar aplicações por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Se precisar de ajuda para entender quais das suas aplicações usam ADAL, recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações ADAL não-Microsoft no seu inquilino.

**Migração de gráficos AAD**

Para aplicações que estão a usar o Azure AD Graph, siga as nossas orientações para migrar [aplicações AD AD para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [A nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. O portal de registo de aplicações Azure mostra quais as aplicações que estão a utilizar o AAD Graph. Recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações. O suporte da Microsoft também pode fornecer-lhe uma lista de todos os usos de gráficos AAD no seu inquilino.
1. Para que a sua aplicação aceda a dados no Microsoft Graph, o utilizador ou administrador deve conceder-lhe as permissões corretas através de um processo de consentimento. As [permissões de referência do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) listam as permissões associadas a cada conjunto principal de APIs do Gráfico microsoft. Também fornece orientações sobre como usar as permissões.
