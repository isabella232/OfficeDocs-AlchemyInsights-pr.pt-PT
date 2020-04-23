---
title: 932 Upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766504"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="dd1bf-102">Upgrade Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="dd1bf-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="dd1bf-103">Por predefinição, a atualização automática está ativada para o Azure AD Connect, o que ajuda a garantir que está a executar a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="dd1bf-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="dd1bf-104">Para verificar as definições de atualização automática, utilize o **cmdlet Get-ADSyncAutoUpgrade** em Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dd1bf-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="dd1bf-105">O cmdlet devolverá um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="dd1bf-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="dd1bf-106">**Ativado**: Está ativada a atualização automática.</span><span class="sxs-lookup"><span data-stu-id="dd1bf-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="dd1bf-107">**Desativado**: A atualização automática está desativada.</span><span class="sxs-lookup"><span data-stu-id="dd1bf-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="dd1bf-108">**Suspenso**: O sistema já não é elegível para receber atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="dd1bf-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="dd1bf-109">Não é possível configurar este valor; é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="dd1bf-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="dd1bf-110">Para mais informações, consulte [a atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="dd1bf-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="dd1bf-111">Para descarregar a versão mais recente do [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Azure AD Connect, vá a .</span><span class="sxs-lookup"><span data-stu-id="dd1bf-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
