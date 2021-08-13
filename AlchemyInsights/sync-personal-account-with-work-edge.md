---
title: Permitir que um utilizador sincronizar uma conta pessoal com a conta de trabalho no Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813403"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Permitir que um utilizador sincronizar uma conta pessoal com a conta de trabalho no Microsoft Edge

Certifique-se de que cumpre estes critérios:

- O Roaming de Estado da Empresa está ativado no centro de administração Azure Active Directory, o que requer uma subscrição para Azure Active Directory Premium ou Enterprise Mobility + Security (EMS). Para mais informações, consulte [Enable Enterprise State Roaming in Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Um ou ambos os seguintes critérios são cumpridos:
    - O serviço Azure Information Protection está ativado para o seu inquilino. Para obter detalhes, consulte [Ativar a proteção do Azure Rights Management a partir da centro de administração do Microsoft 365.](/azure/information-protection/activate-office365)
    - A Azure Active Directory Roaming do Estado da Empresa (ESR) está ativada para qualquer utilizador ou inquilino. Para mais informações, consulte O [que é o roaming de estado empresarial?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Se o AIP e o ESR estiverem ambos desativados, uma mensagem de erro informa os utilizadores de que a sincronização não está disponível para as respetivos contas.
