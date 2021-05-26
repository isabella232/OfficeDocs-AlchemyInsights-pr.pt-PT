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
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="b8073-102">Configurar o Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="b8073-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="b8073-103">O Microsoft Endpoint DLP permite-lhe prolongar a capacidade de monitorização e proteção do DLP às informações confidenciais em dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="b8073-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="b8073-104">Após os dispositivos serem incluídos na gestão de dispositivos, pode criar políticas de DLP para aplicar ações de proteção nos itens.</span><span class="sxs-lookup"><span data-stu-id="b8073-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="b8073-105">O Explorador de Atividade pode ser utilizado para monitorizar a atividade de itens confidenciais.</span><span class="sxs-lookup"><span data-stu-id="b8073-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="b8073-106">Para mais informações, consulte [Integrar dispositivos na gestão de dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="b8073-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="b8073-107">Para começar a utilizar o Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="b8073-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="b8073-108">Certifique-se de que tem o licenciamento de SKU/subscrição adequado.</span><span class="sxs-lookup"><span data-stu-id="b8073-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="b8073-109">Para obter mais informações, consulte [Licenciamento de SKU/subscrições](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="b8073-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="b8073-110">Verifique as permissões necessárias para ativar a gestão de dispositivos, aceder à página de inclusão ou ativar/desativar a monitorização de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b8073-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="b8073-111">Para mais informações, consulte [Permissões](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="b8073-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="b8073-112">Efetue a inclusão da dispositivos na gestão de Dispositivos ao seguir o procedimento para inclusão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b8073-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="b8073-113">Para obter mais informações, consulte [Integrar dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="b8073-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="b8073-114">Crie políticas de DLP para proteger os seus itens confidenciais.</span><span class="sxs-lookup"><span data-stu-id="b8073-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="b8073-115">Para obter informações, consulte [Cenários de política DLP do ponto final](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="b8073-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="b8073-116">Para mais informações sobre o Microsoft Endpoint DLP, consulte [Informações sobre a prevenção de perda de dados em pontos finais do Microsoft 365 ](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="b8073-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="b8073-117">**Passos importantes para a Recolha de dados, se for necessário Suporte:**</span><span class="sxs-lookup"><span data-stu-id="b8073-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="b8073-118">[Transfira MDATP Pré-visualização do Analisador de Clientes.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="b8073-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="b8073-119">Execute a ferramenta como Administrador a partir da janela de cmd:</span><span class="sxs-lookup"><span data-stu-id="b8073-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="b8073-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="b8073-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="b8073-121">Quando lhe for pedido, introduza o número de minutos para recolher **rastreios:**, introduza o número de minutos necessários para executar o cenário.</span><span class="sxs-lookup"><span data-stu-id="b8073-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="b8073-122">Execute o cenário.</span><span class="sxs-lookup"><span data-stu-id="b8073-122">Run the scenario.</span></span>

<span data-ttu-id="b8073-123">Recolha o resultado do ficheiro Zip para dar ao agente de Suporte.</span><span class="sxs-lookup"><span data-stu-id="b8073-123">Collect the Zip file output to give to the Support agent.</span></span>
