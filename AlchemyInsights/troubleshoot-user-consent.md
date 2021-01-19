---
title: Resolução de problemas consentimento do utilizador
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901633"
---
# <a name="troubleshoot-user-consent"></a>Resolução de problemas consentimento do utilizador

1. Pode configurar como os utilizadores finais concordam com as aplicações através do Portal Azure ou PowerShell. Consulte [as definições de consentimento do Utilizador](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para obter mais informações.
1. Um administrador também pode usar a [API do Gráfico microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para conceder consentimento a permissões delegadas em nome de um único utilizador. Para mais informações, consulte [Obter acesso em nome de um utilizador](https://docs.microsoft.com/graph/auth-v2-user).
1. [Erros de Consentimento do Utilizador](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): este artigo discute erros que podem ocorrer durante o processo de consentimento para uma aplicação. Se estiver a resolver pedidos de consentimento inesperados que não contenham mensagens de erro, consulte [Cenários de Autenticação para Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).