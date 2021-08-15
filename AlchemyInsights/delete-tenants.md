---
title: Eliminar inquilino
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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993904"
---
# <a name="delete-tenant"></a>Eliminar inquilino

Para eliminar um Azure AD, certifique-se de que:
- É um Administrador Global no diretório.
- NÃO tem a sua conta com a conta que tem o diretório predefinido, como o contoso.onmicrosoft.com na conta com assinatura assinada, como o admin@contoso.onmicrosoft.com.
- Remova todas as aplicações ativas no diretório antes de eliminar. Para remover aplicações ativas, navegue até Registos de aplicações e remova as aplicações existentes.
- Não existem subscrições ativas para quaisquer Serviços Online da Microsoft, como Microsoft Azure, Office 365 ou Azure AD Premium associados no diretório. Transfira as suas subscrições ou agilizar o cancelamento de subscrições ativas através do Suporte e Faturação do Azure. Saiba mais sobre Como Cancelar subscrições Office 365 e do Azure. Para orientação sobre como associar ou adicionar uma subscrição existente a um inquilino, consulte Associar ou adicionar uma subscrição do Azure ao seu inquilino do [Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Não existem licenças Ativas. Para remover licenças, consulte [Como remover a Subscrição para Remover licença.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Não existem outros utilizadores ativos no diretório além de si como Administrador Global ao tentar eliminar o Azure AD. Remova quaisquer outros utilizadores ativos e quaisquer dependências de um nome de domínio personalizado no inquilino também terão de ser removidas, como utilizadores criados com admin@contoso.com.

Para mais passos detalhados sobre como:
- Elimine "Azure Active Directory" ou "subscrição", consulte [Eliminar Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- A remover aplicações no diretório, consulte [Remover Aplicações.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
