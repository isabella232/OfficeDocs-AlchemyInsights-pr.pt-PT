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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37205420"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="2ef8b-102">Instalação de escritório em um servidor terminal</span><span class="sxs-lookup"><span data-stu-id="2ef8b-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="2ef8b-103">Para implantar o Office 365 ProPlus em um servidor Windows usando serviços de desktop remoto (RDS), anteriormente chamado de Serviços terminais:</span><span class="sxs-lookup"><span data-stu-id="2ef8b-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="2ef8b-104">Você deve ter um plano do Office 365 que inclua o Office 365 ProPlus, como o Office 365 Enterprise E3 ou o Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="2ef8b-105">Os planos Office 365 Business and Office 365 Business Premium não incluem o Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="2ef8b-106">Você precisa ativar a [ativação do computador compartilhado.](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="2ef8b-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="2ef8b-107">Se você quiser instalar o Office 365 ProPlus no RDS do centro de administração Microsoft 365, que usa configurações de instalação padrão, use as ***seguintes etapas.***</span><span class="sxs-lookup"><span data-stu-id="2ef8b-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="2ef8b-108">Você também pode baixar e executar o Assistente de [Suporte e Recuperação](https://aka.ms/SaRA_OfficeSCA_M365Portal) da Microsoft para instalar o Office 365 ProPlus no modo de ativação de computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="2ef8b-109">Verifique o plano do Office 365 que você tem.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="2ef8b-110">Saiba como</span><span class="sxs-lookup"><span data-stu-id="2ef8b-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="2ef8b-111">Se necessário, mude para um plano diferente do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="2ef8b-112">Saiba como</span><span class="sxs-lookup"><span data-stu-id="2ef8b-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="2ef8b-113">Se o Office já estiver instalado no servidor RDS usando quaisquer outros planos do Office 365, desinstalá-lo.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="2ef8b-114">Por exemplo, indo \> para o Painel de Controle Desinstalar um programa.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="2ef8b-115">Desinstale o uso do [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver se deparando com problemas.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="2ef8b-116">No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e instale o [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="2ef8b-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="2ef8b-117">Depois que o Office for instalado, ***não abra ou entre em*** nenhuma inscrição no Office.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="2ef8b-118">No servidor RDS, habilite a ativação compartilhada do computador editando o registro seguindo essas etapas:</span><span class="sxs-lookup"><span data-stu-id="2ef8b-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="2ef8b-119">Clique à direita no botão Do Windows no canto inferior esquerdo da tela e selecione Run.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="2ef8b-120">Na caixa aberta, tipo **regedit,** e selecione então APROVADO.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="2ef8b-121">Selecione sim quando solicitado a permitir que o Editor de Registro faça alterações em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="2ef8b-122">No editor de registro, adicione um valor de corda de **SharedComputerLicensing** com uma configuração de 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="2ef8b-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="2ef8b-123">No servidor RDS, ***entre como usuário final*** e verifique se a [ativação compartilhada do computador está ativada para o Office 365 ProPlus.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="2ef8b-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="2ef8b-124">Para obter mais detalhes sobre pré-requisitos, instruções de configuração e orientação sobre instalações personalizadas usando a ferramenta de implantação do office, [consulte o Deploy Office 365 ProPlus usando serviços de desktop remotos.](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="2ef8b-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="2ef8b-125">Para corrigir erros relacionados à ativação compartilhada do computador, consulte problemas de [solução de problemas com ativação de computador compartilhada para o Office 365 ProPlus.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="2ef8b-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  