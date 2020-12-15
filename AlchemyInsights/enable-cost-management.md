---
title: Permitir a gestão de custos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678768"
---
# <a name="enable-cost-management"></a><span data-ttu-id="8ba0f-102">Permitir a gestão de custos</span><span class="sxs-lookup"><span data-stu-id="8ba0f-102">Enable cost management</span></span>

<span data-ttu-id="8ba0f-103">**O que significa "custos para a sua organização"?**</span><span class="sxs-lookup"><span data-stu-id="8ba0f-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="8ba0f-104">As organizações que utilizam contas do Enterprise Agreement (EA) ou do Microsoft Customer Agreement (MCA) podem desativar o acesso à informação de custos e à informação sobre preços.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="8ba0f-105">Depois de iniciar sessão no portal Azure, podem usar as APIs de Faturação para obter faturas programáticas (uma vez optadas) e detalhes de utilização.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="8ba0f-106">**Como permitir que utilizadores adicionais acedam a faturas**</span><span class="sxs-lookup"><span data-stu-id="8ba0f-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="8ba0f-107">Aceda à **lâmina de Subscrições** no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="8ba0f-108">Selecione **Faturas** e, em seguida, **Aceda às faturas.**</span><span class="sxs-lookup"><span data-stu-id="8ba0f-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="8ba0f-109">Ligue o acesso, seguido de guardar as alterações, para permitir que os utilizadores em funções de aplicação de subscrição descarreguem faturas.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="8ba0f-110">O Administrador de Conta também pode configurar para ter faturas enviadas por e-mail.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="8ba0f-111">Para saber mais, consulte [a sua fatura por e-mail.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)</span><span class="sxs-lookup"><span data-stu-id="8ba0f-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="8ba0f-112">**Como adicionar utilizadores ao papel de Billing Reader**</span><span class="sxs-lookup"><span data-stu-id="8ba0f-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="8ba0f-113">Aceda à **lâmina de Subscrições** no portal Azure.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="8ba0f-114">Selecione **o controlo de acesso (IAM)** e, em seguida, clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="8ba0f-115">Escolha **o Leitor de Faturação** na página De **seleção de funções.**</span><span class="sxs-lookup"><span data-stu-id="8ba0f-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="8ba0f-116">Digite o e-mail do utilizador que pretende convidar e, em seguida, clique **em OK** para enviar o convite.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="8ba0f-117">Siga as instruções fornecidas no e-mail de convite para fazer login como leitor de faturação.</span><span class="sxs-lookup"><span data-stu-id="8ba0f-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="8ba0f-118">Para mais informações, consulte [o Acesso do Grant à Billing.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)</span><span class="sxs-lookup"><span data-stu-id="8ba0f-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="8ba0f-119">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="8ba0f-119">**Recommended documents**</span></span>

- [<span data-ttu-id="8ba0f-120">Ativar vistas da DA e AO através do portal EA</span><span class="sxs-lookup"><span data-stu-id="8ba0f-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="8ba0f-121">Custos incluídos na Gestão de Custos</span><span class="sxs-lookup"><span data-stu-id="8ba0f-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="8ba0f-122">Ofertas suportadas do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="8ba0f-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="8ba0f-123">Rever os custos na análise de custos</span><span class="sxs-lookup"><span data-stu-id="8ba0f-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="8ba0f-124">Fornecer acesso a informações de faturação</span><span class="sxs-lookup"><span data-stu-id="8ba0f-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8ba0f-125">Verifique o acesso a um Acordo de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8ba0f-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






