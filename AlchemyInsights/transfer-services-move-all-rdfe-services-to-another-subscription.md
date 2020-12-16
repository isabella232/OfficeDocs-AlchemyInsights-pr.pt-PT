---
title: Transfer Services - Mover todos os serviços RDFE para outra subscrição
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692173"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="6a494-102">Transfer Services - Mover todos os serviços RDFE para outra subscrição</span><span class="sxs-lookup"><span data-stu-id="6a494-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="6a494-103">**Mover recursos**</span><span class="sxs-lookup"><span data-stu-id="6a494-103">**Move resources**</span></span>

<span data-ttu-id="6a494-104">Os recursos Azure podem ser transferidos para outro grupo de subscrição ou recursos Azure sob a mesma subscrição usando o portal Azure PowerShell, Azure CLI ou a API REST para mover recursos.</span><span class="sxs-lookup"><span data-stu-id="6a494-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="6a494-105">Antes de poder mover recursos, consulte:</span><span class="sxs-lookup"><span data-stu-id="6a494-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="6a494-106">Lista de verificação antes de mover recursos</span><span class="sxs-lookup"><span data-stu-id="6a494-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="6a494-107">Serviços que podem ser movidos</span><span class="sxs-lookup"><span data-stu-id="6a494-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="6a494-108">Como validar o movimento</span><span class="sxs-lookup"><span data-stu-id="6a494-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="6a494-109">Orientar para os serviços</span><span class="sxs-lookup"><span data-stu-id="6a494-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="6a494-110">Para mover os recursos existentes para outro grupo de recursos ou subscrição, pode utilizar:</span><span class="sxs-lookup"><span data-stu-id="6a494-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="6a494-111">Portal Azure</span><span class="sxs-lookup"><span data-stu-id="6a494-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="6a494-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6a494-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="6a494-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6a494-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="6a494-114">REPOUSO API</span><span class="sxs-lookup"><span data-stu-id="6a494-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="6a494-115">Tutorial: [Mover recursos Azure para outro grupo de recursos ou subscrição](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="6a494-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="6a494-116">**Erros de resolução de problemas com o Gestor de Recursos Azure**</span><span class="sxs-lookup"><span data-stu-id="6a494-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="6a494-117">Consulte os artigos abaixo para saber sobre alguns erros comuns de implementação do Azure e receba informações para resolvê-los.</span><span class="sxs-lookup"><span data-stu-id="6a494-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="6a494-118">Se não conseguir encontrar o código de erro do seu erro de implementação, consulte [o código de erro find](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="6a494-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="6a494-119">Erros de implementação de resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="6a494-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="6a494-120">Resolução de problemas que movem os recursos da Azure para um novo grupo de recursos ou subscrição</span><span class="sxs-lookup"><span data-stu-id="6a494-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="6a494-121">Note que se quiser atualizar a sua subscrição Azure, como mudar de livre para pagar, terá de converter a sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="6a494-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="6a494-122">Para atualizar um teste gratuito, consulte [a atualização do seu Teste Gratuito ou subscrição do Microsoft Imagine Azure para Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="6a494-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="6a494-123">Para alterar uma conta pay-as-you-go, consulte [alterar a sua subscrição Azure Pay-As-You-Go para uma oferta diferente](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="6a494-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="6a494-124">**Para adicionar ou associar uma assinatura Azure ao seu inquilino Azure Ative Directory:**</span><span class="sxs-lookup"><span data-stu-id="6a494-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="6a494-125">Faça o súbs e selecione a subscrição que pretende utilizar a partir da [página Subscrições no portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="6a494-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="6a494-126">Selecione **Diretório de Alteração**.</span><span class="sxs-lookup"><span data-stu-id="6a494-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="6a494-127">Reveja quaisquer avisos que apareçam e, em seguida, selecione **Alterar**.</span><span class="sxs-lookup"><span data-stu-id="6a494-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="6a494-128">O diretório é alterado para a subscrição e receberá uma mensagem de sucesso.</span><span class="sxs-lookup"><span data-stu-id="6a494-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="6a494-129">Use o *comutador de diretório* para ir ao seu novo diretório.</span><span class="sxs-lookup"><span data-stu-id="6a494-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="6a494-130">Pode levar até 10 minutos para que tudo apareça corretamente.</span><span class="sxs-lookup"><span data-stu-id="6a494-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="6a494-131">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="6a494-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="6a494-132">Transferência de propriedade de uma assinatura Azure</span><span class="sxs-lookup"><span data-stu-id="6a494-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="6a494-133">Mover recursos para novo grupo de recursos ou subscrição</span><span class="sxs-lookup"><span data-stu-id="6a494-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="6a494-134">Gerir recursos usando o portal Azure</span><span class="sxs-lookup"><span data-stu-id="6a494-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
