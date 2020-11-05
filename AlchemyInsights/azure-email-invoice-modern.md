---
title: Faturação de e-mail moderna Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922140"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="2c540-102">Faturação de e-mail em Azure</span><span class="sxs-lookup"><span data-stu-id="2c540-102">Email invoicing in Azure</span></span>

<span data-ttu-id="2c540-103">Deve ter um proprietário ou um papel de contribuinte no perfil de faturação ou na sua conta de faturação para atualizar a sua preferência por e-mail.</span><span class="sxs-lookup"><span data-stu-id="2c540-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="2c540-104">Uma vez optado, todos os utilizadores com funções de proprietário, colaborador, leitores e gestor de faturas num perfil de faturação receberão a sua fatura por e-mail.</span><span class="sxs-lookup"><span data-stu-id="2c540-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="2c540-105">Inscreva-se no [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2c540-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="2c540-106">Pesquisa de **Gestão de Custos + Faturação.**</span><span class="sxs-lookup"><span data-stu-id="2c540-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="2c540-107">Selecione **Faturas** do lado esquerdo e, em seguida, selecione **e-mail Fatura** a partir do topo da página.</span><span class="sxs-lookup"><span data-stu-id="2c540-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="2c540-108">Se tiver vários perfis de faturação, selecione um perfil de faturação e, em seguida, **selecione Opt in**.</span><span class="sxs-lookup"><span data-stu-id="2c540-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="2c540-109">Selecione **Update**.</span><span class="sxs-lookup"><span data-stu-id="2c540-109">Select **Update**.</span></span>
6. <span data-ttu-id="2c540-110">Se tiver vários perfis de faturação, selecione um perfil de faturação e, em seguida, **selecione Opt in**.</span><span class="sxs-lookup"><span data-stu-id="2c540-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="2c540-111">Você dá aos outros acesso para visualizar, transferir e pagar faturas atribuindo-lhes o papel de gestor de fatura para um perfil de faturação MCA ou MPA.</span><span class="sxs-lookup"><span data-stu-id="2c540-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="2c540-112">Se optou por obter a sua fatura por e-mail, os utilizadores também recebem as faturas por e-mail.</span><span class="sxs-lookup"><span data-stu-id="2c540-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="2c540-113">Inscreva-se no [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2c540-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="2c540-114">Pesquisa de **Gestão de Custos + Faturação.**</span><span class="sxs-lookup"><span data-stu-id="2c540-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="2c540-115">Selecione **perfis de Faturação** do lado esquerdo.</span><span class="sxs-lookup"><span data-stu-id="2c540-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="2c540-116">A partir da lista de perfis de faturação, selecione um perfil de faturação para o qual pretende atribuir uma função de gestor de fatura.</span><span class="sxs-lookup"><span data-stu-id="2c540-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="2c540-117">Selecione **Access Control (IAM)** do lado esquerdo e, em seguida, selecione **Adicionar** a partir do topo da página.</span><span class="sxs-lookup"><span data-stu-id="2c540-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="2c540-118">Na lista de drop-down de função, **selecione Gestor de Faturas**.</span><span class="sxs-lookup"><span data-stu-id="2c540-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="2c540-119">Insira o endereço de e-mail do utilizador para dar acesso.</span><span class="sxs-lookup"><span data-stu-id="2c540-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="2c540-120">**Selecione Guardar** para atribuir o papel.</span><span class="sxs-lookup"><span data-stu-id="2c540-120">Select **Save** to assign the role.</span></span>
