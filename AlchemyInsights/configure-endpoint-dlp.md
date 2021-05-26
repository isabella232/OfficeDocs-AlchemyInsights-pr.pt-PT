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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657940"
---
# <a name="configure-endpoint-dlp"></a>Configurar o Endpoint DLP

O Microsoft Endpoint DLP permite-lhe prolongar a capacidade de monitorização e proteção do DLP às informações confidenciais em dispositivos Windows 10. Após os dispositivos serem incluídos na gestão de dispositivos, pode criar políticas de DLP para aplicar ações de proteção nos itens. O Explorador de Atividade pode ser utilizado para monitorizar a atividade de itens confidenciais. Para mais informações, consulte [Integrar dispositivos na gestão de dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Para começar a utilizar o Endpoint DLP:

- Certifique-se de que tem o licenciamento de SKU/subscrição adequado. Para obter mais informações, consulte [Licenciamento de SKU/subscrições](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verifique as permissões necessárias para ativar a gestão de dispositivos, aceder à página de inclusão ou ativar/desativar a monitorização de dispositivos. Para mais informações, consulte [Permissões](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Efetue a inclusão da dispositivos na gestão de Dispositivos ao seguir o procedimento para inclusão de dispositivos. Para obter mais informações, consulte [Integrar dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Crie políticas de DLP para proteger os seus itens confidenciais. Para obter informações, consulte [Cenários de política DLP do ponto final](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Para mais informações sobre o Microsoft Endpoint DLP, consulte [Informações sobre a prevenção de perda de dados em pontos finais do Microsoft 365 ](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Passos importantes para a Recolha de dados, se for necessário Suporte:**

1. [Transfira MDATP Pré-visualização do Analisador de Clientes.](https://aka.ms/betamdatpanalyzer)
1. Execute a ferramenta como Administrador a partir da janela de cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Quando lhe for pedido, introduza o número de minutos para recolher **rastreios:**, introduza o número de minutos necessários para executar o cenário.
1. Execute o cenário.

Recolha o resultado do ficheiro Zip para dar ao agente de Suporte.
