---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719527"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4b1bc-102">SharePoint ou OneDrive lenta, inacessível ou indisponível para múltiplos utilizadores</span><span class="sxs-lookup"><span data-stu-id="4b1bc-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="4b1bc-103">Se um site da OneDrive ou o SharePoint não está disponível para vários utilizadores, que tinham anteriormente acesso, poderá existir um problema de serviço temporária.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="4b1bc-104">[Verifique o dashboard de estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4b1bc-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="4b1bc-105">Adicionar e licenciar o utilizador</span><span class="sxs-lookup"><span data-stu-id="4b1bc-105">Add and license the user</span></span>

<span data-ttu-id="4b1bc-106">Certifique-se de que o utilizador [atribuir licenças aos utilizadores no Office 365 para a empresa](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="4b1bc-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="4b1bc-107">Atribuir permissões</span><span class="sxs-lookup"><span data-stu-id="4b1bc-107">Assign Permissions</span></span>

<span data-ttu-id="4b1bc-108">Se o utilizador tiver sido atribuído uma licença do Sharepoint e continua a receber uma mensagem de acesso negado, certifique-se de que têm o [nível de permissão adequados](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) atribuído.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="4b1bc-109">Considere utilizar a funcionalidade de pedido de acesso</span><span class="sxs-lookup"><span data-stu-id="4b1bc-109">Consider using the access request feature</span></span>

<span data-ttu-id="4b1bc-110">A [funcionalidade de pedido de acesso](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite às pessoas a pedir acesso ao conteúdo que não têm actualmente permissão para ver.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="4b1bc-111">Permitir script personalizado pode fazer com que o acesso negado problemas</span><span class="sxs-lookup"><span data-stu-id="4b1bc-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="4b1bc-112">Existem determinados cenários em que a funcionalidade de *Permitir script personalizado* pode apresentar um acesso negado.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="4b1bc-113">Para uma lista de funcionalidades afectadas, considerações de segurança e a capacidade para desactivar a funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="4b1bc-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="4b1bc-114">Visite [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="4b1bc-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

