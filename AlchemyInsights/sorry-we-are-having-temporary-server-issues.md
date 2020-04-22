---
title: Corrigir aplicativos do Office Desculpe, estamos tendo mensagens temporárias de problemas de servidor
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764128"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corrigir as aplicações do Office "Desculpe, estamos tendo problemas temporários de servidor" mensagem

Se receber esta mensagem, tente o seguinte:

1. Verifique as definições de firewall, software antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações do Office. Consulte [os intervalos urls e endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vá para **Iniciar** > **A Execução**, e, em seguida, digite **serviços.msc**. Certifique-se de que os seguintes serviços estão em execução:
    - Configuração automática de dispositivos ligados à rede
    - Serviço de Lista de Rede
    - Sensibilização para a localização da rede
    - Registo de Eventos do Windows

Se um destes serviços não estiver a funcionar, tente iniciá-lo. Se tiver algum problema em iniciar o serviço, faça o seguinte comando abrindo um pedido de comando com permissões elevadas:

**sfc /scannow**

Depois deste comando terminar, reinicie o computador.

Para obter informações detalhadas, consulte ["Desculpe, não podemos ligar-nos à sua conta. Tente novamente mais tarde" erro quando ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).