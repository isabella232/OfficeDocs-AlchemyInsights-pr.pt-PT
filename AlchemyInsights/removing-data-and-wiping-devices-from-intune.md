---
title: Desativar dados e apagar dispositivos do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331052"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Desativar dados e apagar dispositivos do Intune

As ações remotas de Desativar Dispositivo e Eliminar Todos os Dados do Dispositivo podem ser utilizadas para remover dados da empresa geridos pelo Intune ou para executar uma reposição de fábrica e restaurar o dispositivo para as suas definições padrão.

1. Inicie sessão na Gestão de Dispositivos do Microsoft 365, e aceda a **Dispositivos** > **Todos os Dispositivos**.
2. Selecione o dispositivo cujos dados pretende apagar.
3. Selecione o tipo de eliminação remota de dados que pretende efetuar. A desativação elimina apenas as informações da organização, ao passo que a eliminação de todos os dados repõe o dispositivo para as suas definições de fábrica.
4. Selecione **Sim** para confirmar. Até que o a eliminação de todos os dados esteja concluída, o estado de ação do Dispositivo é apresentado como *Desativação Pendente*.
    Após concluir a ação, deixará de ver o dispositivo móvel na lista de dispositivos geridos.

**Nota:** os dados da empresa não podem ser removidos dos dispositivos JOINED para o Azure AD. 

Para obter detalhes completos sobre o efeito das ações Desativar e Eliminar todos os dados, incluindo o que é retido e eliminado, consulte a seguinte documentação:

- [Remover dispositivos ao usar a eliminação de todos os dados, a desativação ou ao cancelar manualmente o registo do dispositivo](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Como eliminar apenas os dados empresariais de aplicações geridas pelo Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Eliminar todos os dados de um dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).