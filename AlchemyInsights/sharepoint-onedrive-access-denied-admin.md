---
title: Solucionações de acesso negado mensagens
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051436"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="5bdd0-102">Soluciona-se o acesso negado mensagens no Sharepoint / OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="5bdd0-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="5bdd0-103">Se você estiver recebendo uma mensagem negada de acesso ao tentar navegar para um Sharepoint / OneDrive Admin Center, certifique-se de que você [atribuir uma licença para o usuário](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="5bdd0-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="5bdd0-104">Se o usuário tiver uma licença, você também deve garantir que eles tenham [uma função](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) de administrador que possa acessar os centros de administração.</span><span class="sxs-lookup"><span data-stu-id="5bdd0-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="5bdd0-105">Esse problema também pode ocorrer quando um usuário é excluído e recriado com o mesmo nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="5bdd0-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="5bdd0-106">A nova conta é criada usando um valor puid diferente (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="5bdd0-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="5bdd0-107">Quando o usuário tenta acessar uma coleção do site ou seu OneDrive, o usuário tem um PUID incorreto.</span><span class="sxs-lookup"><span data-stu-id="5bdd0-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="5bdd0-108">Um segundo cenário envolve sincronização do diretório com uma unidade organizacional do Diretório Ativo (OU).</span><span class="sxs-lookup"><span data-stu-id="5bdd0-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="5bdd0-109">Se os usuários já entraram no SharePoint e, em seguida, forem transferidos para uma OU diferente e resincronizados com o SharePoint, eles podem experimentar esse problema.</span><span class="sxs-lookup"><span data-stu-id="5bdd0-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="5bdd0-110">Para resolver esse problema, você deve restaurar a UPN original com as etapas do artigo, [restaurar um usuário no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="5bdd0-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="5bdd0-111">Nota: Se um centro de administração OneDrive ou SharePoint não estiver disponível para vários usuários que tiveram acesso anteriormente, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="5bdd0-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="5bdd0-112">[Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5bdd0-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


