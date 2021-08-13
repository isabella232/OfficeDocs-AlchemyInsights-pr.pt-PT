---
title: Remova o consentimento do utilizador
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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007909"
---
# <a name="troubleshoot-user-consent"></a>Remova o consentimento do utilizador

1. Pode configurar a forma como os utilizadores finais consentem nas aplicações através do Portal do Azure ou do PowerShell. Consulte [Definições de consentimento do utilizador](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) para obter mais informações.
1. Um administrador também pode utilizar a [API Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) Microsoft para conceder consentimento às permissões delegadas em nome de um único utilizador. Para obter mais informações, [consulte Obter acesso em nome de um utilizador.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Erros de Consentimento do](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)Utilizador: este artigo aborda os erros que podem ocorrer durante o processo de consentimento para uma aplicação. Se estiver a remoção de pedidos de autorização inesperados que não contenham mensagens de erro, consulte Cenários de autenticação do [Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)