---
title: Acesso Condicional de Monitorização
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366439"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="8460c-102">Monitorização do Acesso Condicional para Troca</span><span class="sxs-lookup"><span data-stu-id="8460c-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="8460c-103">Os utilizadores direcionados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="8460c-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="8460c-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="8460c-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="8460c-105">Caso se presuma que o dispositivo esteja matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e verificar se aparece no Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="8460c-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="8460c-106">Se não o fizer, o utilizador deverá inscrever o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8460c-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="8460c-107">No portal Azure vai para a conformidade do Dispositivo Intune >.</span><span class="sxs-lookup"><span data-stu-id="8460c-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="8460c-108">No Monitor clique na conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8460c-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="8460c-109">Consulte o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme.</span><span class="sxs-lookup"><span data-stu-id="8460c-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="8460c-110">No portal Azure vai para a conformidade do Dispositivo Intune >.</span><span class="sxs-lookup"><span data-stu-id="8460c-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="8460c-111">Em Gestão, clique em Políticas.</span><span class="sxs-lookup"><span data-stu-id="8460c-111">Under Manage, click Policies.</span></span> <span data-ttu-id="8460c-112">Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do seu utilizador.</span><span class="sxs-lookup"><span data-stu-id="8460c-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="8460c-113">Se não for atribuído nenhum perfil, o Intune não poderá confirmar o estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8460c-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="8460c-114">Editar a atribuição de acesso condicional do utilizador.</span><span class="sxs-lookup"><span data-stu-id="8460c-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="8460c-115">No portal Azure aceda às Políticas de Acesso Condicionado **Intune**  >  **Conditional access**  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="8460c-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="8460c-116">Selecione uma política da lista.</span><span class="sxs-lookup"><span data-stu-id="8460c-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="8460c-117">Clique em Utilizadores e grupos.</span><span class="sxs-lookup"><span data-stu-id="8460c-117">Click Users and groups.</span></span>
4. <span data-ttu-id="8460c-118">Para direcionar uma determinada política a alguém, adicione-a à lista de incluir.</span><span class="sxs-lookup"><span data-stu-id="8460c-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="8460c-119">Para garantir que uma pessoa é omitida da apólice, adicione-a à lista de exclusão.</span><span class="sxs-lookup"><span data-stu-id="8460c-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="8460c-120">Links úteis:</span><span class="sxs-lookup"><span data-stu-id="8460c-120">Helpful links:</span></span>

[<span data-ttu-id="8460c-121">Visão geral da conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8460c-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="8460c-122">Resolução de problemas CA</span><span class="sxs-lookup"><span data-stu-id="8460c-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="8460c-123">Política de resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="8460c-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="8460c-124">Monitorização da conformidade do dispositivo Intune</span><span class="sxs-lookup"><span data-stu-id="8460c-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="8460c-125">Nota: estes passos só são úteis para resolver problemas na resolução do Azure Ative Directory recurso Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="8460c-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="8460c-126">Também é possível colocar em quarentena um dispositivo que bloqueia o seu acesso por e-mail com a política de Troca.</span><span class="sxs-lookup"><span data-stu-id="8460c-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="8460c-127">Mais informações sobre a gestão do dispositivo Exchange podem ser [encontradas aqui.](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)</span><span class="sxs-lookup"><span data-stu-id="8460c-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
