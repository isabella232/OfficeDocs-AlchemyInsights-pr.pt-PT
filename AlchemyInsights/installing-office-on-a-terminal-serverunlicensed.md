---
title: Instalar o office num servidor de terminais - sem licença
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410133"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalar o Office num servidor de terminais

Para implementar o Office 365 ProPlus num servidor do Windows utilizando os serviços de ambiente de trabalho remoto (RDS), anteriormente denominado Serviços de Terminal:
  
- Tem de ter um plano do Office 365 que inclui Office 365 ProPlus, tal como E3 de empresa do Office 365 ou E5 de empresa. Os planos de negócio do Office 365 e no Office 365 Business Premium não incluem ProPlus do Office 365.
    
- É necessário activar a [activação do computador partilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Se pretender instalar o Office 365 ProPlus no RDS a partir do portal Office 365, * * *que utiliza predefinições de instalação* * *, siga estes passos: 
  
1. Verifique qual o plano do Office 365 tiver. [Obter informações sobre como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Se necessário, mude para uma diferente do Office 365 planear. [Obter informações sobre como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Se o Office já está instalado no servidor de RDS utilizando outros planos de Office 365, desinstale-o. Por exemplo, através do painel de controlo \> desinstalar um programa. Desinstale a utilizar o [Assistente de recuperação e de suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se estiver a executar em problemas. 
    
4. No servidor de RDS, iniciar sessão no portal Office 365 com a conta de administrador e, em seguida, [instalar o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Depois de instalado o Office, * * *não abrir ou iniciar sessão no* * * para as aplicações do Office. 
    
6. No servidor de RDS, permitir a activação do computador partilhado editando o registo seguindo estes passos:
    
1. Faça duplo clique no botão de Windows no canto inferior esquerdo do ecrã e seleccione Executar. Na caixa Abrir, escreva **regedit**e, em seguida, seleccione ' OK '. 
    
2. Seleccione Sim quando lhe for pedido para permitir que o Editor de registo para efectuar alterações ao dispositivo.
    
3. No Editor de registo, adicione um valor de cadeia de **SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. No servidor de RDS, * * *Iniciar sessão como um utilizador final* * * e [Certifique-se de que a activação do computador partilhado está activada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Para mais informações sobre pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas utilizando a ferramenta de implementação do Office, consulte [Implementar o Office 365 ProPlus utilizando os serviços de ambiente de trabalho remoto](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Para corrigir os erros relacionados com a activação do computador partilhado, consulte [problemas de resolução de problemas com a activação do computador partilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

