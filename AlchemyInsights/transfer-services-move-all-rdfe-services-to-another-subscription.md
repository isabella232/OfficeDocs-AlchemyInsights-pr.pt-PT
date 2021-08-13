---
title: Transferir Serviços - Mover todos os serviços RDFE para outra subscrição
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940078"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transferir Serviços - Mover todos os serviços RDFE para outra subscrição

**Mover recursos**

Os recursos do Azure podem ser movidos para outro grupo de recursos ou subscrição do Azure na mesma subscrição através do portal do Azure, do Azure PowerShell, do Azure CLI ou da API REST para mover recursos.

Antes de poder mover recursos, consulte:

- [Lista de verificação antes de mover recursos](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Serviços que podem ser movidos](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Como validar a movimentação](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Orientação para movimentações de serviços](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Para mover recursos existentes para outro grupo de recursos ou subscrição, pode utilizar:

- [Portal do Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: Mover [recursos do Azure para outro grupo ou subscrição de recursos](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Remova erros com o Gestor de Recursos do Azure**

Consulte os artigos abaixo para saber mais sobre alguns erros comuns de implementação do Azure e receber informações para resolvê-los. Se não conseguir encontrar o código de erro para o erro de implementação, consulte [Encontrar código de erro.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Remoção de erros de implementação](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Remova a movimentação de recursos do Azure para um novo grupo ou subscrição de recursos](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Tenha em atenção que, se quiser atualizar a sua subscrição do Azure, tal como mudar da subscrição gratuita para pay-as-go, terá de converter a sua subscrição.

- Para atualizar uma avaliação gratuita, consulte Atualizar a sua Avaliação Gratuita ou a sua subscrição do [Microsoft Imagine Azure para o Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Para alterar uma conta pré-paga, consulte Alterar a sua subscrição do [Azure Pay-As-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)para uma oferta diferente.

**Para adicionar ou associar uma subscrição do Azure ao seu inquilino do Azure Active Directory:**

1. Inscreva-se e selecione a subscrição que pretende utilizar a partir da [página Subscrições no portal do Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. **Selecione Alterar diretório**.
3. Reveja todos os avisos apresentados e, em seguida, **selecione Alterar**.
4. O diretório é alterado para a subscrição e receberá uma mensagem de sucesso.
5. Utilize o *Comutador* de diretório para ir para o seu novo diretório. Pode demorar até 10 minutos para que tudo seja apresentado corretamente.

**Documentos recomendados**

- [Transferir a propriedade de uma subscrição do Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mover recursos para um novo grupo de recursos ou subscrição](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gerir recursos com o portal do Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
