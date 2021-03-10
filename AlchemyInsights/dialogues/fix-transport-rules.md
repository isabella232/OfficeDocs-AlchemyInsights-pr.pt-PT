---
title: Fixar regras de transporte
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695858"
---
# <a name="fix-transport-rules"></a>Fixar regras de transporte

Uma regra de fluxo de correio personalizado afetou esta mensagem. Para rever a regra exata, faça o seguinte:

1. Nos resultados da submissão, em **informações adicionais,** note o **GUID** ou o **Nome De Política**.
2. Launch Exchange Management Shell. Para mais informações, consulte [Abrir a Shell de Gestão de Câmbios.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Executar este comando (utilizando o GUID a partir da sua submissão):  **Get-TransportRule -identidade "GUID" | fl * Descrição***
4. Reveja a descrição para ver as condições configuradas que afetaram a mensagem.

Para saber mais, consulte [a Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
