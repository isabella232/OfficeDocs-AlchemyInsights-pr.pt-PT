---
title: Bloqueio de ativação de bypass em dispositivos iOS supervisionados com Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424216"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Bloqueio de ativação de bypass em dispositivos iOS supervisionados com Intune

A capacidade de contornar o bloqueio de ativação nos dispositivos iOS facilita a recuperação do cenário em que um utilizador permite o bloqueio de ativação num dispositivo corporativo e, em seguida, sai da empresa.

Os requisitos necessários para contornar um bloqueio de ativação incluem:

- Um dispositivo é "supervisionado".
- O bloqueio de ativação é ativado com sucesso utilizando a política de restrição do dispositivo iOS no Intune.

Além disso, ao contornar um bloqueio de ativação, deve:

- Possuir fisicamente o dispositivo a ser limpo.
- Copie o código antes de emitir a limpeza.

**Nota:** O código de limpeza não é sensível a casos, pelo que os caracteres "-" não são necessários.

Para mais informações, consulte o Bloqueio de [Ativação do Bypass em dispositivos iOS supervisionados com o Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**FAQ**

P: **Emiti uma ação remota para remover os dados da empresa de um dispositivo, e agora está preso num estado pendente.**

R: Para uma ação remota para completar com sucesso, o dispositivo direcionado deve estar online e saudável. Nas seguintes situações, a ação remota permanece em estado pendente durante 30 dias, ou até que o dispositivo reconheça o comando quando o dispositivo:

- Não tem conectividade.
- Perde o seu estatuto de gestão com a Intune.

Se achar que um dispositivo já não está a fazer o check-in e que não removerá os dados da empresa, selecione Delete. A eliminação remove o registo do dispositivo de modo a que não apareça mais na lista de dispositivos Intune. Para que o dispositivo volte a funcionar, o seu utilizador deve voltar a inscrever o dispositivo.

P: **Porque é que certas ações remotas não estão disponíveis para eu usar?**

R: Nem todas as plataformas suportam todas as ações de dispositivos remotos. As seguintes ações remotas são específicas da plataforma.

- Bloqueio de ativação do bypass (apenas iOS)
- Início Fresco (apenas janelas)
- Modo perdido (apenas iOS)
- Localizar dispositivo (apenas iOS)
- Reiniciar (apenas para windows)

Para obter mais detalhes sobre cada ação, consulte [as ações do dispositivo disponíveis.](https://docs.microsoft.com/intune/device-management#available-device-actions)