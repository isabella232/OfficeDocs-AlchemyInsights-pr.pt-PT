---
title: Perguntas sobre como utilizar a Ferramenta de Implementação do Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774902"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="16bd0-102">Perguntas sobre como utilizar a Ferramenta de Implementação do Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="16bd0-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="16bd0-103">Descarregue a Ferramenta de Implementação do Office a partir do [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="16bd0-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="16bd0-104">Depois de descarregar o ficheiro, execute o ficheiro executável de auto-extracção, que contém a Ferramenta de Implementação do Office Deployment executável (setup.exe) e um ficheiro de configuração da amostra (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="16bd0-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="16bd0-105">**Para excluir ou remover aplicações microsoft 365 para produtos empresariais de computadores clientes:**</span><span class="sxs-lookup"><span data-stu-id="16bd0-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="16bd0-106">Ao instalar as Aplicações Microsoft 365 para empresas, pode excluir produtos específicos.</span><span class="sxs-lookup"><span data-stu-id="16bd0-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="16bd0-107">Para tal, siga os passos para instalar o Office com o ODT, mas inclua o elemento ExcludeApp no seu ficheiro de configuração.</span><span class="sxs-lookup"><span data-stu-id="16bd0-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="16bd0-108">Por exemplo, este ficheiro de configuração instala todas as Aplicações Microsoft 365 para produtos empresariais, exceto o Publisher:</span><span class="sxs-lookup"><span data-stu-id="16bd0-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="16bd0-109">Visão geral da ferramenta de implantação do office</span><span class="sxs-lookup"><span data-stu-id="16bd0-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

