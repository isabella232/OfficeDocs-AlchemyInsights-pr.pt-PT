---
title: Invoicing de e-mail do Azure Moderno
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820837"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="716f5-102">Invoicing de e-mail do Azure</span><span class="sxs-lookup"><span data-stu-id="716f5-102">Email invoicing in Azure</span></span>

<span data-ttu-id="716f5-103">Tem de ter um proprietário ou uma função de contribuinte no perfil de faturação ou na sua conta de faturação para atualizar a preferência da fatura por e-mail.</span><span class="sxs-lookup"><span data-stu-id="716f5-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="716f5-104">Assim que optar ativamente por participar, todos os utilizadores com as funções de proprietário, colaborador, leitores e gestor de faturação num perfil de faturação receberão a sua fatura por e-mail.</span><span class="sxs-lookup"><span data-stu-id="716f5-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="716f5-105">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="716f5-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="716f5-106">Procure **Gestão de Custos + Faturação**.</span><span class="sxs-lookup"><span data-stu-id="716f5-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="716f5-107">Selecione **Faturas** do lado esquerdo e, em seguida, selecione **Fatura por e-mail** na parte superior da página.</span><span class="sxs-lookup"><span data-stu-id="716f5-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="716f5-108">Se tiver múltiplos perfis de faturação, selecione um perfil de faturação e, em seguida, selecione **Optar**.</span><span class="sxs-lookup"><span data-stu-id="716f5-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="716f5-109">Selecione **Atualizar**.</span><span class="sxs-lookup"><span data-stu-id="716f5-109">Select **Update**.</span></span>
6. <span data-ttu-id="716f5-110">Se tiver múltiplos perfis de faturação, selecione um perfil de faturação e, em seguida, selecione **Optar**.</span><span class="sxs-lookup"><span data-stu-id="716f5-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="716f5-111">Dá acesso a outras pessoas verem, transferirem, e pagarem faturas ao atribuir-lhes a função gestor de faturas de um perfil de faturação MCA ou MPA.</span><span class="sxs-lookup"><span data-stu-id="716f5-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="716f5-112">Caso tenha optado por obter a sua fatura por e-mail, os utilizadores também receberão as faturas por e-mail.</span><span class="sxs-lookup"><span data-stu-id="716f5-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="716f5-113">Inicie sessão no [portal do Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="716f5-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="716f5-114">Procure **Gestão de Custos + Faturação**.</span><span class="sxs-lookup"><span data-stu-id="716f5-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="716f5-115">Selecione **Perfis de faturação** do lado esquerdo.</span><span class="sxs-lookup"><span data-stu-id="716f5-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="716f5-116">Na lista perfis de faturação, selecione um perfil de faturação ao qual pretende atribuir uma função de gestor de faturas.</span><span class="sxs-lookup"><span data-stu-id="716f5-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="716f5-117">Selecione **Controlo de acesso (IAM)** do lado esquerdo e, em seguida, selecione **Adicionar** na parte superior da página.</span><span class="sxs-lookup"><span data-stu-id="716f5-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="716f5-118">Na lista de opções pendente, selecione **Gestor de faturas**.</span><span class="sxs-lookup"><span data-stu-id="716f5-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="716f5-119">Introduza o endereço de e-mail do utilizador para lhe conceder acesso.</span><span class="sxs-lookup"><span data-stu-id="716f5-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="716f5-120">Selecione **Guardar** para atribuir a função.</span><span class="sxs-lookup"><span data-stu-id="716f5-120">Select **Save** to assign the role.</span></span>
