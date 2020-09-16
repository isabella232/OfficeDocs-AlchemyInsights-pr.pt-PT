---
title: Sobre a identidade em Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664181"
---
# <a name="about-identity-in-yammer"></a>Sobre a identidade em Yammer

Recomenda-se que todas as redes tomem as seguintes medidas para evitar questões relacionadas com a identidade:

1. Impor a identidade do Office 365 depois de ter disponibilizado as contas da Microsoft 365 para os utilizadores em Azure AD para garantir que todos os utilizadores acedam utilizando a sua conta primária da Microsoft 365. Para mais informações, consulte [a identidade do Enforce Office 365 para utilizadores da Yammer.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Consolidar várias redes Yammer. As configurações legacy Yammer permitem que várias redes Yammer sejam ligadas a um inquilino. Para obter mais informações, consulte [a migração da Rede - Consolidar várias redes Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcionalmente, imponha o licenciamento para a Yammer bloquear os utilizadores da Yammer se não tiverem licença. Para mais informações, consulte [as licenças de utilizador da Manage Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Por fim, audite a lista de utilizadores para redes Yammer mais antigas e suspenda os utilizadores antigos. Recomenda-se que suspenda (desativar) os utilizadores em vez de os eliminar, porque a eliminação é irreversível. Para obter mais informações, consulte [os utilizadores da Audit Yammer em redes ligadas ao Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [remover os utilizadores.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Ao configurar o Yammer usando estes passos, também estará pronto para configurar a sua rede Yammer para Modo Nativo para a Microsoft 365. Para obter mais informações, consulte [configurar a sua rede Yammer para Modo Nativo para a Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).