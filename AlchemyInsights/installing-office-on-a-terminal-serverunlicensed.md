---
title: Instalando o Office em um servidor de terminal-não licenciado
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
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205420"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalando o Office em um servidor de terminal

Para implantar o Office 365 ProPlus em um Windows Server usando serviços de área de trabalho remota (RDS), anteriormente denominados serviços de terminal:
  
- Você deve ter um plano do Office 365 que inclua o Office 365 ProPlus, como o Office 365 Enterprise E3 ou o Enterprise e5. Os planos Office 365 Business e Office 365 Business Premium não incluem o Office 365 ProPlus.

- Você precisa ativar a [ativação do computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Se pretender instalar o Office 365 ProPlus no RDS a partir do centro de administração do Microsoft 365, ***que utiliza as definições de instalação predefinidas***, utilize os seguintes passos.

> [!TIP]
> Você também pode baixar e executar o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar o Office 365 ProPlus no modo de ativação de computador compartilhado.
  
1. Verifique o plano do Office 365 que você tem. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessário, alterne para um plano diferente do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Se o Office já estiver instalado no servidor RDS usando outros planos do Office 365, desinstale-o. Por exemplo, indo para o painel \> de controle desinstalar um programa. Desinstale usando o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando em problemas.

4. No servidor RDS, inicie sessão no centro de administração do Microsoft 365 com a conta de administrador e [Instale o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Após a instalação do Office, ***não abra nem entre em*** nenhum aplicativo do Office.

6. No servidor RDS, habilite a ativação do computador compartilhado editando o registro seguindo estas etapas:

1. Clique com botão direito no botão do Windows no canto inferior esquerdo da tela e selecione executar. Na caixa abrir, digite **regedit**e, em seguida, selecione OK.

2. Selecione Sim quando solicitado para permitir que o editor do Registro faça alterações no seu dispositivo.

3. No editor do registro, adicione um valor de cadeia de caracteres de **Sharedcomputerlicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. No servidor RDS, ***faça login como um usuário final*** e [Verifique se a ativação do computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Para obter mais detalhes sobre pré-requisitos, instruções de instalação e orientação sobre instalações personalizadas usando a ferramenta de implantação do Office, consulte [implantar o office 365 ProPlus usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Para corrigir erros relacionados à ativação do computador compartilhado, consulte [solucionar problemas com a ativação do computador compartilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  