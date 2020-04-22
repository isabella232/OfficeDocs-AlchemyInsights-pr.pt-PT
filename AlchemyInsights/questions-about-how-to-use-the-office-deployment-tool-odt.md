---
title: Perguntas sobre como usar a Ferramenta de Implantação de Escritórios (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698069"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Perguntas sobre como usar a Ferramenta de Implantação de Escritórios (ODT)

Descarregue a ferramenta de implementação do Office a partir do [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Depois de descarregar o ficheiro, execute o ficheiro executável auto-extraído, que contém a Ferramenta de Implementação do Office executável (configuração.exe) e um ficheiro de configuração de amostra (configuração.xml).
  
 **Para excluir ou remover as Aplicações Microsoft 365 para produtos empresariais de computadores clientes:**
  
Ao instalar aplicações microsoft 365 para empresa, pode excluir produtos específicos. Para tal, siga os passos para instalar o Office com o ODT, mas inclua o elemento ExcludeApp no seu ficheiro de configuração. Por exemplo, este ficheiro de configuração instala todas as Aplicações Microsoft 365 para produtos empresariais, exceto a Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Visão geral da ferramenta de implantação do escritório](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

