---
title: Corrigir aplicações da Microsoft 365 Desculpe, estamos tendo mensagem temporária de problemas de servidor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582714"
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