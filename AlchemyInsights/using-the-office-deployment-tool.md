---
title: Utilizando a ferramenta de implementação do Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483879"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="404e6-102">Utilizando a ferramenta de implementação do Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="404e6-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="404e6-p101">Utilize a ferramenta de implementação do Office (ODT) para implementar o Office 365 versões do Office. A ferramenta de implementação do Office (setup.exe) é executada a partir da linha de comandos e utiliza um ficheiro XML de configuração para determinar quais as definições a aplicar quando implementar o Office.</span><span class="sxs-lookup"><span data-stu-id="404e6-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="404e6-105">Transferir a versão mais recente da ferramenta de implementação do Office a partir do [Centro de transferências da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="404e6-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="404e6-p102">Utilize a [Ferramenta de personalização do Office (PTU)](https://config.office.com) para seleccionar as preferências de implementação e criar o ficheiro XML de configuração. Exportar o ficheiro de configuração e colocá-lo localmente na mesma pasta em que reside o setup.exe.</span><span class="sxs-lookup"><span data-stu-id="404e6-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="404e6-p103">**Nota:** Instalação do Office problemas normalmente ocorrem devido a incorrectamente configurado ou ficheiros de configuração malformatted. Para evitar estes problemas, recomendamos que utilize a ferramenta de personalização do Office para criar o ficheiro de configuração. Também pode importar ficheiros de configuração existentes para a ferramenta de personalização do Office.</span><span class="sxs-lookup"><span data-stu-id="404e6-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="404e6-p104">A partir de uma linha de comandos elevada, mude para a localização onde reside a setup.exe e executar a ferramenta de implementação do Office no modo de transferência e especifique o ficheiro de configuração que acabou de guardar. Neste exemplo, o ficheiro de configuração é denominado Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="404e6-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="404e6-113">Executar a ferramenta de implementação do Office no modo de configurar e especifique o ficheiro de configuração.</span><span class="sxs-lookup"><span data-stu-id="404e6-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="404e6-114">**Nota:** Tem de executar este passo do computador cliente no qual pretende instalar o Office e tem de ter permissões de administrador local nesse computador.</span><span class="sxs-lookup"><span data-stu-id="404e6-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="404e6-p105">Para mais informações sobre como utilizar a ferramenta de implementação do Office para os Office 365 ProPlus cenários de implementação, consulte [Descrição geral da ferramenta de implementação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Para obter mais detalhes sobre como utilizar a ferramenta de personalização do Office, consulte [Descrição geral da ferramenta de personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="404e6-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

