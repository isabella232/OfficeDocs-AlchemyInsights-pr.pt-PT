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
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004165"
---
# <a name="duplicate-device-record-in-the-portal"></a>Registo de dispositivo duplicado no portal

É possível que veja 2 registos de um dispositivo no portal se o dispositivo não reportar corretamente o estado de cogestão ao site do Gestor de Configuração. Para verificar o estado de cogestão de um dispositivo, consulte a coluna **Cogerido** do dispositivo na consola do Gestor de Configuração. Se a coluna não estiver visível, pode adicioná-la, ao clicar com o botão do rato em qualquer um dos cabeçalhos da coluna e selecioná-la a partir da lista.

O valor cogerido deve ser **Sim**. Se o valor for **Não**, abra a miniaplicação cliente do Gestor de Configuração no dispositivo cliente e verifique a propriedade **Cogestão** no separador Geral.

- Se o valor for **Ativado**, isso significa que existem problemas de comunicação do cliente com o Ponto de Gestão. Consulte o ficheiro **CcmMessaging.log** no dispositivo para investigar potenciais problemas de conectividade.

- Se o valor for **Desativado** e o dispositivo estiver inscrito no Intune, certifique-se de que o dispositivo recebeu a política de cogestão, ao rever o ficheiro **CoManagementHandler.log** no dispositivo.
