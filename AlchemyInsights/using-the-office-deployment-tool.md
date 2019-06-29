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
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365536"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizando a ferramenta de implementação do Office (ODT)

Utilize a ferramenta de implementação do Office (ODT) para implementar o Office 365 versões do Office. A ferramenta de implementação do Office (setup.exe) é executada a partir da linha de comandos e utiliza um ficheiro XML de configuração para determinar quais as definições a aplicar quando implementar o Office.
  
1. Transferir a versão mais recente da ferramenta de implementação do Office a partir do [Centro de transferências da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Utilize a [Ferramenta de personalização do Office (PTU)](https://config.office.com) para seleccionar as preferências de implementação e criar o ficheiro XML de configuração. Exportar o ficheiro de configuração e colocá-lo localmente na mesma pasta em que reside o setup.exe.

    **Nota:** Instalação do Office problemas normalmente ocorrem devido a incorrectamente configurado ou ficheiros de configuração malformatted. Para evitar estes problemas, recomendamos que utilize a ferramenta de personalização do Office para criar o ficheiro de configuração. Também pode importar ficheiros de configuração existentes para a ferramenta de personalização do Office.

3. A partir de uma linha de comandos elevada, mude para a localização onde reside a setup.exe e executar a ferramenta de implementação do Office no modo de transferência e especifique o ficheiro de configuração que acabou de guardar. Neste exemplo, o ficheiro de configuração é denominado Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Executar a ferramenta de implementação do Office no modo de configurar e especifique o ficheiro de configuração.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Nota:** Tem de executar este passo do computador cliente no qual pretende instalar o Office e tem de ter permissões de administrador local nesse computador.

Para mais informações sobre como utilizar a ferramenta de implementação do Office para os Office 365 ProPlus cenários de implementação, consulte [Descrição geral da ferramenta de implementação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Para obter mais detalhes sobre como utilizar a ferramenta de personalização do Office, consulte [Descrição geral da ferramenta de personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
