---
title: Localizar dispositivos iOS perdidos com o Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440425"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Localizar dispositivos iOS perdidos com o Intune

Ativar o modo perdido num dispositivo iOS permite que um administrador tenha uma mensagem e um número de telefone de contacto apresentados no ecrã de bloqueio.

Depois de o modo perdido ser ativado, o administrador pode utilizar a ação do dispositivo Localizar para identificar a localização física do dispositivo.

A ação do dispositivo Localizar no Intune funciona com dispositivos iOS para mostrar a localização de um dispositivo específico num mapa.

A utilização desta ação requer que o dispositivo iOS esteja em:

- Modo supervisionado
- Modo perdido

Para obter mais informações, consulte [Ativar o modo perdido em dispositivos iOS/iPadOS com dispositivos Intune](https://docs.microsoft.com/intune/device-lost-mode) e [Localizar dispositivos iOS/iPadOS perdidos ou roubados com Intune](https://docs.microsoft.com/intune/device-locate).

**FAQ**

P: Emiti uma ação remota para remover os dados da empresa de um dispositivo, e agora está preso num estado pendente.

R: Para uma ação remota para completar com sucesso, o dispositivo direcionado deve estar online e saudável. Nas seguintes situações, a ação remota permanece em estado pendente durante 30 dias, ou até que o dispositivo reconheça o comando:

- Quando o dispositivo não tem conectividade
- Quando o dispositivo perde o seu estatuto de gestão com a Intune

Se achar que um dispositivo já não está a fazer o check-in e que não será capaz de remover os dados da empresa, selecione Delete. A eliminação remove o registo do dispositivo de modo a que não apareça mais na lista de dispositivos Intune. Se o dispositivo voltar a funcionar, o utilizador terá de o reinscrevê-lo.

P: Porque é que certas ações remotas não estão disponíveis para eu usar?

R: Nem todas as plataformas suportam todas as ações de dispositivos remotos. As seguintes ações remotas são específicas da plataforma, pelo que estão disponíveis apenas para as plataformas notadas.

- Bloqueio de ativação do bypass (apenas iOS)
- Início Fresco (apenas janelas)
- Modo perdido (apenas iOS)
- Localizar dispositivo (apenas iOS)
- Reiniciar (apenas para windows)

Para obter mais detalhes sobre cada ação, consulte [as ações do dispositivo disponíveis.](https://docs.microsoft.com/intune/device-management#available-device-actions)