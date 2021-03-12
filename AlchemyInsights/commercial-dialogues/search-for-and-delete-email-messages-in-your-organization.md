---
title: Procure e elimine mensagens de e-mail na sua organização
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750013"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="79723-102">Procure e elimine mensagens de e-mail na sua organização</span><span class="sxs-lookup"><span data-stu-id="79723-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="79723-103">Siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="79723-103">Follow these steps:</span></span>

1. <span data-ttu-id="79723-104">Se não for administrador global, procurar mensagens a sua conta deve ser adicionada ao **grupo de funções eDiscovery Manager** ou à **função de gestão de Compliance Search**.</span><span class="sxs-lookup"><span data-stu-id="79723-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="79723-105">Para eliminar mensagens, terá de se juntar ao grupo de **funções de Gestão** da Organização ou à **função de gestão de Pesquisa e Purga.**</span><span class="sxs-lookup"><span data-stu-id="79723-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="79723-106">As permissões a estas funções são atribuídas no [Centro de Conformidade & Segurança.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="79723-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="79723-107">[Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem para eliminar.</span><span class="sxs-lookup"><span data-stu-id="79723-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="79723-108">[Ligue-se ao Centro de Conformidade & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="79723-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="79723-109">Se estiver a utilizar o MFA, consulte estas instruções: [Ligue-se à Segurança & Compliance Center PowerShell utilizando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="79723-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="79723-110">Eliminar a mensagem: executar o `New-ComplianceSearchAction` cmdlet para apagar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="79723-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="79723-111">As mensagens eliminadas são transferidas para a pasta de Itens Recuperáveis de um utilizador.</span><span class="sxs-lookup"><span data-stu-id="79723-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="79723-112">Para um comando de exemplo, consulte [o passo 3: Eliminar a mensagem.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="79723-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
