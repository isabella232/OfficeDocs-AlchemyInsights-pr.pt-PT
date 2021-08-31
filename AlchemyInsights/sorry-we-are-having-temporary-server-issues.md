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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744678"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corrigir a mensagem Microsoft 365 aplicações "Lamentamos, mas estamos a ter problemas temporários com o servidor"

Nota: se estiver a utilizar uma versão mais antiga do Windows (por exemplo, Windows 7 SP1, Windows Server [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 2008 R2), utilize a correção fácil para ativar o TLS 1.2 como predefinição. Para obter mais informações, consulte Update [to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

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