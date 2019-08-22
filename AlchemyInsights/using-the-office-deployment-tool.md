---
title: Utilizando a ferramenta de implementação do Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 874bb7883bca4f062e85963a6828a771cd2dad9b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531586"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="62358-102">Utilizando a ferramenta de implementação do Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="62358-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="62358-103">Utilize a ferramenta de implementação do Office (ODT) para implementar o Office 365 versões do Office.</span><span class="sxs-lookup"><span data-stu-id="62358-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="62358-104">A ferramenta de implementação do Office (setup.exe) é executada a partir da linha de comandos e utiliza um ficheiro XML de configuração para determinar quais as definições a aplicar quando implementar o Office.</span><span class="sxs-lookup"><span data-stu-id="62358-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="62358-105">Transferir a versão mais recente da ferramenta de implementação do Office a partir do [Centro de transferências da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="62358-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="62358-106">Utilize a [Ferramenta de personalização do Office (PTU)](https://config.office.com) para seleccionar as preferências de implementação e criar o ficheiro XML de configuração.</span><span class="sxs-lookup"><span data-stu-id="62358-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="62358-107">Exportar o ficheiro de configuração e colocá-lo localmente na mesma pasta em que reside o setup.exe.</span><span class="sxs-lookup"><span data-stu-id="62358-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="62358-108">**Nota:** Instalação do Office problemas normalmente ocorrem devido a incorrectamente configurado ou ficheiros de configuração malformatted.</span><span class="sxs-lookup"><span data-stu-id="62358-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="62358-109">Para evitar estes problemas, recomendamos que utilize a ferramenta de personalização do Office para criar o ficheiro de configuração.</span><span class="sxs-lookup"><span data-stu-id="62358-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="62358-110">Também pode importar ficheiros de configuração existentes para a ferramenta de personalização do Office.</span><span class="sxs-lookup"><span data-stu-id="62358-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="62358-111">A partir de uma linha de comandos elevada, mude para a localização onde reside a setup.exe e executar a ferramenta de implementação do Office no modo de transferência e especifique o ficheiro de configuração que acabou de guardar.</span><span class="sxs-lookup"><span data-stu-id="62358-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="62358-112">Neste exemplo, o ficheiro de configuração é denominado Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="62358-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="62358-113">Executar a ferramenta de implementação do Office no modo de configurar e especifique o ficheiro de configuração.</span><span class="sxs-lookup"><span data-stu-id="62358-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="62358-114">**Nota:** Tem de executar este passo do computador cliente no qual pretende instalar o Office e tem de ter permissões de administrador local nesse computador.</span><span class="sxs-lookup"><span data-stu-id="62358-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="62358-115">Para mais informações sobre como utilizar a ferramenta de implementação do Office para os Office 365 ProPlus cenários de implementação, consulte [Descrição geral da ferramenta de implementação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="62358-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="62358-116">Para obter mais detalhes sobre como utilizar a ferramenta de personalização do Office, consulte [Descrição geral da ferramenta de personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="62358-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
