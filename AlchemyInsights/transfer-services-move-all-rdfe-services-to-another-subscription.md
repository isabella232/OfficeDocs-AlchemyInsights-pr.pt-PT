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
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services - Mover todos os serviços RDFE para outra subscrição

**Mover recursos**

Os recursos Azure podem ser transferidos para outro grupo de subscrição ou recursos Azure sob a mesma subscrição usando o portal Azure PowerShell, Azure CLI ou a API REST para mover recursos.

Antes de poder mover recursos, consulte:

- [Lista de verificação antes de mover recursos](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Serviços que podem ser movidos](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Como validar o movimento](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Orientar para os serviços](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Para mover os recursos existentes para outro grupo de recursos ou subscrição, pode utilizar:

- [Portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REPOUSO API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [Mover recursos Azure para outro grupo de recursos ou subscrição](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Erros de resolução de problemas com o Gestor de Recursos Azure**

Consulte os artigos abaixo para saber sobre alguns erros comuns de implementação do Azure e receba informações para resolvê-los. Se não conseguir encontrar o código de erro do seu erro de implementação, consulte [o código de erro find](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Erros de implementação de resolução de problemas](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Resolução de problemas que movem os recursos da Azure para um novo grupo de recursos ou subscrição](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Note que se quiser atualizar a sua subscrição Azure, como mudar de livre para pagar, terá de converter a sua subscrição.

- Para atualizar um teste gratuito, consulte [a atualização do seu Teste Gratuito ou subscrição do Microsoft Imagine Azure para Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Para alterar uma conta pay-as-you-go, consulte [alterar a sua subscrição Azure Pay-As-You-Go para uma oferta diferente](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Para adicionar ou associar uma assinatura Azure ao seu inquilino Azure Ative Directory:**

1. Faça o súbs e selecione a subscrição que pretende utilizar a partir da [página Subscrições no portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Selecione **Diretório de Alteração**.
3. Reveja quaisquer avisos que apareçam e, em seguida, selecione **Alterar**.
4. O diretório é alterado para a subscrição e receberá uma mensagem de sucesso.
5. Use o *comutador de diretório* para ir ao seu novo diretório. Pode levar até 10 minutos para que tudo apareça corretamente.

**Documentos Recomendados**

- [Transferência de propriedade de uma assinatura Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mover recursos para novo grupo de recursos ou subscrição](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gerir recursos usando o portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
