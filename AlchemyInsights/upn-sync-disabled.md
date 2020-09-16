---
title: UPN sincronizado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749525"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="e0144-102">UPN sincronizado</span><span class="sxs-lookup"><span data-stu-id="e0144-102">UPN sync disabled</span></span>

<span data-ttu-id="e0144-103">Se começou a sincronizar a Azure AD antes de 30 de março de 2016, execute o seguinte cmdlet Azure AD PowerShell para ativar o soft match da UPN apenas para a sua organização:</span><span class="sxs-lookup"><span data-stu-id="e0144-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="e0144-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="e0144-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="e0144-105">UPN soft match é automaticamente ligado para organizações que começaram a sincronizar a Azure AD em ou depois de 30 de março de 2016.</span><span class="sxs-lookup"><span data-stu-id="e0144-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="e0144-106">Para saber mais sobre como permitir uma partida suave na UPN e outras funcionalidades de sincronização, consulte [as funcionalidades do serviço de sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="e0144-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

