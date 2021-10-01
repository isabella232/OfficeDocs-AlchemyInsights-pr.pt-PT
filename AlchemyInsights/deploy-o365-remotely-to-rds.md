---
title: Implementar Microsoft 365 Apps para Grandes Empresas para utilização partilhada em RDS, Servidor de Terminal ou VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041017"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementar Microsoft 365 Apps para Grandes Empresas para utilização partilhada em RDS, Servidor de Terminal ou VDI

Para implementar o Microsoft 365 Apps a utilização dos Serviços de Ambiente de Trabalho Remoto (RDS), anteriormente utilizados os Serviços de Terminal, tem de:

- Utilize a correção fácil para ativar o TLS 1.2 como predefinição se estiver a executar uma versão anterior do Windows (por exemplo, Windows 7 SP1, Windows Server 2008 R2). Para uma correção fácil e mais informações, consulte Atualizar para ativar o [TLS 1.1 e o TLS 1.2 como protocolos seguros predefinido no WinHTTP no Windows](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy). 
- Tenha um plano que inclua Microsoft 365 Apps para Grandes Empresas (anteriormente Office 365 Plus). Por exemplo, Office 365 E3 ou Microsoft 365 E5 ou qualquer plano que inclua a versão de ambiente de trabalho do Project ou Visio, como o Project (Plano 3) ou Visio (Plano 2) ou o plano Microsoft 365 Empresas Premium, que também inclui Microsoft 365 Apps para Pequenas e Médias Empresas.
- Ativar a ativação do computador partilhado. Para obter mais informações, consulte [Resumo da ativação do computador partilhado para o Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Nota:** para instalar o Microsoft 365 Apps no modo de ativação do computador partilhado, transfira e execute [o Microsoft Assistente de Recuperação e Suporte](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Para obter detalhes sobre pré-requisitos, instruções de configuração e orientações para personalizar instalações com a Ferramenta de Implementação do Office, consulte Implementar o [Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)através dos Serviços de Ambiente de Trabalho Remoto.

Para corrigir erros relacionados com a ativação de computadores partilhados, consulte:

- [Remova problemas com a ativação do computador partilhado Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Repor Aplicações Microsoft 365 para estado de ativação para empresas](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Se quiser instalar o Microsoft 365 Apps RDS a partir do centro de administração do Microsoft 365, que utiliza as predefinições de instalação, siga estes passos:

1. Verifique que Microsoft 365 plano que tem. Para obter mais informações, [consulte Que subscrição tenho?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Se for necessário, mude para um plano Microsoft 365 diferente. Para obter mais informações, [consulte Atualizar para um plano diferente.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Se Microsoft 365 Apps já estiver instalado no servidor RDS com outros planos incompatíveis, desinstale-o indo ao Painel de Controlo  >  **Desinstalar um programa.** Se encontrar problemas, desinstale ao transferir o [Microsoft Assistente de Recuperação e Suporte](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. No servidor RDS, inscreva-se no servidor centro de administração do Microsoft 365 a sua conta de administrador e [instale a Office](https://portal.office.com/OLS/MySoftware.aspx).

   Após Office instalada, não abra ou inscreva-se em nenhuma Office aplicações.

1. No servidor RDS, ative o computador partilhado ao editar o registo:

   1. Clique com o botão direito Windows botão direito do rato no canto inferior esquerdo do seu ecrã e **selecione Executar**. Na caixa Abrir, escreva **regedit** e, em seguida, selecione **OK**.

   1. Quando lhe for pedido para permitir que o Editor de Registo faça alterações ao seu dispositivo, **selecione Sim.**

   1. No Editor de Registo, em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, adicione um valor de cadeia de texto **SharedComputerLicensing** com uma definição **de 1** .

1. No servidor RDS, instale-se como utilizador final e verifique se a ativação do computador partilhado está ativada para Microsoft 365 Apps. 

   Para obter detalhes, consulte [Verificar se a ativação do computador partilhado está ativada para Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).