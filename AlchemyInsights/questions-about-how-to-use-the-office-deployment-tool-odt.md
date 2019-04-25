---
title: Perguntas sobre como utilizar a ferramenta de implementação do Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371779"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="a24a1-102">Perguntas sobre como utilizar a ferramenta de implementação do Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="a24a1-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a24a1-103">Transferir a ferramenta de implementação do Office a partir do [Centro de transferências da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a24a1-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="a24a1-104">Depois de transferir o ficheiro, execute o ficheiro executável extracção automática que contém a implementação de ferramenta do Office executável (setup.exe) e um ficheiro de configuração de exemplo (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="a24a1-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="a24a1-105">**Para excluir ou remover produtos Office 365 ProPlus de computadores de cliente:**</span><span class="sxs-lookup"><span data-stu-id="a24a1-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="a24a1-106">Quando instalar o Office 365 ProPlus, pode excluir a produtos específicos.</span><span class="sxs-lookup"><span data-stu-id="a24a1-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="a24a1-107">Para tal, siga os passos para instalar o Office com a ODT, mas incluir o elemento ExcludeApp no ficheiro de configuração.</span><span class="sxs-lookup"><span data-stu-id="a24a1-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="a24a1-108">Por exemplo, este ficheiro de configuração instala todos os produtos do Office 365 ProPlus excepto Publisher:</span><span class="sxs-lookup"><span data-stu-id="a24a1-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="a24a1-109">Descrição geral da ferramenta de implementação do Office</span><span class="sxs-lookup"><span data-stu-id="a24a1-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

