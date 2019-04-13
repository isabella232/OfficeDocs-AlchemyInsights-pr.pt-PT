---
title: 932 AADConnect actualizar
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858971"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="ef69d-102">Actualização Azure AD ligar</span><span class="sxs-lookup"><span data-stu-id="ef69d-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="ef69d-103">Por predefinição, a actualização automática está activada para Azure ligar AD, que ajuda a garantir está a executar a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="ef69d-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="ef69d-104">Para verificar as definições de actualização automáticas, utilize o cmdlet **Get-ADSyncAutoUpgrade** no PowerShell de AD Azure.</span><span class="sxs-lookup"><span data-stu-id="ef69d-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="ef69d-105">O cmdlet irá devolver um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="ef69d-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="ef69d-106">**Activado**: actualização automática está activada.</span><span class="sxs-lookup"><span data-stu-id="ef69d-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="ef69d-107">**Desactivado**: actualização automática está desactivada.</span><span class="sxs-lookup"><span data-stu-id="ef69d-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="ef69d-108">**Suspenso**: O sistema já não é elegível para receber actualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="ef69d-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="ef69d-109">Não é possível configurar este valor; é definida pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ef69d-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="ef69d-110">Para mais informações, consulte [actualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="ef69d-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="ef69d-111">Para transferir a versão mais recente do Azure AD ligar, vá para [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="ef69d-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
