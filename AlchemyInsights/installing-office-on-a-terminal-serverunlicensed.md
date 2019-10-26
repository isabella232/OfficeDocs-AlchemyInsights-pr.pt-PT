---
title: Instalação de escritório em um servidor terminal - sem licença
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205420"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalação de escritório em um servidor terminal

Para implantar o Office 365 ProPlus em um servidor Windows usando serviços de desktop remoto (RDS), anteriormente chamado de Serviços terminais:
  
- Você deve ter um plano do Office 365 que inclua o Office 365 ProPlus, como o Office 365 Enterprise E3 ou o Enterprise E5. Os planos Office 365 Business and Office 365 Business Premium não incluem o Office 365 ProPlus.

- Você precisa ativar a [ativação do computador compartilhado.](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

Se você quiser instalar o Office 365 ProPlus no RDS do centro de administração Microsoft 365, que usa configurações de instalação padrão, use as ***seguintes etapas.***

> [!TIP]
> Você também pode baixar e executar o Assistente de [Suporte e Recuperação](https://aka.ms/SaRA_OfficeSCA_M365Portal) da Microsoft para instalar o Office 365 ProPlus no modo de ativação de computador compartilhado.
  
1. Verifique o plano do Office 365 que você tem. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessário, mude para um plano diferente do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Se o Office já estiver instalado no servidor RDS usando quaisquer outros planos do Office 365, desinstalá-lo. Por exemplo, indo \> para o Painel de Controle Desinstalar um programa. Desinstale o uso do [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver se deparando com problemas.

4. No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e instale o [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Depois que o Office for instalado, ***não abra ou entre em*** nenhuma inscrição no Office.

6. No servidor RDS, habilite a ativação compartilhada do computador editando o registro seguindo essas etapas:

1. Clique à direita no botão Do Windows no canto inferior esquerdo da tela e selecione Run. Na caixa aberta, tipo **regedit,** e selecione então APROVADO.

2. Selecione sim quando solicitado a permitir que o Editor de Registro faça alterações em seu dispositivo.

3. No editor de registro, adicione um valor de corda de **SharedComputerLicensing** com uma configuração de 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. No servidor RDS, ***entre como usuário final*** e verifique se a [ativação compartilhada do computador está ativada para o Office 365 ProPlus.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

Para obter mais detalhes sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas usando a ferramenta de implantação do office, [consulte o Deploy Office 365 ProPlus usando serviços de desktop remotos.](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)
  
Para corrigir erros relacionados à ativação compartilhada do computador, consulte problemas de [solução de problemas com ativação de computador compartilhada para o Office 365 ProPlus.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
  