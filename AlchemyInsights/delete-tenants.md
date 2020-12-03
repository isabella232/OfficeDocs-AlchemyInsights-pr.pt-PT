---
title: Apagar inquilino
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564884"
---
# <a name="delete-tenant"></a>Apagar inquilino

Para eliminar um AD Azure, certifique-se:
- És administrador global no diretório.
- Não está inscrito numa conta que tenha o diretório por defeito, como contoso.onmicrosoft.com na conta de assinatura, como admin@contoso.onmicrosoft.com.
- Remova quaisquer aplicações ativas no diretório antes da eliminação. Para remover aplicações ativas, navegue para os registos da App e remova as aplicações existentes.
- Não existem subscrições ativas para quaisquer Serviços Microsoft Online, tais como Microsoft Azure, Office 365 ou Azure AD Premium associados no diretório. Transfira as suas subscrições ou acelere o cancelamento de subscrições ativas através do Suporte e Faturação do Azure. Saiba mais sobre como cancelar as assinaturas Do Office 365 e Azure. Para obter orientações sobre a associação ou a adição de uma subscrição existente a um inquilino, consulte [Associate ou adicione uma subscrição Azure ao seu inquilino AZure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Não há licença ativa. Para remover licenças, consulte [como remover a licença de Remoção de Assinaturas.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Não existem outros utilizadores ativos no diretório além de si mesmo como Administrador Global ao tentar eliminar o AD Azure. Remova quaisquer outros utilizadores ativos, e quaisquer dependências de um nome de domínio personalizado no inquilino também terão de ser removidas, como os utilizadores criados com admin@contoso.com.

Para mais detalhes, como:
- Eliminar "Azure Ative Directory" ou "subscription", ver [Delete Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Remover as aplicações no diretório, ver [Remoção de Aplicações](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
