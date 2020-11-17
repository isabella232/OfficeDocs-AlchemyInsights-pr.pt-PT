---
title: Utilização da ferramenta de implantação do office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085843"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="336ec-102">Utilização da Ferramenta de Implantação do Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="336ec-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="336ec-103">Utiliza a Ferramenta de Implantação do Office (ODT) para implementar as versões do Office 365 do Office.</span><span class="sxs-lookup"><span data-stu-id="336ec-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="336ec-104">A Ferramenta de Implantação do Office (setupodt.exe) é executada a partir da linha de comando e utiliza um ficheiro XML de configuração para determinar que definições aplicar ao implementar o Office.</span><span class="sxs-lookup"><span data-stu-id="336ec-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="336ec-105">Descarregue a versão mais recente da Ferramenta de Implementação do Office a partir do [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="336ec-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="336ec-106">Utilize a [Ferramenta de Personalização do Office (OCT)](https://config.office.com) para selecionar as suas preferências de implementação e criar o ficheiro XML de configuração.</span><span class="sxs-lookup"><span data-stu-id="336ec-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="336ec-107">Exporte o ficheiro de configuração e coloque-o localmente na mesma pasta onde reside o setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="336ec-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="336ec-108">**Nota:** Os problemas de instalação do escritório ocorrem geralmente devido a ficheiros de configuração mal configurados ou malformados.</span><span class="sxs-lookup"><span data-stu-id="336ec-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="336ec-109">Para evitar tais problemas, recomendamos que utilize a Ferramenta de Personalização do Office para criar o ficheiro de configuração.</span><span class="sxs-lookup"><span data-stu-id="336ec-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="336ec-110">Também pode importar ficheiros de configuração existentes na Ferramenta de Personalização do Office.</span><span class="sxs-lookup"><span data-stu-id="336ec-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="336ec-111">A partir de uma operação de comando elevada, mude para o local onde reside setupodt.exe e execute a Ferramenta de Implementação do Office no modo de descarregamento e especifique o ficheiro de configuração que acabou de guardar.</span><span class="sxs-lookup"><span data-stu-id="336ec-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="336ec-112">Neste exemplo, o ficheiro de configuração é nomeado Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="336ec-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="336ec-113">4.Executar a Ferramenta de Implementação do Office no modo de configuração e especificar o ficheiro de configuração.</span><span class="sxs-lookup"><span data-stu-id="336ec-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="336ec-114">**Nota:** Tem de correr este passo a partir do computador cliente no qual pretende instalar o Office e tem de ter permissões de administrador local nesse computador.</span><span class="sxs-lookup"><span data-stu-id="336ec-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="336ec-115">Para saber mais sobre a utilização da Ferramenta de Implementação do Office para as suas Aplicações Microsoft 365 para cenários de implementação de empresas, consulte [a visão geral da Ferramenta de Implementação do Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="336ec-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="336ec-116">Para obter mais detalhes sobre como utilizar a Ferramenta de Personalização do Office, consulte [a visão geral da Ferramenta de Personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="336ec-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
