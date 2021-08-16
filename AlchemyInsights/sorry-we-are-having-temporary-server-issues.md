---
title: Corrigir Microsoft 365 aplicações Lamentamos, mas estamos a ter problemas temporários com o servidor
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021607"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corrigir a mensagem Microsoft 365 aplicações "Lamentamos, mas estamos a ter problemas temporários com o servidor"

Se receber esta mensagem, experimente o seguinte:

1. Verifique a sua firewall, software antivírus e definições de proxy para confirmar que não estão a bloquear o acesso à Internet a Microsoft 365 aplicações. Consulte [Intervalos de URLs e endereços IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Vá para **Iniciar**  >  **Executar e,** em seguida, **escreva services.msc**. Certifique-se de que os seguintes serviços estão todos em execução:
    - Configuração Automática de Dispositivos Ligados à Rede
    - Serviço de Lista de Rede
    - Sensibilização sobre a Localização da Rede
    - Windows Registo de Eventos

Se um destes serviços não estiver em execução, tente iniciá-lo. Se tiver problemas ao iniciar o serviço, execute o seguinte comando ao abrir uma linha de comandos com permissões elevadas:

**sfc /scannow**

Quando este comando terminar, reinicie o computador.

Para obter informações detalhadas, [consulte "Lamentamos, mas não é possível ligar à sua conta. Erro tente novamente mais tarde" ao ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).