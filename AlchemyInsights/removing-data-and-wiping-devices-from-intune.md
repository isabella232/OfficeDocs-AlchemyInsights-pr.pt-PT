---
title: Remoção de dados e dispositivos de limpeza do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440470"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Remoção de dados e dispositivos de limpeza do Intune

As ações remotas de remoção de dispositivos e limpeza de dispositivos podem ser utilizadas para remover os dados da empresa geridos pelo Intune ou para executar um reset de fábrica e devolver o dispositivo às suas definições predefinidas.

1. Inscreva-se na Microsoft 365 Device Management e vá para **dispositivos**  >  **todos os dispositivos**.
2. Selecione o dispositivo que pretende limpar.
3. Selecione o tipo de limpeza remota que pretende fazer. A aposentadoria elimina apenas informações organizacionais, enquanto as toalhetes completas devolvem o dispositivo às suas definições de fábrica.
4. Selecione **Sim** para confirmar. Até que a limpeza termine, o estado de ação do dispositivo mostra como Aposentadoria Pendente.</br>
    Depois de concluída a ação, deixará de ver o dispositivo móvel na lista de dispositivos geridos.

**Nota** Os dados da empresa não podem ser removidos dos dispositivos associados à Azure AD.

Para obter todos os detalhes sobre o efeito das ações retire e limpadoras, incluindo o que é retido e o que é eliminado, consulte [remover os dispositivos utilizando limpeza, aposentação ou desinsusamento manual do dispositivo](https://docs.microsoft.com/intune/devices-wipe).

Para apagar todos os dados de um dispositivo macOS, consulte [apagar todos os dados de um dispositivo macOS](https://docs.microsoft.com/intune/device-erase).