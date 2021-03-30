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
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="e07c8-102">Configurar o Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="e07c8-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="e07c8-103">O Microsoft Endpoint DLP permite-lhe prolongar a capacidade de monitorização e proteção do DLP às informações confidenciais em dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e07c8-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="e07c8-104">Após os dispositivos serem incluídos na gestão de dispositivos, pode criar políticas de DLP para aplicar ações de proteção nos itens.</span><span class="sxs-lookup"><span data-stu-id="e07c8-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="e07c8-105">O Explorador de Atividade pode ser utilizado para monitorizar a atividade de itens confidenciais.</span><span class="sxs-lookup"><span data-stu-id="e07c8-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="e07c8-106">Para mais informações, consulte [Integrar dispositivos na gestão de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="e07c8-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="e07c8-107">Para começar a utilizar o Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="e07c8-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="e07c8-108">Certifique-se de que tem o licenciamento de SKU/subscrição adequado.</span><span class="sxs-lookup"><span data-stu-id="e07c8-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="e07c8-109">Para obter mais informações, consulte [Licenciamento de SKU/subscrições](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="e07c8-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="e07c8-110">Verifique as permissões necessárias para ativar a gestão de dispositivos, aceder à página de inclusão ou ativar/desativar a monitorização de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e07c8-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="e07c8-111">Para mais informações, consulte [Permissões](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="e07c8-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="e07c8-112">Efetue a inclusão da dispositivos na gestão de Dispositivos ao seguir o procedimento para inclusão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e07c8-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="e07c8-113">Se não estiver a utilizar a opção de Ativação de Dispositivos (pré-visualização) nas **Definições** de Conformidade do M365, certifique-se de que tem a licença adequada e as permissões acima referidas.</span><span class="sxs-lookup"><span data-stu-id="e07c8-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="e07c8-114">Para obter mais informações, consulte [Integrar dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="e07c8-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="e07c8-115">Crie políticas de DLP para proteger os seus itens confidenciais.</span><span class="sxs-lookup"><span data-stu-id="e07c8-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="e07c8-116">Para obter informações, consulte [Cenários de política DLP do ponto final](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e07c8-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="e07c8-117">Para mais informações sobre o Microsoft Endpoint DLP, consulte [Informações sobre a prevenção de perda de dados em pontos finais do Microsoft 365 ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="e07c8-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="e07c8-118">**Passos importantes para a Recolha de dados, se for necessário Suporte:**</span><span class="sxs-lookup"><span data-stu-id="e07c8-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="e07c8-119">Transfira o "MDATP Client Analyzer Preview" a partir de [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="e07c8-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="e07c8-120">Execute a ferramenta como Administrador a partir da janela de cmd:</span><span class="sxs-lookup"><span data-stu-id="e07c8-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="e07c8-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="e07c8-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="e07c8-122">Quando lhe for pedido que "Introduza o número de minutos para recolher os rastreios:", introduza o número de minutos necessários para executar o cenário</span><span class="sxs-lookup"><span data-stu-id="e07c8-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="e07c8-123">Executar o cenário</span><span class="sxs-lookup"><span data-stu-id="e07c8-123">Run the scenario</span></span>

<span data-ttu-id="e07c8-124">Recolha a saída de ficheiro Zip para fornecer ao agente de Suporte.</span><span class="sxs-lookup"><span data-stu-id="e07c8-124">Collect the Zip file output to be given to the Support agent.</span></span>
