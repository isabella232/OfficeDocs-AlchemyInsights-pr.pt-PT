---
title: Registo de dispositivo duplicado no portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814527"
---
# <a name="duplicate-device-record-in-the-portal"></a>Registo de dispositivo duplicado no portal

É possível que veja 2 registos de um dispositivo no portal se o dispositivo não reportar corretamente o estado de cogestão ao site do Gestor de Configuração. Para verificar o estado de cogestão de um dispositivo, consulte a coluna **Cogerido** do dispositivo na consola do Gestor de Configuração. Se a coluna não estiver visível, pode adicioná-la, ao clicar com o botão do rato em qualquer um dos cabeçalhos da coluna e selecioná-la a partir da lista.

O valor cogerido deve ser **Sim**. Se o valor for **Não**, abra a miniaplicação cliente do Gestor de Configuração no dispositivo cliente e verifique a propriedade **Cogestão** no separador Geral.

- Se o valor for **Ativado**, isso significa que existem problemas de comunicação do cliente com o Ponto de Gestão. Consulte o ficheiro **CcmMessaging.log** no dispositivo para investigar potenciais problemas de conectividade.

- Se o valor for **Desativado** e o dispositivo estiver inscrito no Intune, certifique-se de que o dispositivo recebeu a política de cogestão, ao rever o ficheiro **CoManagementHandler.log** no dispositivo.
