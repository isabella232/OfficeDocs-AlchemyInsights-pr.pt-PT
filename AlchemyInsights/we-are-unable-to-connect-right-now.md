---
title: Problema de Ativação - Não podemos nos conectar agora
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806453"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Correção da mensagem das aplicações Microsoft 365 "Não conseguimos ligar-nos agora"

Se receber esta mensagem, experimente o seguinte:

1. Verifique as definições de firewall, antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações da Microsoft 365. Consulte [os intervalos de endereços Microsoft URLs e IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Ir para **start**  >  **run** e, em seguida, escrever **serviços.msc**. Certifique-se de que todos os seguintes serviços estão em funcionamento:
    - Configuração automática de dispositivos ligados à rede
    - Serviço de Lista de Rede
    - Consciência de localização da rede
    - Registo de eventos do Windows

Se um destes serviços não estiver a funcionar, tente iniciá-lo. Se tiver algum problema em iniciar o serviço, executar o seguinte comando abrindo um pedido de comando com permissões elevadas:

**sfc /scannow**

Depois de terminar este comando, reinicie o computador.

Para obter informações detalhadas, consulte ["Desculpe, não podemos ligar-nos à sua conta. Tente novamente mais tarde" erro quando ativar o Office a partir do Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).