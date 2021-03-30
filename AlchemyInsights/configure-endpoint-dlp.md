---
title: Configurar o Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402445"
---
# <a name="configure-endpoint-dlp"></a>Configurar o Endpoint DLP

O Microsoft Endpoint DLP permite-lhe prolongar a capacidade de monitorização e proteção do DLP às informações confidenciais em dispositivos Windows 10. Após os dispositivos serem incluídos na gestão de dispositivos, pode criar políticas de DLP para aplicar ações de proteção nos itens. O Explorador de Atividade pode ser utilizado para monitorizar a atividade de itens confidenciais. Para mais informações, consulte [Integrar dispositivos na gestão de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Para começar a utilizar o Endpoint DLP:

- Certifique-se de que tem o licenciamento de SKU/subscrição adequado. Para obter mais informações, consulte [Licenciamento de SKU/subscrições](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verifique as permissões necessárias para ativar a gestão de dispositivos, aceder à página de inclusão ou ativar/desativar a monitorização de dispositivos. Para mais informações, consulte [Permissões](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Efetue a inclusão da dispositivos na gestão de Dispositivos ao seguir o procedimento para inclusão de dispositivos. Se não estiver a utilizar a opção de Ativação de Dispositivos (pré-visualização) nas **Definições** de Conformidade do M365, certifique-se de que tem a licença adequada e as permissões acima referidas. Para obter mais informações, consulte [Integrar dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Crie políticas de DLP para proteger os seus itens confidenciais. Para obter informações, consulte [Cenários de política DLP do ponto final](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Para mais informações sobre o Microsoft Endpoint DLP, consulte [Informações sobre a prevenção de perda de dados em pontos finais do Microsoft 365 ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Passos importantes para a Recolha de dados, se for necessário Suporte:**

1. Transfira o "MDATP Client Analyzer Preview" a partir de [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Execute a ferramenta como Administrador a partir da janela de cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Quando lhe for pedido que "Introduza o número de minutos para recolher os rastreios:", introduza o número de minutos necessários para executar o cenário
5. Executar o cenário

Recolha a saída de ficheiro Zip para fornecer ao agente de Suporte.
