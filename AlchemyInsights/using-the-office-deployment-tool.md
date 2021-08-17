---
title: Utilizar a Office de Implementação
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083781"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizar a Office de Implementação (ODT)

Utilize a Ferramenta Office de Implementação (ODT) para implementar Office 365 versões do Office. A ferramenta Office Deployment Tool (setup.exe) é executada a partir da linha de comandos e utiliza um ficheiro XML de configuração para determinar quais as definições a aplicar ao implementar Office.
  
1. Transfira a versão mais recente da Ferramenta Office Implementação a partir do Centro [de Transferências da Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Utilize a [Office de Personalização Automática (OCT)](https://config.office.com) para selecionar as preferências de implementação e criar o ficheiro XML de configuração. Exporte o ficheiro de configuração e coloque-o localmente na mesma pasta onde o setup.exe local.

    **Nota: Office** de instalação frequentemente ocorrem devido a ficheiros de configuração mal configurados ou mal formatados. Para evitar esses problemas, recomendamos que utilize a Ferramenta de Office personalização para criar o ficheiro de configuração. Também pode importar ficheiros de configuração existentes para a Office de Personalização.

3. A partir de uma fila de comandos elevada, mude para a localização onde o setup.exe se encontra e execute a Ferramenta de Implementação do Office no modo de transferência e especifique o ficheiro de configuração que acabou de guardar. Neste exemplo, o ficheiro de configuração tem o nome Configuration.xml:

```setup.exe /download Configuration.xml```

4.Execute a Office de Implementação Automática no modo de configuração e especifique o ficheiro de configuração.

```setup.exe /configure Configuration.xml```

**Nota:** Tem de executar este passo a partir do computador cliente no qual pretende instalar o Office e tem de ter permissões de administrador local no computador.

Para saber mais sobre como Office a Ferramenta de Implementação para os cenários de implementação do Microsoft 365 Apps para Grandes Empresas, consulte o Office da Ferramenta de Implementação do [Office.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Para obter mais detalhes sobre como utilizar a Ferramenta Office Personalização, consulte o Office [de Personalização da Ferramenta de Personalização.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
