---
title: Instalar o office num servidor de terminais - sem licença
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498426"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="66566-102">Instalar o Office num servidor de terminais</span><span class="sxs-lookup"><span data-stu-id="66566-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="66566-103">Para implementar o Office 365 ProPlus num servidor do Windows utilizando os serviços de ambiente de trabalho remoto (RDS), anteriormente denominado Serviços de Terminal:</span><span class="sxs-lookup"><span data-stu-id="66566-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="66566-104">Tem de ter um plano do Office 365 que inclui Office 365 ProPlus, tal como E3 de empresa do Office 365 ou E5 de empresa.</span><span class="sxs-lookup"><span data-stu-id="66566-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="66566-105">Os planos de negócio do Office 365 e no Office 365 Business Premium não incluem ProPlus do Office 365.</span><span class="sxs-lookup"><span data-stu-id="66566-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="66566-106">É necessário activar a [activação do computador partilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="66566-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="66566-107">Se pretender instalar o Office 365 ProPlus no RDS a partir do portal Office 365, ***que utiliza predefinições de instalação***, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="66566-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="66566-108">Verifique qual o plano do Office 365 tiver.</span><span class="sxs-lookup"><span data-stu-id="66566-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="66566-109">Obter informações sobre como</span><span class="sxs-lookup"><span data-stu-id="66566-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="66566-110">Se necessário, mude para uma diferente do Office 365 planear.</span><span class="sxs-lookup"><span data-stu-id="66566-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="66566-111">Obter informações sobre como</span><span class="sxs-lookup"><span data-stu-id="66566-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="66566-112">Se o Office já está instalado no servidor de RDS utilizando outros planos de Office 365, desinstale-o.</span><span class="sxs-lookup"><span data-stu-id="66566-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="66566-113">Por exemplo, através do painel de controlo \> desinstalar um programa.</span><span class="sxs-lookup"><span data-stu-id="66566-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="66566-114">Desinstale a utilizar o [Assistente de recuperação e de suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se estiver a executar em problemas.</span><span class="sxs-lookup"><span data-stu-id="66566-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="66566-115">No servidor de RDS, iniciar sessão no portal Office 365 com a conta de administrador e, em seguida, [instalar o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="66566-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="66566-116">Depois de instalado o Office, ***não abra ou iniciar sessão em*** quaisquer aplicações do Office.</span><span class="sxs-lookup"><span data-stu-id="66566-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="66566-117">No servidor de RDS, permitir a activação do computador partilhado editando o registo seguindo estes passos:</span><span class="sxs-lookup"><span data-stu-id="66566-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="66566-118">Faça duplo clique no botão de Windows no canto inferior esquerdo do ecrã e seleccione Executar.</span><span class="sxs-lookup"><span data-stu-id="66566-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="66566-119">Na caixa Abrir, escreva **regedit**e, em seguida, seleccione ' OK '.</span><span class="sxs-lookup"><span data-stu-id="66566-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="66566-120">Seleccione Sim quando lhe for pedido para permitir que o Editor de registo para efectuar alterações ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66566-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="66566-121">No Editor de registo, adicione um valor de cadeia de **SharedComputerLicensing** com uma definição de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="66566-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="66566-122">No servidor RDS, ***Iniciar sessão como um utilizador final*** e [Certifique-se de que a activação do computador partilhado está activada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="66566-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="66566-123">Para mais informações sobre pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas utilizando a ferramenta de implementação do Office, consulte [Implementar o Office 365 ProPlus utilizando os serviços de ambiente de trabalho remoto](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="66566-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="66566-124">Para corrigir os erros relacionados com a activação do computador partilhado, consulte [problemas de resolução de problemas com a activação do computador partilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="66566-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  