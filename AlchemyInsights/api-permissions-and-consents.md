---
title: Permissões e Consentimento da API
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974990"
---
# <a name="api-permissions-and-consent"></a>Permissões e consentimento da API

As aplicações que se integram com a plataforma de identidade da Microsoft seguem um modelo de autorização que dá aos utilizadores e administradores o controlo sobre a forma como os dados podem ser acedidos. A implementação do modelo de autorização foi atualizada no ponto final da plataforma de identidade da Microsoft. Altera a forma como uma aplicação deve interagir com a plataforma de identidade da Microsoft. [Permissões e consentimento no ponto final da plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) abrange os conceitos básicos deste modelo de autorização, incluindo âmbitos, permissões e consentimento.

O [quadro de consentimento do Azure Ative Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita o desenvolvimento de aplicações de clientes multi-inquilinos e clientes nativos. Estas aplicações permitem a inscrição por conta de utilizador de um inquilino AZure AD que é diferente daquele em que a aplicação está registada. Podem também ter de aceder a APIs web, como a API do Microsoft Graph (para aceder a Azure AD, Intune e serviços na Microsoft 365) e a APIs de outros serviços da Microsoft, além das suas próprias APIs web.

