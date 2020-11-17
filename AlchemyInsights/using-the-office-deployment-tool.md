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
# <a name="using-the-office-deployment-tool-odt"></a>Utilização da Ferramenta de Implantação do Office (ODT)

Utiliza a Ferramenta de Implantação do Office (ODT) para implementar as versões do Office 365 do Office. A Ferramenta de Implantação do Office (setupodt.exe) é executada a partir da linha de comando e utiliza um ficheiro XML de configuração para determinar que definições aplicar ao implementar o Office.
  
1. Descarregue a versão mais recente da Ferramenta de Implementação do Office a partir do [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Utilize a [Ferramenta de Personalização do Office (OCT)](https://config.office.com) para selecionar as suas preferências de implementação e criar o ficheiro XML de configuração. Exporte o ficheiro de configuração e coloque-o localmente na mesma pasta onde reside o setupodt.exe.

    **Nota:** Os problemas de instalação do escritório ocorrem geralmente devido a ficheiros de configuração mal configurados ou malformados. Para evitar tais problemas, recomendamos que utilize a Ferramenta de Personalização do Office para criar o ficheiro de configuração. Também pode importar ficheiros de configuração existentes na Ferramenta de Personalização do Office.

3. A partir de uma operação de comando elevada, mude para o local onde reside setupodt.exe e execute a Ferramenta de Implementação do Office no modo de descarregamento e especifique o ficheiro de configuração que acabou de guardar. Neste exemplo, o ficheiro de configuração é nomeado Configuration.xml:

```setupodt.exe /download Configuration.xml```

4.Executar a Ferramenta de Implementação do Office no modo de configuração e especificar o ficheiro de configuração.

```setupodt.exe /configure Configuration.xml```

**Nota:** Tem de correr este passo a partir do computador cliente no qual pretende instalar o Office e tem de ter permissões de administrador local nesse computador.

Para saber mais sobre a utilização da Ferramenta de Implementação do Office para as suas Aplicações Microsoft 365 para cenários de implementação de empresas, consulte [a visão geral da Ferramenta de Implementação do Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Para obter mais detalhes sobre como utilizar a Ferramenta de Personalização do Office, consulte [a visão geral da Ferramenta de Personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
