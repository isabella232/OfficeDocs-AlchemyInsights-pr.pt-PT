---
title: Problemas de consentimento do administrador
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
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952584"
---
# <a name="admin-consent-issues"></a>Problemas de consentimento do administrador

1. Ative [o fluxo de trabalho de consentimento do administrador](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) para permitir que os utilizadores peçam aprovação de administrador diretamente a partir do ecrã de consentimento.

1. Se o utilizador ou os utilizadores da sua aplicação estiverem a detetar erros inesperados durante o processo de consentimento, consulte este artigo para ver os passos de remoção de problemas: Erro inesperado ao executar consentimento numa [aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Saiba mais sobre a Autorização do administrador no [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [plataforma de identidades da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), como funciona o pedido de autorização e como avaliar um pedido de autorização do administrador para toda a área [do inquilino.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. As aplicações integradas com plataforma de identidades da Microsoft seguem um modelo de autorização que permite aos utilizadores e administradores controlar a forma como os dados podem ser acetidos. A implementação do modelo de autorização foi atualizada no ponto final da plataforma de identidades da Microsoft e altera a forma como uma aplicação tem de interagir com a plataforma de identidades da Microsoft. Consulte [Permissões e consentimento no ponto final plataforma de identidades da Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) para obter uma visão geral deste modelo de autorização, incluindo âmbitos, permissões e consentimento.