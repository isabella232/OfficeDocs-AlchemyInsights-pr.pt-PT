---
title: Instalação de escritório num Servidor de Terminal - Não Licenciado
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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763228"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalação de escritório em um servidor de terminal

Para implementar aplicações Microsoft 365 para empresa num Servidor Windows utilizando serviços de ambiente de trabalho remotos (RDS), anteriormente chamados Serviços de Terminal:
  
- Deve ter uma subscrição Microsoft 365 que inclua aplicações Microsoft 365 para empresa, como o Office 365 Enterprise E3 ou enterprise E5. As Aplicações Microsoft 365 para negócios e aplicações Microsoft 365 para planos premium de negócios não incluem aplicações Microsoft 365 para empresa.

- Tem de ativar a [ativação do computador partilhado.](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

Se pretender instalar aplicações Microsoft 365 para empresa em RDS a partir do centro de administração microsoft 365, que utiliza as definições de ***instalação predefinidas,*** utilize os seguintes passos.

> [!TIP]
> Também pode descarregar e executar o [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar as Aplicações Microsoft 365 para empresas em modo de ativação de computador partilhado.
  
1. Verifique qual a subscrição do Microsoft 365 que tem. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessário, mude para uma subscrição diferente do Microsoft 365. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Se o Office já estiver instalado no servidor RDS utilizando quaisquer outras subscrições do Microsoft 365, desinstale-o. Por exemplo, indo \> ao Painel de Controlo Desinstalar um programa. Desinstale utilizando o [Microsoft Support e Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se estiver a ter problemas.

4. No servidor RDS, inscreva-se no centro de administração da Microsoft 365 com a sua conta de administrador e [instale aplicações Microsoft 365 para empresa](https://portal.office.com/OLS/MySoftware.aspx).

5. Depois de instalado o Office, ***não abra nem inscreva*** em quaisquer candidaturas do Office.

6. No servidor RDS, ative a ativação do computador partilhado editando o registo seguindo estes passos:

1. Clique no botão Windows no canto inferior esquerdo do ecrã e selecione Executar. Na caixa Aberta, escreva **regedite**e, em seguida, selecione OK.

2. Selecione Sim quando solicitado para permitir que o Editor de Registo faça alterações no seu dispositivo.

3. No Editor de Registo, adicione um valor de cadeia de **SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuração.

7. No servidor RDS, ***inscreva-se como utilizador final*** e verifique se a [ativação partilhada de computador está ativada para aplicações microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Para mais detalhes sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas utilizando a Ferramenta de Implementação do Office, consulte [implementar aplicações Microsoft 365 para empresa utilizando serviços](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)de ambiente de trabalho remotos .
  
Para corrigir erros relacionados com a ativação partilhada de computador, consulte [problemas de Resolução de Problemas com ativação de computador partilhado para aplicações microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  