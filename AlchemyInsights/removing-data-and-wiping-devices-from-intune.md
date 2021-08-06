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
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922256"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Desativar dados e apagar dispositivos do Intune

As ações remotas de Desativar Dispositivo e Eliminar Todos os Dados do Dispositivo podem ser utilizadas para remover dados da empresa geridos pelo Intune ou para executar uma reposição de fábrica e restaurar o dispositivo para as suas definições padrão.

1. Inicie sessão na Gestão de Dispositivos do Microsoft 365, e aceda a **Dispositivos** > **Todos os Dispositivos**.
2. Selecione o dispositivo cujos dados pretende apagar.
3. Selecione o tipo de eliminação remota de dados que pretende efetuar. A desativação elimina apenas as informações da organização, ao passo que a eliminação de todos os dados repõe o dispositivo para as suas definições de fábrica.
4. Selecione **Sim** para confirmar. Até que o a eliminação de todos os dados esteja concluída, o estado de ação do Dispositivo é apresentado como *Desativação Pendente*.
    Após concluir a ação, deixará de ver o dispositivo móvel na lista de dispositivos geridos.

> [!NOTE]
> Os dados da empresa não podem ser removidos dos dispositivos ASSOCIADOS ao Azure AD. 

Para obter detalhes completos sobre o efeito das ações Desativar e Eliminar todos os dados, incluindo o que é retido e eliminado, consulte a seguinte documentação:

- [Remover dispositivos ao usar a eliminação de todos os dados, a desativação ou ao cancelar manualmente o registo do dispositivo](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Como eliminar apenas os dados empresariais de aplicações geridas pelo Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Eliminar todos os dados de um dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).