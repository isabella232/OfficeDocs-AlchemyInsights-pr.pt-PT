---
title: Problemas de início de sessão em aplicações do Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938303"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Ecrã de início de sessão em branco em aplicações do Office

Para corrigir este problema, tente o seguinte:
- Instale as actualizações mais recentes para o [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Repor Opções do Internet Explorer: vá para **Ferramentas** > **Opções da Internet** > **Avançadas** > **Repor definições do Internet Explorer** (note que irá perder as definições personalizadas) e, em seguida, tente iniciar novamente sessão no Office.
- Desactive o Windows Defender aplicação Guard (WDAG) ou qualquer programa de firewall ou antivírus semelhante:
    1. No painel de controlo, vá para **programas**e, em seguida, escolha **Activar funcionalidades do Windows ou desactivar**.
    2. Se estiver activada a protecção de aplicação do Windows Defender, tente desactivá-la.<br/>
    **Nota:** Tem de reiniciar o computador.
- Certifique-se de que a Microsoft.AAD.BrokerPlugin [Das WAM Plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) não está a ser bloqueado por qualquer aplicação ou programa de firewall/anti-antivírus.
- [Office Limpar credenciais](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizando o Gestor de credenciais do Windows.<br/>
    **Nota:** Os caminhos de registo para o Office 2016 foram alterados para 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Para mais informações, consulte [problemas de ligação no início de sessão-in após a actualização do Office de 2016 compilação 16.0.7967 10 do Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).