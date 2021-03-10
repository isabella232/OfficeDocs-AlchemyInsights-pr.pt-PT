---
title: Dispositivos não-Windows offboard do Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695156"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Dispositivos não-Windows offboard do Microsoft Defender Advanced Threat Protection (ATP)

Faça o seguinte:

1. Siga a documentação de terceiros para desligar a solução de terceiros do Microsoft Defender ATP.
2. Do seu inquilino Azure Ative Directory, remova permissões para a solução de terceiros:

    1. Inscreva-se no [portal Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Selecione **Todos os serviços**  >  **Azure Ative Directory**  >  **Enterprise Applications**.
    1. Selecione a aplicação que gostaria de embarcar.
    1. Selecione **Eliminar**.

Para saber mais, consulte [dispositivos não-Windows offboard](https://go.microsoft.com/fwlink/?linkid=2143630).
