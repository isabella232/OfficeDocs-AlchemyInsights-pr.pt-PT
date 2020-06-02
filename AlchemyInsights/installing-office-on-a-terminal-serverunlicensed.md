---
title: Instalação de escritório num Servidor de Terminais - Não licenciado
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508639"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalação do Office num Servidor de Terminais

Para implementar aplicações microsoft 365 para empresa num Servidor windows usando Serviços de Ambiente de Trabalho Remoto (RDS), anteriormente denominado Terminal Services:
  
- Deve ter uma subscrição do Microsoft 365 que inclui aplicações microsoft 365 para empresas, como o Office 365 Enterprise E3 ou Enterprise E5. As aplicações microsoft 365 para empresas e as aplicações microsoft 365 para planos Premium de negócios não incluem aplicações microsoft 365 para empresa.

- É necessário [ativar a ativação partilhada do computador.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Se pretender instalar aplicações microsoft 365 para empresas em RDS a partir do centro de administração microsoft 365, ***que utiliza definições de instalação predefinidos,*** utilize os seguintes passos.

> [!TIP]
> Também pode descarregar e executar o [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar aplicações microsoft 365 para empresas no modo de ativação de computador partilhado.
  
1. Verifique a subscrição do Microsoft 365 que tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessário, mude para uma subscrição diferente do Microsoft 365. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Se o Office já estiver instalado no servidor RDS utilizando quaisquer outras subscrições do Microsoft 365, desinstale-o. Por exemplo, indo ao Painel de Controlo \> Desinstalar um programa. Desinstala-se utilizando [o Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se estiver a ter problemas.

4. No servidor RDS, inscreva-se no centro de administração microsoft 365 com a sua conta de administrador e [instale aplicações microsoft 365 para empresa](https://portal.office.com/OLS/MySoftware.aspx).

5. Depois de instalado o Office, ***não abra nem inscreva nenhuma*** aplicação do Office.

6. No servidor RDS, ative a ativação partilhada do computador editando o registo seguindo estes passos:

1. Clique no botão Windows no canto inferior esquerdo do seu ecrã e selecione Executar. Na caixa Open, **escreva regedit**e, em seguida, selecione OK.

2. Selecione Sim quando solicitado para permitir que o Editor de Registo escora alterações no seu dispositivo.

3. No Editor de Registo, adicione um valor de cadeia de **SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. No servidor RDS, ***inscreva-se como utilizador final*** e verifique se a [ativação partilhada do computador está ativada para as Aplicações da Microsoft 365 para a empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Para obter mais detalhes sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas utilizando a Ferramenta de Implementação do Office, consulte [implementar aplicações do Microsoft 365 para empresa utilizando serviços de ambiente de trabalho remotos](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Para corrigir erros relacionados com a ativação partilhada do computador, consulte [problemas de resolução de problemas com ativação partilhada de computador para apps da Microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  