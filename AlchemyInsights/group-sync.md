---
title: Sincronização de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256789"
---
# <a name="group-sync"></a><span data-ttu-id="0e8dc-102">Sincronização de grupo</span><span class="sxs-lookup"><span data-stu-id="0e8dc-102">Group sync</span></span>

<span data-ttu-id="0e8dc-103">Este artigo fornece orientações sobre a sincronização de grupos.</span><span class="sxs-lookup"><span data-stu-id="0e8dc-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="0e8dc-104">Se um administrador global ou dono de grupo não for capaz de modificar propriedades de grupo ou adicionar membros ou atribuir proprietários no portal Azure, certifique-se de que a fonte da autoridade para o grupo é Azure Ative Directory (Azure AD) para o administrador global ou proprietário do grupo para modificar o grupo.</span><span class="sxs-lookup"><span data-stu-id="0e8dc-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="0e8dc-105">Antes de tentar eliminar um grupo sincronizado em Azure AD, certifique-se de que [apagou todas as licenças atribuídas](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) para evitar erros.</span><span class="sxs-lookup"><span data-stu-id="0e8dc-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="0e8dc-106">Para compreender como sincronizar utilizadores, grupos e contactos, consulte [o Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)e siga [sincronizar um grupo no local para a Azure utilizando o Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) para sincronizar grupos on-perm utilizando a ligação AD.</span><span class="sxs-lookup"><span data-stu-id="0e8dc-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="0e8dc-107">Siga este guia [Erros de resolução de problemas durante](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) a sincronização para resolver erros comuns durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="0e8dc-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

