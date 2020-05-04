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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010625"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="04b7a-102">Instalação de escritório em um servidor de terminal</span><span class="sxs-lookup"><span data-stu-id="04b7a-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="04b7a-103">Para implementar aplicações Microsoft 365 para empresa num Servidor Windows utilizando serviços de ambiente de trabalho remotos (RDS), anteriormente chamados Serviços de Terminal:</span><span class="sxs-lookup"><span data-stu-id="04b7a-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="04b7a-104">Deve ter uma subscrição Microsoft 365 que inclua aplicações Microsoft 365 para empresa, como o Office 365 Enterprise E3 ou enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="04b7a-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="04b7a-105">As Aplicações Microsoft 365 para negócios e aplicações Microsoft 365 para planos premium de negócios não incluem aplicações Microsoft 365 para empresa.</span><span class="sxs-lookup"><span data-stu-id="04b7a-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="04b7a-106">Tem de ativar a [ativação do computador partilhado.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="04b7a-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="04b7a-107">Se pretender instalar aplicações Microsoft 365 para empresa em RDS a partir do centro de administração microsoft 365, que utiliza as definições de ***instalação predefinidas,*** utilize os seguintes passos.</span><span class="sxs-lookup"><span data-stu-id="04b7a-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="04b7a-108">Também pode descarregar e executar o [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar as Aplicações Microsoft 365 para empresas em modo de ativação de computador partilhado.</span><span class="sxs-lookup"><span data-stu-id="04b7a-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="04b7a-109">Verifique qual a subscrição do Microsoft 365 que tem.</span><span class="sxs-lookup"><span data-stu-id="04b7a-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="04b7a-110">Saiba como</span><span class="sxs-lookup"><span data-stu-id="04b7a-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="04b7a-111">Se necessário, mude para uma subscrição diferente do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="04b7a-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="04b7a-112">Saiba como</span><span class="sxs-lookup"><span data-stu-id="04b7a-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="04b7a-113">Se o Office já estiver instalado no servidor RDS utilizando quaisquer outras subscrições do Microsoft 365, desinstale-o.</span><span class="sxs-lookup"><span data-stu-id="04b7a-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="04b7a-114">Por exemplo, indo \> ao Painel de Controlo Desinstalar um programa.</span><span class="sxs-lookup"><span data-stu-id="04b7a-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="04b7a-115">Desinstale utilizando o [Microsoft Support e Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se estiver a ter problemas.</span><span class="sxs-lookup"><span data-stu-id="04b7a-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="04b7a-116">No servidor RDS, inscreva-se no centro de administração da Microsoft 365 com a sua conta de administrador e [instale aplicações Microsoft 365 para empresa](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="04b7a-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="04b7a-117">Depois de instalado o Office, ***não abra nem inscreva*** em quaisquer candidaturas do Office.</span><span class="sxs-lookup"><span data-stu-id="04b7a-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="04b7a-118">No servidor RDS, ative a ativação do computador partilhado editando o registo seguindo estes passos:</span><span class="sxs-lookup"><span data-stu-id="04b7a-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="04b7a-119">Clique no botão Windows no canto inferior esquerdo do ecrã e selecione Executar.</span><span class="sxs-lookup"><span data-stu-id="04b7a-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="04b7a-120">Na caixa Aberta, escreva **regedite**e, em seguida, selecione OK.</span><span class="sxs-lookup"><span data-stu-id="04b7a-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="04b7a-121">Selecione Sim quando solicitado para permitir que o Editor de Registo faça alterações no seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04b7a-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="04b7a-122">No Editor de Registo, adicione um valor de cadeia de **SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuração.</span><span class="sxs-lookup"><span data-stu-id="04b7a-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="04b7a-123">No servidor RDS, ***inscreva-se como utilizador final*** e verifique se a [ativação partilhada de computador está ativada para aplicações microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="04b7a-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="04b7a-124">Para mais detalhes sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas utilizando a Ferramenta de Implementação do Office, consulte [implementar aplicações Microsoft 365 para empresa utilizando serviços](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)de ambiente de trabalho remotos .</span><span class="sxs-lookup"><span data-stu-id="04b7a-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="04b7a-125">Para corrigir erros relacionados com a ativação partilhada de computador, consulte [problemas de Resolução de Problemas com ativação de computador partilhado para aplicações microsoft 365 para empresa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="04b7a-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  