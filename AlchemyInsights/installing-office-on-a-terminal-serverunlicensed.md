---
title: Instalar o Office num Servidor de Terminal - NãoLiceado
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322010"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalar Office num Servidor de Terminal

Para implementar o Microsoft 365 Apps para Grandes Empresas num servidor Windows utilizando os Serviços de Ambiente de Trabalho Remoto (RDS), anteriormente denominados Serviços de Terminal:
  
- Tem de ter uma subscrição Microsoft 365 subscrição que inclua Microsoft 365 Apps para Grandes Empresas, como o Office 365 Enterprise E3 ou Enterprise E5. Os Microsoft 365 Apps para Pequenas e Médias Empresas e Microsoft 365 Apps para Pequenas e Médias Empresas Premium planos não incluem Microsoft 365 Apps para Grandes Empresas.

- Tem de ativar [a ativação do computador partilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Se quiser instalar o Microsoft 365 Apps para Grandes Empresas RDS a partir do ***centro de administração do Microsoft 365,*** que utiliza as predefinições de instalação, utilize os seguintes passos.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Verifique o Microsoft 365 de subscrição que tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Se for necessário, mude para uma subscrição Microsoft 365 subscrição. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Se Office servidor RDS já estiver instalado com outras subscrições de Microsoft 365, desinstale-a. Por exemplo, ao ir para o Painel de \> Controlo, desinstale um programa. Desinstale [com o Microsoft Assistente de Recuperação e Suporte](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft se estiver a ter problemas.

4. No servidor RDS, inscreva-se no servidor centro de administração do Microsoft 365 a sua conta de administrador e [instale a Microsoft 365 Apps para Grandes Empresas](https://portal.office.com/OLS/MySoftware.aspx).

5. Após Office instalada, não ***abra ou inscreva-se*** em nenhuma Office aplicações.

6. No servidor RDS, ative o computador partilhado ao editar o registo ao seguir estes passos:

1. Clique com o botão direito Windows botão direito do rato no canto inferior esquerdo do seu ecrã e selecione Executar. Na caixa Abrir, escreva **regedit e, em** seguida, selecione OK.

2. Selecione Sim quando lhe for pedido para permitir que o Editor de Registo faça alterações ao seu dispositivo.

3. No Editor de Registo, adicione um valor de cadeia de **propriedade SharedComputerLicensing** com uma definição de 1 em \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. No servidor RDS, ***instale-se*** como utilizador final e verifique se a ativação do computador partilhado está ativada para [o Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Para obter mais detalhes sobre pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas com a Ferramenta de Implementação do Office, consulte Implementar o [Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)através dos Serviços de Ambiente de Trabalho Remoto.
  
Para corrigir erros relacionados com a ativação do computador partilhado, consulte Resolver problemas com a ativação do computador partilhado [para o Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  