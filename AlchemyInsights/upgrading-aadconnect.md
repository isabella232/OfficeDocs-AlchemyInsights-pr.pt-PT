---
title: 932 Upgrade AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806050"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="b9080-102">Upgrade Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b9080-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="b9080-103">Por predefinição, a atualização automática está ativada para o Azure AD Connect, o que ajuda a garantir que está a executar a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="b9080-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="b9080-104">Para verificar as definições de atualização automática, utilize o cmdlet **Get-ADSyncAutoUpgrade** em Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b9080-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="b9080-105">O cmdlet devolverá um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="b9080-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="b9080-106">**Ativado**: A atualização automática está ativada.</span><span class="sxs-lookup"><span data-stu-id="b9080-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="b9080-107">**Desativado:** A atualização automática está desativada.</span><span class="sxs-lookup"><span data-stu-id="b9080-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="b9080-108">**Suspenso**: O sistema já não é elegível para receber atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="b9080-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="b9080-109">Não pode configurar este valor; é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b9080-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="b9080-110">Para mais informações, consulte [a atualização automática.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)</span><span class="sxs-lookup"><span data-stu-id="b9080-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="b9080-111">Para descarregar a versão mais recente do Azure AD Connect, vá a [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="b9080-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
