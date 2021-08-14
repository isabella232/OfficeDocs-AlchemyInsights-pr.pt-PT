---
title: Perguntas sobre como utilizar a Office de Implementação (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959694"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Perguntas sobre como utilizar a Office de Implementação (ODT)

Transfira a Office de Implementação a partir do Centro [de Transferências da Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Após transferir o ficheiro, execute o ficheiro executável de extração automática, que contém a Ferramenta de Implementação do Office executável (setup.exe) e um ficheiro de configuração de exemplo (configuration.xml).
  
 **Para excluir ou remover produtos Microsoft 365 Apps para Grandes Empresas dos computadores cliente:**
  
Ao instalar Microsoft 365 Apps para Grandes Empresas, pode excluir produtos específicos. Para o fazer, siga os passos para instalar o Office com o ODT, mas inclua o elemento ExcludeApp no seu ficheiro de configuração. Por exemplo, este ficheiro de configuração instala todos os produtos Microsoft 365 Apps para Grandes Empresas exceto Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

