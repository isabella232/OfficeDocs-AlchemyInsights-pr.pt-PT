---
title: Não é possível aceder ao SharePoint ou ao centro de administração OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824446"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="96134-102">Não é possível aceder ao SharePoint ou ao centro de administração OneDrive</span><span class="sxs-lookup"><span data-stu-id="96134-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="96134-103">Se o seu site do Centro De Admin SharePoint ou OneDrive estiver inacessível ou indisponível, pode haver um problema de serviço temporário em que os utilizadores experimentem atrasos intermitentes ou erros de navegação ao aceder a sites SharePoint ou conteúdo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="96134-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="96134-104">Consulte o [painel de saúde do Serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se a sua organização está com impacto.</span><span class="sxs-lookup"><span data-stu-id="96134-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="96134-105">É necessário atribuir uma licença do Microsoft Office SharePoint Online aos administradores globais e do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="96134-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="96134-106">As novas contas criadas apenas com uma licença do Microsoft Office SharePoint Online ou uma função de administrador podem ter problemas em aceder ao Microsoft Office SharePoint Online, como "acesso negado" ou "utilizador não encontrado".</span><span class="sxs-lookup"><span data-stu-id="96134-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="96134-107">Aguarde pelo menos 24 horas para que a sincronização seja concluída em todos os sistemas.</span><span class="sxs-lookup"><span data-stu-id="96134-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="96134-108">Compreendemos que 24 horas pode parecer muito tempo.</span><span class="sxs-lookup"><span data-stu-id="96134-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="96134-109">Em muitos casos, estamos a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="96134-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="96134-110">Os utilizadores privilegiados de Gestão de Identidade[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)podem ter acesso negado se a janela de tempo de acesso permitida for muito pequena, ver  [Acesso negado às contas PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="96134-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>