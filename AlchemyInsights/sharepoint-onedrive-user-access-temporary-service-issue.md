---
title: Questões de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771255"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="89c1b-102">SharePoint ou OneDrive Lento, Inacessível ou Indisponível para Vários Utilizadores</span><span class="sxs-lookup"><span data-stu-id="89c1b-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="89c1b-103">Se um site OneDrive ou SharePoint não estiver disponível para vários utilizadores que tiveram acesso anteriormente, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="89c1b-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="89c1b-104">[Verifique o painel de saúde do serviço.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="89c1b-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="89c1b-105">**Adicionar e licenciar o utilizador**</span><span class="sxs-lookup"><span data-stu-id="89c1b-105">**Add and license the user**</span></span>

<span data-ttu-id="89c1b-106">Certifique-se de atribuir [licenças aos utilizadores da Microsoft 365 para negócios.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="89c1b-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="89c1b-107">**Atribuir permissões**</span><span class="sxs-lookup"><span data-stu-id="89c1b-107">**Assign Permissions**</span></span>

<span data-ttu-id="89c1b-108">Se o utilizador tiver recebido uma licença Sharepoint e ainda estiver a receber uma mensagem de acesso negada, certifique-se de que tem o [nível de permissão adequado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atribuído.</span><span class="sxs-lookup"><span data-stu-id="89c1b-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="89c1b-109">**Considere usar a funcionalidade de pedido de acesso**</span><span class="sxs-lookup"><span data-stu-id="89c1b-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="89c1b-110">A [funcionalidade de pedido](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) de acesso permite que as pessoas solicitem acesso a conteúdos que não têm atualmente permissão para ver.</span><span class="sxs-lookup"><span data-stu-id="89c1b-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="89c1b-111">**Permitir scripts personalizados pode causar acesso a problemas negados**</span><span class="sxs-lookup"><span data-stu-id="89c1b-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="89c1b-112">Existem certos cenários em que a funcionalidade *de script personalizado Permitir* pode estar a apresentar um acesso negado.</span><span class="sxs-lookup"><span data-stu-id="89c1b-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="89c1b-113">Para uma lista de funcionalidades afetadas, considerações de segurança e a capacidade de desativar a funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="89c1b-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="89c1b-114">Visite [o Allow ou evite scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="89c1b-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

