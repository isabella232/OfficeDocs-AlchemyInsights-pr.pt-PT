---
title: Monitor Intune Acesso Condicional
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427926"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="ccc25-102">Monitor Intune Acesso Condicional</span><span class="sxs-lookup"><span data-stu-id="ccc25-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="ccc25-103">Os utilizadores direcionados com acesso condicional receberão um e-mail de notificação se não cumprirem os requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="ccc25-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="ccc25-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="ccc25-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="ccc25-105">Caso se presuma que o dispositivo esteja matriculado, aconselhe o utilizador a recorrer à aplicação Portal da Empresa e verificar se aparece no Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="ccc25-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="ccc25-106">Se não o fizer, o utilizador deve inscrever o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ccc25-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="ccc25-107">No portal Azure aceda à conformidade do Dispositivo **Intune**  >  .</span><span class="sxs-lookup"><span data-stu-id="ccc25-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="ccc25-108">Para ver o relatório de conformidade do dispositivo para verificar se o dispositivo do utilizador está marcado como conforme, no **Monitor**, clique na **conformidade do Dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="ccc25-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="ccc25-109">No portal Azure aceda à conformidade do Dispositivo **Intune**  >  .</span><span class="sxs-lookup"><span data-stu-id="ccc25-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="ccc25-110">Em **Gestão,** clique em **Políticas**.</span><span class="sxs-lookup"><span data-stu-id="ccc25-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="ccc25-111">Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do seu utilizador.</span><span class="sxs-lookup"><span data-stu-id="ccc25-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="ccc25-112">Se não for atribuído nenhum perfil, o Intune não poderá confirmar o estado de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ccc25-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="ccc25-113">Editar a atribuição de acesso condicional do utilizador.</span><span class="sxs-lookup"><span data-stu-id="ccc25-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="ccc25-114">No portal Azure, navegue para Políticas de Acesso Condicionado **Intune**  >    >  , selecione uma política da lista e clique em **Utilizadores e grupos**.</span><span class="sxs-lookup"><span data-stu-id="ccc25-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="ccc25-115">Para direcionar uma determinada política a alguém, adicione-a à **lista Incluindo.**</span><span class="sxs-lookup"><span data-stu-id="ccc25-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="ccc25-116">Para garantir que uma pessoa é omitida da apólice, adicione-a à **lista de exclusão**.</span><span class="sxs-lookup"><span data-stu-id="ccc25-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="ccc25-117">**Links úteis:**</span><span class="sxs-lookup"><span data-stu-id="ccc25-117">**Helpful links:**</span></span>

- [<span data-ttu-id="ccc25-118">Visão geral da conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ccc25-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="ccc25-119">Resolução de problemas CA</span><span class="sxs-lookup"><span data-stu-id="ccc25-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="ccc25-120">Política de resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="ccc25-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="ccc25-121">Monitorização da conformidade do dispositivo Intune</span><span class="sxs-lookup"><span data-stu-id="ccc25-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="ccc25-122">Estes passos só são úteis para resolver problemas na resolução do recurso Azure Ative Directory Conditional Access.</span><span class="sxs-lookup"><span data-stu-id="ccc25-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="ccc25-123">Também é possível colocar em quarentena um dispositivo que bloqueia o seu acesso por e-mail com a política de Troca.</span><span class="sxs-lookup"><span data-stu-id="ccc25-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="ccc25-124">Mais informações sobre a gestão do dispositivo Exchange podem ser [**encontradas aqui.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="ccc25-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
