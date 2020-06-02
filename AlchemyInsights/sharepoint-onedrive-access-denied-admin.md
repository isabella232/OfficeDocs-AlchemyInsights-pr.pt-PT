---
title: Acesso a resolução de problemas Mensagens negadas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505390"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="99170-102">Acesso a resolução de problemas Mensagens negadas no Sharepoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="99170-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="99170-103">Se estiver a receber uma mensagem de acesso negada ao tentar navegar para um Sharepoint/OneDrive Admin Center, certifique-se de que [atribui uma licença ao utilizador](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="99170-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="99170-104">Se o utilizador tiver uma licença, deve também certificar-se de que lhes é [atribuída uma função de administrador](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) que pode aceder aos centros de administração.</span><span class="sxs-lookup"><span data-stu-id="99170-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="99170-105">Este problema também pode ocorrer quando um utilizador é eliminado e recriado com o mesmo nome principal do utilizador (UPN).</span><span class="sxs-lookup"><span data-stu-id="99170-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="99170-106">A nova conta é criada utilizando um valor puid diferente (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="99170-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="99170-107">Quando o utilizador tenta aceder a uma coleção de sites ou ao seu OneDrive, o utilizador tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="99170-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="99170-108">Um segundo cenário envolve a sincronização do diretório com uma unidade organizacional ative directy (OU).</span><span class="sxs-lookup"><span data-stu-id="99170-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="99170-109">Se os utilizadores já se inscreveram no SharePoint, e depois forem transferidos para um OU diferente e resincamados com o SharePoint, poderão experimentar este problema.</span><span class="sxs-lookup"><span data-stu-id="99170-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="99170-110">Para resolver este problema, deverá restaurar a UPN original com os passos do artigo, [Restaurar um utilizador na Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="99170-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="99170-111">Nota: Se um centro de administração OneDrive ou SharePoint não estiver disponível para vários utilizadores que tenham tido acesso anteriormente, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="99170-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="99170-112">[Verifique o painel de saúde do serviço.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="99170-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


