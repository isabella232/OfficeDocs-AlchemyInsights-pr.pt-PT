---
title: Resolver mensagens de acesso negado
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760351"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="f9f44-102">Resolução de problemas de acesso negado mensagens no Centro de administração do Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="f9f44-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="f9f44-103">Se estiver a receber uma mensagem de acesso negado ao tentar navegar para um centro de administração do Sharepoint/OneDrive, certifique-se que [atribua uma licença para o utilizador](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="f9f44-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="f9f44-104">Se o utilizador tiver uma licença, deve também certificar-se de que são [atribuídos uma função de administrador](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) que pode aceder os centros de admin.</span><span class="sxs-lookup"><span data-stu-id="f9f44-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="f9f44-105">Este problema também pode ocorrer quando um utilizador é eliminado e recriado com o mesmo nome principal de utilizador (UPN).</span><span class="sxs-lookup"><span data-stu-id="f9f44-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="f9f44-106">A nova conta é criada utilizando um valor diferente de PUID (ID exclusivo do Passport).</span><span class="sxs-lookup"><span data-stu-id="f9f44-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="f9f44-107">Quando o utilizador tenta aceder a uma colecção de sites ou seu OneDrive, o utilizador tem um PUID incorrecto.</span><span class="sxs-lookup"><span data-stu-id="f9f44-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="f9f44-108">Um segundo cenário envolve a sincronização de directório com uma unidade organizacional (UO) de Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f9f44-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="f9f44-109">Se os utilizadores já iniciado sessão no SharePoint e, em seguida, são movidos para uma UO diferente e resynced com o SharePoint, eles poderão detectar este problema.</span><span class="sxs-lookup"><span data-stu-id="f9f44-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="f9f44-110">Para resolver este problema, deverá restaurar o UPN original com os passos no artigo [restaurar um utilizador no Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f9f44-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="f9f44-111">Nota: Se um centro de OneDrive ou de administração do SharePoint não está disponível para vários utilizadores, que tinham anteriormente acesso, poderá existir um problema de serviço temporária.</span><span class="sxs-lookup"><span data-stu-id="f9f44-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="f9f44-112">[Verifique o dashboard de estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f9f44-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


