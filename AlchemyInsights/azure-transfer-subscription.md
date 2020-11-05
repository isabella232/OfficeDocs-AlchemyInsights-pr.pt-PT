---
title: Transferir propriedade de faturação Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922166"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="4d5b1-102">Transferir propriedade de faturação Azure</span><span class="sxs-lookup"><span data-stu-id="4d5b1-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="4d5b1-103">Inscreva-se no [portal Azure](https://portal.azure.com/) como administrador da conta de faturação que tem a subscrição que pretende transferir.</span><span class="sxs-lookup"><span data-stu-id="4d5b1-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="4d5b1-104">Se não tem a certeza se é e administrador, ou se precisa de determinar quem é, consulte [o administrador de faturação da conta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)determine .</span><span class="sxs-lookup"><span data-stu-id="4d5b1-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="4d5b1-105">Pesquisa em **Gestão de Custos + Faturação.**</span><span class="sxs-lookup"><span data-stu-id="4d5b1-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="4d5b1-106">Selecione **Subscrições** do painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="4d5b1-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="4d5b1-107">Dependendo do acesso, poderá ter de selecionar um âmbito de faturação e, em seguida, **subscrições** ou **subscrições Azure**.</span><span class="sxs-lookup"><span data-stu-id="4d5b1-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="4d5b1-108">**Selecione a propriedade de faturação de transferência** para a subscrição que pretende transferir</span><span class="sxs-lookup"><span data-stu-id="4d5b1-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="4d5b1-109">Insira o endereço de e-mail de um utilizador que é um administrador de faturação da conta que será o novo proprietário para a subscrição e, em seguida, selecione o pedido de **transferência de envio**</span><span class="sxs-lookup"><span data-stu-id="4d5b1-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="4d5b1-110">O utilizador recebe um e-mail com instruções para rever o seu pedido de transferência.</span><span class="sxs-lookup"><span data-stu-id="4d5b1-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="4d5b1-111">Para aprovar o pedido de transferência, o utilizador seleciona o link no e-mail e segue as instruções.</span><span class="sxs-lookup"><span data-stu-id="4d5b1-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="4d5b1-112">**Nota:** Se transferir a propriedade da faturação da sua subscrição para a conta de um utilizador em outro inquilino da AD Azure, todas as atribuições de controlo de acesso baseado em [funções (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)para gerir recursos na subscrição são permanentemente removidas.</span><span class="sxs-lookup"><span data-stu-id="4d5b1-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="4d5b1-113">Apenas o novo proprietário terá acesso à gestão de recursos na subscrição.</span><span class="sxs-lookup"><span data-stu-id="4d5b1-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="4d5b1-114">Para obter mais informações, consulte [a subscrição de Transferência para um utilizador em outro inquilino AD Azure.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="4d5b1-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="4d5b1-115">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="4d5b1-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="4d5b1-116">Transferir a propriedade de uma subscrição do Azure para outra conta</span><span class="sxs-lookup"><span data-stu-id="4d5b1-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="4d5b1-117">Sobre a transferência de propriedade de faturação para uma subscrição do Azure</span><span class="sxs-lookup"><span data-stu-id="4d5b1-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="4d5b1-118">Transfering Visual Studio, Microsoft Partner Network (MPN) e Pay à medida que vai de dev/Test subscrições</span><span class="sxs-lookup"><span data-stu-id="4d5b1-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="4d5b1-119">Transfer Ownership FAQ</span><span class="sxs-lookup"><span data-stu-id="4d5b1-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="4d5b1-120">Problemas de transferência Questões de Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d5b1-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
