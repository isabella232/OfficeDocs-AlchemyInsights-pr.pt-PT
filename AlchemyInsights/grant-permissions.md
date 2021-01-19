---
title: Conceder permissões
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901612"
---
# <a name="grant-permissions"></a><span data-ttu-id="d0226-102">Conceder permissões</span><span class="sxs-lookup"><span data-stu-id="d0226-102">Grant permissions</span></span>

1. <span data-ttu-id="d0226-103">**Concessão de consentimento administrativo em todo** o inquilino : Consulte o consentimento da [administração do arrendatário para um pedido](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) de instruções passo a passo para conceder o consentimento administrativo do portal Azure, utilizando a Azure AD PowerShell, ou a partir do consentimento.</span><span class="sxs-lookup"><span data-stu-id="d0226-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="d0226-104">**Concessão de consentimento em nome de um utilizador específico**: Em vez de conceder o consentimento para toda a organização, um administrador também pode usar a [API do Microsoft Graph](https://docs.microsoft.com/graph/use-the-api) para conceder consentimento a permissões delegadas em nome de um único utilizador.</span><span class="sxs-lookup"><span data-stu-id="d0226-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="d0226-105">Para mais informações, consulte [Obter acesso em nome de um utilizador](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="d0226-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>