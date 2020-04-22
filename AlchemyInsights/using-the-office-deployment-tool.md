---
title: Utilização da ferramenta de implantação do escritório
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726259"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilização da ferramenta de implantação do escritório (ODT)

Utiliza a Ferramenta de Implantação do Office (ODT) para implementar versões do Office 365 do Office. A Ferramenta de Implantação do Office (setup.exe) é executada a partir da linha de comando e utiliza um ficheiro XML de configuração para determinar quais as definições a aplicar ao implementar o Office.
  
1. Descarregue a versão mais recente da Ferramenta de Implementação do Office a partir do [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Utilize a Ferramenta de Personalização do [Office (OCT)](https://config.office.com) para selecionar as suas preferências de implementação e criar o ficheiro XML de configuração. Exportar o ficheiro de configuração e colocá-lo localmente na mesma pasta onde reside a configuração.exe.

    **Nota:** Os problemas de instalação do escritório ocorrem geralmente devido a ficheiros de configuração mal configurados ou mal formados. Para evitar tais problemas, recomendamos que utilize a Ferramenta de Personalização do Office para criar o ficheiro de configuração. Também pode importar ficheiros de configuração existentes na Ferramenta de Personalização do Office.

3. A partir de um pedido de comando elevado, altere para o local onde a configuração.exe reside e execute a Ferramenta de Implementação do Office no modo de descarregamento e especifique o ficheiro de configuração que acabou de guardar. Neste exemplo, o ficheiro de configuração chama-se Configuração.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Executar a ferramenta de implantação do office no modo configurar e especificar o ficheiro de configuração.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Nota:** Tem de executar este passo a partir do computador cliente no qual pretende instalar o Office e tem de ter permissões de administrador local nesse computador.

Para saber mais sobre a utilização da Ferramenta de Implementação do Office para as suas Aplicações Microsoft 365 para cenários de implementação da empresa, consulte a [visão geral da ferramenta de implementação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Para mais detalhes sobre como utilizar a ferramenta de personalização do escritório, consulte a [visão geral da ferramenta de personalização do office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
