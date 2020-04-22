---
title: Acesso de problemas Mensagens negadas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758493"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="a2534-102">Acesso de problemas Mensagens negadas no Sharepoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="a2534-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="a2534-103">Se estiver a receber uma mensagem negada de acesso ao tentar navegar para um Sharepoint/OneDrive Admin Center, certifique-se de que [atribui uma licença ao utilizador](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="a2534-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="a2534-104">Se o utilizador tiver uma licença, deve também certificar-se de que lhes é [atribuída uma função](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) de administrador que possa aceder aos centros de administração.</span><span class="sxs-lookup"><span data-stu-id="a2534-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="a2534-105">Este problema também pode ocorrer quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN).</span><span class="sxs-lookup"><span data-stu-id="a2534-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a2534-106">A nova conta é criada utilizando um valor DIFERENTE de PUID (Id Exclusivo passaporte).</span><span class="sxs-lookup"><span data-stu-id="a2534-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a2534-107">Quando o utilizador tenta aceder a uma recolha do site ou ao seu OneDrive, o utilizador tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="a2534-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a2534-108">Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional do Diretório Ativo (OU).</span><span class="sxs-lookup"><span data-stu-id="a2534-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a2534-109">Se os utilizadores já se inscreveram no SharePoint, e depois são transferidos para um OU diferente e resincronizados com o SharePoint, podem experimentar este problema.</span><span class="sxs-lookup"><span data-stu-id="a2534-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a2534-110">Para resolver este problema, deve restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a2534-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="a2534-111">Nota: Se um centro de administração OneDrive ou SharePoint não estiver disponível para vários utilizadores que anteriormente tiveram acesso, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="a2534-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="a2534-112">[Verifique o painel de saúde do serviço.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="a2534-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


