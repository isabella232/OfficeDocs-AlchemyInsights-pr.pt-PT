---
title: Resolução de problemas de associação ao Azure AD Híbrido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401918"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="3321c-102">Resolução de problemas de associação ao Azure AD Híbrido</span><span class="sxs-lookup"><span data-stu-id="3321c-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="3321c-103">Altamente recomendado certifique-se de que um dispositivo pode aceder aos pontos finais de registo de dispositivos na conta do sistema ao utilizar o [script "Test Device Registration Connectivity"](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="3321c-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="3321c-104">Se estiver a configurar registos de dispositivos pela primeira vez, consulte [Introdução à gestão de dispositivos no Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) para saber como colocar dispositivos sob o controlo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3321c-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="3321c-105">Se estiver a registar dispositivos no Azure AD diretamente e a inscrevê-los no Intune, certifique-se primeiro de que [configurou o Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e de que tem [licenças](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) disponíveis.</span><span class="sxs-lookup"><span data-stu-id="3321c-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="3321c-106">Certifique-se de que tem autorização para executar operações no Azure AD e no AD no local.</span><span class="sxs-lookup"><span data-stu-id="3321c-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="3321c-107">Apenas um administrador global no Azure AD pode gerir as definições dos registos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3321c-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="3321c-108">Além disso, se estiver a configurar o registo automático no seu Active Directory no local, terá de ser um administrador do Active Directory e do AD FS (se aplicável).</span><span class="sxs-lookup"><span data-stu-id="3321c-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="3321c-109">Para obter mais detalhes sobre como resolver potenciais problemas de associação ao Azure AD híbrido, consulte [Resolução de Problemas de Associação ao Azure AD híbrido](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Para configurar a associação ao Azure AD híbrido e Gerir Dispositivos através do portal Azure AD, consulte [Configurar dispositivos associados ao Azure AD híbrido (associados a um domínio no local)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) e [Gerir dispositivos através do portal do Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3321c-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3321c-110">Para resolver problemas comuns com a associação ao Azure Active Directory Híbrido (AD), consulte [FAQ sobre a associação ao Azure AD híbrido](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="3321c-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
