---
title: Sobre a identidade em Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148306"
---
# <a name="about-identity-in-yammer"></a>Sobre a identidade em Yammer

Recomenda-se que todas as redes tomem as seguintes medidas para evitar questões relacionadas com a identidade:

1. Impor a identidade do Office 365 depois de ter disponibilizado as contas da Microsoft 365 para os utilizadores em Azure AD para garantir que todos os utilizadores acedam utilizando a sua conta primária da Microsoft 365. Para mais informações, consulte [a identidade do Enforce Office 365 para utilizadores da Yammer.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Consolidar várias redes Yammer. As configurações legacy Yammer permitem que várias redes Yammer sejam ligadas a um inquilino. Para obter mais informações, consulte [a migração da Rede - Consolidar várias redes Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcionalmente, imponha o licenciamento para a Yammer bloquear os utilizadores da Yammer se não tiverem licença. Para mais informações, consulte [as licenças de utilizador da Manage Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Por fim, audite a lista de utilizadores para redes Yammer mais antigas e suspenda os utilizadores antigos. Recomenda-se que suspenda (desativar) os utilizadores em vez de os eliminar, porque a eliminação é irreversível. Para obter mais informações, consulte [os utilizadores da Audit Yammer em redes ligadas ao Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [remover os utilizadores.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Ao configurar o Yammer usando estes passos, também estará pronto para configurar a sua rede Yammer para Modo Nativo para a Microsoft 365. Para obter mais informações, consulte [configurar a sua rede Yammer para Modo Nativo para a Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).