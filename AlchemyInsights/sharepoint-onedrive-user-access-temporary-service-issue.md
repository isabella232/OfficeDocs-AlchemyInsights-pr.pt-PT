---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053812"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="af171-102">SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários</span><span class="sxs-lookup"><span data-stu-id="af171-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="af171-103">Se um site OneDrive ou SharePoint não estiver disponível para vários usuários que tiveram acesso anteriormente, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="af171-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="af171-104">[Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="af171-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="af171-105">**Adicionar e licenciar o usuário**</span><span class="sxs-lookup"><span data-stu-id="af171-105">**Add and license the user**</span></span>

<span data-ttu-id="af171-106">Certifique-se de atribuir [licenças aos usuários no Office 365 para negócios.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span><span class="sxs-lookup"><span data-stu-id="af171-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="af171-107">**Atribuir permissões**</span><span class="sxs-lookup"><span data-stu-id="af171-107">**Assign Permissions**</span></span>

<span data-ttu-id="af171-108">Se o usuário tiver sido atribuído uma licença Sharepoint e ainda estiver recebendo uma mensagem negada de acesso, certifique-se de que eles tenham o [nível de permissão adequado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atribuído.</span><span class="sxs-lookup"><span data-stu-id="af171-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="af171-109">**Considere usar o recurso de solicitação de acesso**</span><span class="sxs-lookup"><span data-stu-id="af171-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="af171-110">O recurso de [solicitação](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) de acesso permite que as pessoas solicitem acesso a conteúdo que atualmente não têm permissão para ver.</span><span class="sxs-lookup"><span data-stu-id="af171-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="af171-111">**Permitir que o script personalizado pode causar problemas negados de acesso**</span><span class="sxs-lookup"><span data-stu-id="af171-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="af171-112">Há certos cenários em que o recurso *de script personalizado Permitir* pode estar apresentando um acesso negado.</span><span class="sxs-lookup"><span data-stu-id="af171-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="af171-113">Para obter uma lista de recursos afetados, considerações de segurança e a capacidade de desativar o recurso.</span><span class="sxs-lookup"><span data-stu-id="af171-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="af171-114">Visite [Permitir ou evitar script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="af171-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

