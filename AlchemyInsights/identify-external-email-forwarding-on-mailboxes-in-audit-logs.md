---
title: Identificar o reencaminhamento de correio electrónico externo nas caixas de correio nos registos de auditoria
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909465"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="47710-102">Identificar quando o reencaminhamento de correio electrónico externo está configurado nas caixas de correio</span><span class="sxs-lookup"><span data-stu-id="47710-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="47710-103">Quando um utilizador configura o reencaminhamento de correio electrónico externo numa caixa de correio, a actividade é auditada como parte do cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="47710-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="47710-104">Pode ver a actividade de utilizar a procura de registo de auditoria no & Security Center de conformidade.</span><span class="sxs-lookup"><span data-stu-id="47710-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="47710-105">Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="47710-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="47710-106">Clique em **Procurar e de investigação** e seleccione a **Procura de registo de auditoria**.</span><span class="sxs-lookup"><span data-stu-id="47710-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="47710-107">Seleccione o intervalo de datas nos campos **data de início** e **data de fim** .</span><span class="sxs-lookup"><span data-stu-id="47710-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="47710-108">Não é necessário especificar um nome de utilizador.</span><span class="sxs-lookup"><span data-stu-id="47710-108">You don't need to specify a username.</span></span> <span data-ttu-id="47710-109">Verifique se que o campo de **actividades** é definido para **Mostrar resultados para todas as actividades**.</span><span class="sxs-lookup"><span data-stu-id="47710-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="47710-110">Clique em **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="47710-110">Click **Search**.</span></span>

<span data-ttu-id="47710-111">Nos resultados, clique em **Resultados de filtro** e escreva **Set-Mailbox** na caixa de actividade de filtragem.</span><span class="sxs-lookup"><span data-stu-id="47710-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="47710-112">Seleccione um registo de auditoria nos resultados.</span><span class="sxs-lookup"><span data-stu-id="47710-112">Select an audit record in the results.</span></span> <span data-ttu-id="47710-113">Na lista de opções de **Detalhes** , clique em **obter mais informações**.</span><span class="sxs-lookup"><span data-stu-id="47710-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="47710-114">Devem observar os detalhes de cada registo de auditoria para determinar se a actividade está relacionada para reencaminhamento de correio electrónico.</span><span class="sxs-lookup"><span data-stu-id="47710-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="47710-115">**ObjectId**: O valor de alias da caixa de correio que foi modificado.</span><span class="sxs-lookup"><span data-stu-id="47710-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="47710-116">**Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de correio electrónico de destino.</span><span class="sxs-lookup"><span data-stu-id="47710-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="47710-117">**ID de utilizador**: O utilizador configurado reencaminhamento de correio electrónico na caixa de correio no campo **ID de objecto** .</span><span class="sxs-lookup"><span data-stu-id="47710-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="47710-118">Para mais informações, consulte [determinar que configurou para uma caixa de correio de reencaminhamento de correio electrónico](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="47710-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
