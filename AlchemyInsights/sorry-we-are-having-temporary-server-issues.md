---
title: Corrigir aplicações da Microsoft 365 Desculpe, estamos tendo mensagem temporária de problemas de servidor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758256"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Correção das aplicações microsoft 365 "Desculpe, estamos tendo problemas temporários de servidor"

Se receber esta mensagem, experimente o seguinte:

1. Verifique as definições de firewall, antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações da Microsoft 365. Consulte [os intervalos de endereços URLs e IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ir para **start**  >  **run**e, em seguida, escrever **serviços.msc**. Certifique-se de que todos os seguintes serviços estão em funcionamento:
    - Configuração automática de dispositivos ligados à rede
    - Serviço de Lista de Rede
    - Consciência de localização da rede
    - Registo de eventos do Windows

Se um destes serviços não estiver a funcionar, tente iniciá-lo. Se tiver algum problema em iniciar o serviço, executar o seguinte comando abrindo um pedido de comando com permissões elevadas:

**sfc /scannow**

Depois de terminar este comando, reinicie o computador.

Para obter informações detalhadas, consulte ["Desculpe, não podemos ligar-nos à sua conta. Por favor, tente novamente mais tarde" erro quando ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).