---
title: Questões de consentimento administrativo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901508"
---
# <a name="admin-consent-issues"></a>Questões de consentimento administrativo

1. Ativar o [fluxo de trabalho](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) de consentimento administrativo para permitir que os utilizadores solicitem a aprovação do administrador diretamente a partir do ecrã de consentimento.

1. Se você ou os utilizadores da sua aplicação estiverem a ver erros inesperados durante o processo de consentimento, consulte este artigo para etapas de resolução de problemas: [Erro inesperado ao efetuar o consentimento de uma aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Saiba mais sobre [o consentimento do Administrador na plataforma de identidade da Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)como funciona o pedido de [consentimento](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) e como avaliar um pedido de consentimento administrativo em todo [o cliente](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. As aplicações que se integram com a plataforma de identidade da Microsoft seguem um modelo de autorização que dá aos utilizadores e administradores o controlo sobre a forma como os dados podem ser acedidos. A implementação do modelo de autorização foi atualizada no ponto final da plataforma de identidade da Microsoft, e altera a forma como uma aplicação deve interagir com a plataforma de identidade da Microsoft. Consulte [permissões e consentimento no ponto final da plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) para uma visão geral deste modelo de autorização, incluindo âmbitos, permissões e consentimento.