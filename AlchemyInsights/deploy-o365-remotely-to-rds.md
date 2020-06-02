---
title: Implementação de Aplicativos Microsoft 365 para uso partilhado em RDS, Terminal Server ou VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507597"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementação de Aplicativos Microsoft 365 para uso partilhado em RDS, Terminal Server ou VDI

Para implementar aplicações microsoft 365 para empresas que utilizem serviços de desktop remoto (RDS), anteriormente nomeados Serviços de Terminal:
- Você deve ter um plano Microsoft 365 Para Negócios ou um plano office 365 que inclui Aplicações Microsoft 365 para empresas, tais como Office 365 Enterprise E3 ou Enterprise E5.
   > [!NOTE] 
   > As aplicações microsoft 365 para negócios e os planos Microsoft 365 Business Premium Standard não incluem aplicações microsoft 365 para empresas.
- Tem de [ativar a ativação partilhada do computador.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Também pode descarregar e executar o [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar aplicações microsoft 365 para empresas no modo de ativação de computador partilhado.

Para obter mais informações sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas utilizando a Ferramenta de Implementação do Office, consulte [implementar aplicações do Microsoft 365 para empresas utilizando serviços de ambiente de trabalho remotos](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Corrigir erros relacionados com a ativação partilhada do computador:
- Consulte [problemas de resolução de problemas com ativação de computador partilhada para aplicações da Microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Consulte [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218) (Repor as Aplicações do Microsoft 365 para empresas).

Se pretender instalar aplicações microsoft 365 para empresas em RDS a partir do centro de administração Microsoft 365, ***que utiliza definições de instalação predefinidos,*** utilize os seguintes passos:

1.    Verifique a subscrição que tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Se necessário, mude para uma subscrição diferente. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Se o Office já estiver instalado no servidor RDS utilizando quaisquer outras subscrições da Microsoft, desinstale-o. Por exemplo, indo ao **Painel de Controlo**  >  **Desinstale um programa**. Desinstala-se utilizando [o Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se estiver a ter problemas.
4.    No servidor RDS, inscreva-se no centro de administração microsoft 365 com a sua conta de administrador e [instale aplicações microsoft 365 para empresa](https://portal.office.com/OLS/MySoftware.aspx).
5.    Depois de instalado o Office, ***não abra nem inscreva nenhuma*** aplicação do Office.
6.    No servidor RDS, ative a ativação partilhada do computador editando o registo seguindo estes passos:
   1. Clique no botão Windows no canto inferior esquerdo do seu ecrã e selecione **Executar**. Na caixa Aberta, escreva **regedit**e, em seguida, selecione **OK**.
   2. Selecione **Sim** quando solicitado para permitir que o Editor de Registo escora alterações no seu dispositivo.
   3. No Editor de Registo, adicione um valor de cadeia de **SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. No servidor RDS, ***inscreva-se como utilizador final*** e verifique se a [ativação partilhada do computador está ativada para as Aplicações da Microsoft 365 para a empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

