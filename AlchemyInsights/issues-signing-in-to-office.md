---
title: Problemas ao inscrever-se Microsoft 365 aplicações
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
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088047"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Ecrã de sign-in em branco Microsoft 365 aplicações

Para corrigir este problema, experimente o seguinte:
- Instale as atualizações mais [recentes Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Repor as opções do Internet Explorer: Vá para Ferramentas Opções da Internet Repor o  >    >    >  **Internet Explorer Definições** (tenha em atenção que perderá as definições personalizadas) e, em seguida, tente entrar novamente no Office.
- Desativar a Windows Defender Application Guard (WDAG) ou qualquer programa de antivírus ou firewall semelhante:
    1. No Painel de Controlo, vá para Programas e, em **seguida,** selecionar A Windows **funcionalidades de desligá-los**.
    2. Se a Windows Defender Application Guard estiver ativada, experimente desatiná-la.<br/>
    **Nota:** Poderá ter de reiniciar o computador.
- Certifique-se de que o plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) não está a ser bloqueado por qualquer aplicação ou programa de firewall/antivírus.
- [Limpe Office de credenciais utilizando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) o Windows de Credenciais.<br/>
    **Nota:** Os caminhos de registo Office 2016 mudaram para 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Para obter mais informações, consulte Problemas de ligação ao inscrever-se após a atualização para [a comarca 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)do Office Windows 10 .