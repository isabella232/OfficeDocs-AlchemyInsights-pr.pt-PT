---
title: Corrigindo aplicativos do Office Desculpe, estamos tendo mensagem temporária de problemas de servidor
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628001"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corrigindo os aplicativos do Office "Desculpe, estamos tendo problemas temporários de servidor" mensagem

Se você receber esta mensagem, tente o seguinte:

1. Verifique seu firewall, software antivírus e configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet aos aplicativos do Office. Veja [o Office 365 URLs e as faixas](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)de endereço IP.

2. Vá para **iniciar** > **a corrida,** e depois digite **services.msc**. Certifique-se de que os seguintes serviços estão todos em execução:
    - Configuração automática de dispositivos conectados à rede
    - Serviço de lista de rede
    - Conscientização de localização da rede
    - Registro do evento de Windows

Se um desses serviços não estiver funcionando, tente iniciá-lo. Se você tiver um problema para iniciar o serviço, execute o comando a seguir, abrindo uma solicitação de comando com permissões elevadas:

**sfc /scannow Sfc / scannow**

Após este comando terminar, reinicie o computador.

Para obter informações detalhadas, [consulte "Desculpe, não podemos nos conectar à sua conta. Por favor, tente novamente mais tarde" erro quando você ativar office do Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).