---
title: Identificar reencaminhamento de e-mail externo em caixas de correio em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696308"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="62640-102">Identifique quando o reencaminhamento de e-mail externo é configurado em caixas de correio</span><span class="sxs-lookup"><span data-stu-id="62640-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="62640-103">Quando um utilizador do Microsoft 365 configura o envio de e-mails externos numa caixa de correio, a atividade é auditada como parte do **cmdlet Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="62640-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="62640-104">Pode ver a atividade utilizando a pesquisa de registo de auditoria no Centro de Conformidade & de Segurança.</span><span class="sxs-lookup"><span data-stu-id="62640-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="62640-105">Faça login no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="62640-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="62640-106">Aceda à página de pesquisa de registo de registo de auditoria **de pesquisa.**  >  **Audit log search**</span><span class="sxs-lookup"><span data-stu-id="62640-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="62640-107">Selecione o intervalo de datas nos campos **data de início** e **fim.**</span><span class="sxs-lookup"><span data-stu-id="62640-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="62640-108">Não precisa de especificar um nome de utilizador.</span><span class="sxs-lookup"><span data-stu-id="62640-108">You don't need to specify a username.</span></span> <span data-ttu-id="62640-109">Verifique se o campo **de Atividades** está definido para **mostrar resultados para todas as atividades**.</span><span class="sxs-lookup"><span data-stu-id="62640-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="62640-110">Clique **em Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="62640-110">Click **Search**.</span></span>

<span data-ttu-id="62640-111">Nos resultados, clique em **Resultados do Filtro** e escreva **Set-Mailbox** na caixa de filtro de atividade.</span><span class="sxs-lookup"><span data-stu-id="62640-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="62640-112">Selecione um registo de auditoria nos resultados.</span><span class="sxs-lookup"><span data-stu-id="62640-112">Select an audit record in the results.</span></span> <span data-ttu-id="62640-113">No flyout **Details,** clique **em Mais informações.**</span><span class="sxs-lookup"><span data-stu-id="62640-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="62640-114">Você tem que olhar para os detalhes de cada registo de auditoria para determinar se a atividade está relacionada com o reencaminhamento de e-mail.</span><span class="sxs-lookup"><span data-stu-id="62640-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="62640-115">**ObjectId**: O valor do pseudónimo da caixa de correio que foi modificada.</span><span class="sxs-lookup"><span data-stu-id="62640-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="62640-116">**Parâmetros**: _ReencaminhamentoSmtpAddress_ indica o endereço de e-mail-alvo.</span><span class="sxs-lookup"><span data-stu-id="62640-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="62640-117">**UserId**: O utilizador que configura o reencaminhamento de e-mail na caixa de correio no campo **ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="62640-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="62640-118">Para obter mais informações, consulte [Determineing quem criou o reencaminhamento de e-mail para uma caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="62640-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
