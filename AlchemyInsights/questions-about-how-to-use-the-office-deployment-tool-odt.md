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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Perguntas sobre como utilizar a ferramenta de implementação do Office (ODT)

Transferir a ferramenta de implementação do Office a partir do [Centro de transferências da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Depois de transferir o ficheiro, execute o ficheiro executável extracção automática que contém a implementação de ferramenta do Office executável (setup.exe) e um ficheiro de configuração de exemplo (configuration.xml).
  
 **Para excluir ou remover produtos Office 365 ProPlus de computadores de cliente:**
  
Quando instalar o Office 365 ProPlus, pode excluir a produtos específicos. Para tal, siga os passos para instalar o Office com a ODT, mas incluir o elemento ExcludeApp no ficheiro de configuração. Por exemplo, este ficheiro de configuração instala todos os produtos do Office 365 ProPlus excepto Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Descrição geral da ferramenta de implementação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

