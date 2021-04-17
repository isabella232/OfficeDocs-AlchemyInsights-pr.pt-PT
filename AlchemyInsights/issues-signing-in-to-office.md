---
title: Problemas de sessão nas aplicações da Microsoft 365
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833050"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Ecrã de sindução em branco nas aplicações da Microsoft 365

Para corrigir este problema, experimente o seguinte:
- Instale as atualizações mais recentes para [windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Redefinir as opções do Internet Explorer: Vá a **Ferramentas**  >  **Opções** de Internet  >    >  **Versões avançadas do Internet Reset (note** que perderá as definições personalizadas) e tente iniciar novamente a sessão no Office.
- Desative a Proteção de Aplicações do Windows Defender (WDAG) ou qualquer programa semelhante de firewall ou antivírus:
    1. No Painel de Controlo, vá a Programas e, em seguida, escolha as **funcionalidades** **Turn Windows ligados ou desligados**.
    2. Se o Windows Defender Application Guard estiver ativado, tente desativá-lo.<br/>
    **Nota:** Pode ser necessário reiniciar o computador.
- Certifique-se de que o plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) não está a ser bloqueado por qualquer aplicação ou programa de firewall/antivírus.
- [Credenciais de Escritório Claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando Gestor credencial do Windows.<br/>
    **Nota:** Os percursos de registo do Office 2016 mudaram para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identidade\)

Para obter mais informações, consulte [os problemas de ligação no sôm-in após a atualização do Office 2016 construir 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).