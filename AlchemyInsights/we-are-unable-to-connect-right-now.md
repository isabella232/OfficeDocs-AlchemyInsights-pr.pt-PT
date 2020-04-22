---
title: Problema de Ativação - Não conseguimos ligar-nos agora
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716183"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Corrigir as aplicações do Office "Não conseguimos ligar agora"

Se receber esta mensagem, tente o seguinte:

1. Verifique as definições de firewall, software antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações do Office. Consulte [os urLs da Microsoft e os intervalos](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)de endereços IP .

2. Vá para **Iniciar** > **A Execução**, e, em seguida, digite **serviços.msc**. Certifique-se de que os seguintes serviços estão em execução:
    - Configuração automática de dispositivos ligados à rede
    - Serviço de Lista de Rede
    - Sensibilização para a localização da rede
    - Registo de Eventos do Windows

Se um destes serviços não estiver a funcionar, tente iniciá-lo. Se tiver algum problema em iniciar o serviço, faça o seguinte comando abrindo um pedido de comando com permissões elevadas:

**sfc /scannow**

Depois deste comando terminar, reinicie o computador.

Para obter informações detalhadas, consulte ["Desculpe, não podemos ligar-nos à sua conta. Tente novamente mais tarde" erro quando activao o Office a partir do Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).