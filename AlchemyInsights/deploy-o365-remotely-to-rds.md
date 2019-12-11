---
title: Implantação do Office 365 ProPlus para uso compartilhado em RDS, Terminal Server ou VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959470"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implantação do Office 365 ProPlus para uso compartilhado em RDS, Terminal Server ou VDI

Para implantar o Office 365 ProPlus usando serviços de desktop remoto (RDS), anteriormente chamado de Serviços terminais:
- Você deve ter um plano Microsoft 365 For Business ou um plano do Office 365 que inclua o Office 365 ProPlus, como o Office 365 Enterprise E3 ou o Enterprise E5.
   > [!NOTE] 
   > Os planos Office 365 Business and Office 365 Business Premium não incluem o Office 365 ProPlus.
- Você deve habilitar a [ativação do computador compartilhado.](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

> [!NOTE]
> Você também pode baixar e executar o Assistente de [Suporte e Recuperação](https://aka.ms/SaRA_OfficeSCA_M365Portal) da Microsoft para instalar o Office 365 ProPlus no modo de ativação de computador compartilhado.

Para obter mais informações sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas usando a ferramenta de implantação do office, [consulte o Deploy Office 365 ProPlus usando serviços](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)de desktop remotos.

Corrigir erros relacionados à ativação do computador compartilhado:
- Veja problemas de [solucionação de problemas com ativação de computador compartilhado para o Office 365 ProPlus.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
- Veja o estado de [ativação do Reset Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Se você quiser instalar o Office 365 ProPlus no RDS do centro de administração Microsoft 365, que usa configurações de instalação padrão, use as ***seguintes etapas:***

1.  Verifique o plano do Office 365 que você tem. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Se necessário, mude para um plano diferente do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Se o Office já estiver instalado no servidor RDS usando quaisquer outros planos do Office 365, desinstalá-lo. Por exemplo, indo para **o Painel** > de Controle**desinstalar um programa**. Desinstale o uso do [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver se deparando com problemas.
4.  No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e instale o [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Depois que o Office for instalado, ***não abra ou entre em*** nenhuma inscrição no Office.
6.  No servidor RDS, habilite a ativação compartilhada do computador editando o registro seguindo essas etapas:
   1. Clique à direita no botão Do Windows no canto inferior esquerdo da tela e selecione **Run**. Na caixa aberta, tipo **regedit,** e selecione então **APROVADO.**
   2. Selecione **sim** quando solicitado a permitir que o Editor de Registro faça alterações em seu dispositivo.
   3. No editor de registro, adicione um valor de corda de **SharedComputerLicensing** com uma configuração de 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. No servidor RDS, ***entre como usuário final*** e verifique se a [ativação compartilhada do computador está ativada para o Office 365 ProPlus.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

