---
title: Implementação de Aplicações Microsoft 365 para utilização partilhada em RDS, Terminal Server ou VDI
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
ms.openlocfilehash: 51512b29f8d37ce6c39ece5bb704cb01e88e463d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010265"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementação de Aplicações Microsoft 365 para utilização partilhada em RDS, Terminal Server ou VDI

Para implementar aplicações microsoft 365 para empresa utilizando serviços de ambiente de trabalho remotos (RDS), anteriormente chamados Serviços de Terminal:
- Deve ter um microsoft 365 para plano de negócios ou um plano Office 365 que inclua aplicações Microsoft 365 para empresa, como office 365 Enterprise E3 ou Enterprise E5.
   > [!NOTE] 
   > As Aplicações Microsoft 365 para negócios e os planos Microsoft 365 Business Premium Standard não incluem aplicações Microsoft 365 para empresa.
- Tem de ativar a [ativação do computador partilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Também pode descarregar e executar o [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar as Aplicações Microsoft 365 para empresas em modo de ativação de computador partilhado.

Para obter mais informações sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas utilizando a Ferramenta de Implementação do Office, consulte [implementar aplicações Microsoft 365 para empresa utilizando serviços](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)de ambiente de trabalho remotos .

Para corrigir erros relacionados com a ativação do computador partilhado:
- Consulte [problemas de Troubleshoot com ativação de computador partilhado para aplicações microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Consulte [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218) (Repor as Aplicações do Microsoft 365 para empresas).

Se pretender instalar aplicações Microsoft 365 para empresa em RDS a partir do centro de administração microsoft 365, que utiliza as definições de ***instalação predefinidas,*** utilize os seguintes passos:

1.    Verifique qual a subscrição que tem. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Se necessário, mude para uma subscrição diferente. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Se o Office já estiver instalado no servidor RDS utilizando quaisquer outras subscrições da Microsoft, desinstale-o. Por exemplo, indo ao **Painel** > de Controlo**Desinstalar um programa**. Desinstale utilizando o [Microsoft Support e Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se estiver a ter problemas.
4.    No servidor RDS, inscreva-se no centro de administração da Microsoft 365 com a sua conta de administrador e [instale aplicações Microsoft 365 para empresa](https://portal.office.com/OLS/MySoftware.aspx).
5.    Depois de instalado o Office, ***não abra nem inscreva*** em quaisquer candidaturas do Office.
6.    No servidor RDS, ative a ativação do computador partilhado editando o registo seguindo estes passos:
   1. Clique no botão Windows no canto inferior esquerdo do ecrã e selecione **Executar**. Na caixa Aberta, escreva **regedite,** e, em seguida, selecione **OK**.
   2. Selecione **Sim** quando solicitado para permitir que o Editor de Registo faça alterações no seu dispositivo.
   3. No Editor de Registo, adicione um valor de cadeia de **SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuração.
   4. No servidor RDS, ***inscreva-se como utilizador final*** e verifique se a [ativação partilhada de computador está ativada para aplicações microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

