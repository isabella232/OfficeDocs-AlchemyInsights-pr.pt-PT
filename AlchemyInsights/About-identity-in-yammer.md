---
title: Acerca da identidade no Yammer
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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918948"
---
# <a name="about-identity-in-yammer"></a>Acerca da identidade no Yammer

Recomenda-se que todas as redes esticam os seguintes passos para evitar problemas relacionados com a identidade:

1. Impor a Office 365 após aprovisionar as Microsoft 365 dos utilizadores no Azure AD para garantir que todos os utilizadores inscrevem a sua conta Microsoft 365 principal. Para mais informações, consulte [Impor a identidade Office 365 utilizador do Yammer utilizadores.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Consolidar múltiplas Yammer rede. As configurações Yammer legadas permitem que múltiplas Yammer de rede sejam ligadas a um inquilino. Para mais informações, consulte [Migração de rede – consolidar várias Yammer rede](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcionalmente, imponha o licenciamento para Yammer bloquear os utilizadores do Yammer se não tenham uma licença. Para mais informações, consulte [Gerir Yammer licenças de utilizador no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Por fim, audite a lista de utilizadores de redes Yammer antigas e suspenda utilizadores antigos. Recomenda-se que suspenda (desativar) os utilizadores em vez de os eliminar, uma vez que a eliminação é irreversível. Para mais informações, consulte [Auditar Yammer utilizadores em redes ligadas a utilizadores Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [Remover utilizadores.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Ao configurar Yammer utilizando estes passos, também estará pronto para configurar a sua rede Yammer para o Modo Nativo para Microsoft 365. Para mais informações, consulte Configurar a sua [rede Yammer para o Modo Nativo para Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).