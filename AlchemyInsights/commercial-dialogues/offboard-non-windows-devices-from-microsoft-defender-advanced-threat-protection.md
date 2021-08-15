---
title: Dispositivos que não Windows da Proteção Avançada Contra Ameaças (ATP) do Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967812"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Dispositivos que não Windows da Proteção Avançada Contra Ameaças (ATP) do Microsoft Defender

Faça o seguinte:

1. Siga a documentação de terceiros para desligar a solução de terceiros da ATP do Microsoft Defender.
2. A partir do Azure Active Directory do seu inquilino, remova as permissões para a solução de terceiros:

    1. Inicie sessão no [portal do Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. **Selecione Todos os** serviços  >  **Azure Active Directory**  >  **Enterprise Applications**.
    1. Selecione a aplicação que gostaria de desemborar.
    1. **Selecione Eliminar**.

Para saber mais, consulte [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).
