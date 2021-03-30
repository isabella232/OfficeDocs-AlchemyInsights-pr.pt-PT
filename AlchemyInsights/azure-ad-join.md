---
title: Azure Ative Directy junta-se
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405676"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="f0278-102">Azure Ative Directy junta-se</span><span class="sxs-lookup"><span data-stu-id="f0278-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="f0278-103">Se estiver a configurar os registos do dispositivo pela primeira vez, certifique-se de que reviu [a Introdução à gestão do dispositivo no Azure Ative Directory](/azure/active-directory/devices/overview) que o irá orientar sobre como colocar os Dispositivos sob o controlo da Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0278-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="f0278-104">Se estiver a registar os dispositivos no Azure AD diretamente e a inscrevê-los no Intune, terá de se certificar de que [tem configurado Intune](/mem/intune/enrollment/device-enrollment) e ter o [licenciamento](/mem/intune/fundamentals/licenses-assign) em primeiro lugar.</span><span class="sxs-lookup"><span data-stu-id="f0278-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="f0278-105">Certifique-se de que está autorizado a realizar operações no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0278-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="f0278-106">Apenas um administrador global em Azure AD pode gerir as definições para registos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f0278-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="f0278-107">Para fazer a Azure AD aderir à implementação, consulte [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="f0278-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="f0278-108">Para obter mais detalhes sobre a resolução de problemas comuns com a aderência do Azure AD, consulte [Azure Ad Join FAQ](/azure/active-directory/devices/faq) e para o windows 10 pro device, ver [Não conseguir juntar a máquina do Windows 10 Pro ao Azure AD - Precisa de atualizar para - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span><span class="sxs-lookup"><span data-stu-id="f0278-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
