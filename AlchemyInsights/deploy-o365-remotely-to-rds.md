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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325614"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementar Microsoft 365 Apps para Grandes Empresas para utilização partilhada em RDS, Servidor de Terminal ou VDI

Para implementar o Microsoft 365 Apps para Grandes Empresas Serviços de Ambiente de Trabalho Remoto (RDS), anteriormente denominados Serviços de Terminal:

- Tem de ter um plano Microsoft 365 para Empresas ou um plano Office 365 que inclua Microsoft 365 Apps para Grandes Empresas, como o Office 365 Enterprise E3 ou Enterprise E5.
   **Nota:** as Microsoft 365 Apps para Pequenas e Médias Empresas e Microsoft 365 Empresas planos não incluem Microsoft 365 Apps para Grandes Empresas.
- Tem de [ativar a ativação do computador partilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

**Nota:** também pode transferir e executar o [Microsoft Assistente de Recuperação e Suporte](https://aka.ms/SaRA_OfficeSCA_M365Portal) instalar o Microsoft 365 Apps para Grandes Empresas no modo de ativação do computador partilhado.

Para obter mais informações sobre pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas através da Ferramenta de Implementação do Office, consulte Implementar o [Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)através dos Serviços de Ambiente de Trabalho Remoto.

Para corrigir erros relacionados com a ativação do computador partilhado:

- Consulte [Remoção de problemas com a ativação do computador partilhado Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Consulte [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218) (Repor as Aplicações do Microsoft 365 para empresas).

Se quiser instalar o Microsoft 365 Apps para Grandes Empresas RDS a partir do ***centro de administração do Microsoft 365,*** que utiliza as predefinições de instalação, utilize os seguintes passos:

1. Verifique que subscrição tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Se for necessário, mude para uma subscrição diferente. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Se Office já estiver instalado no servidor RDS com outras subscrições da Microsoft, desinstale-a. Por exemplo, ao ir para o **Painel de**  >  **Controlo, desinstale um programa.** Desinstale [com o Microsoft Assistente de Recuperação e Suporte](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft se estiver a ter problemas.
4. No servidor RDS, inscreva-se no servidor centro de administração do Microsoft 365 a sua conta de administrador e [instale a Microsoft 365 Apps para Grandes Empresas](https://portal.office.com/OLS/MySoftware.aspx).
5. Após Office instalada, não ***abra ou inscreva-se*** em nenhuma Office aplicações.
6. No servidor RDS, ative o computador partilhado ao editar o registo ao seguir estes passos:
   1. Clique com o botão direito Windows botão direito do rato no canto inferior esquerdo do seu ecrã e **selecione Executar**. Na caixa Abrir, escreva **regedit** e, em seguida, selecione **OK**.
   2. **Selecione** Sim quando lhe for pedido para permitir que o Editor de Registo faça alterações ao seu dispositivo.
   3. No Editor de Registo, adicione um valor de cadeia de valor **de SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. No servidor RDS, ***instale-se*** como utilizador final e verifique se a ativação do computador partilhado está ativada [para Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
