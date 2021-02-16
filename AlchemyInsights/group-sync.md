---
title: Sincronização de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256789"
---
# <a name="group-sync"></a>Sincronização de grupo

Este artigo fornece orientações sobre a sincronização de grupos.

1. Se um administrador global ou dono de grupo não for capaz de modificar propriedades de grupo ou adicionar membros ou atribuir proprietários no portal Azure, certifique-se de que a fonte da autoridade para o grupo é Azure Ative Directory (Azure AD) para o administrador global ou proprietário do grupo para modificar o grupo.
2. Antes de tentar eliminar um grupo sincronizado em Azure AD, certifique-se de que [apagou todas as licenças atribuídas](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) para evitar erros.

Para compreender como sincronizar utilizadores, grupos e contactos, consulte [o Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)e siga [sincronizar um grupo no local para a Azure utilizando o Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) para sincronizar grupos on-perm utilizando a ligação AD.

Siga este guia [Erros de resolução de problemas durante](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) a sincronização para resolver erros comuns durante a sincronização.

