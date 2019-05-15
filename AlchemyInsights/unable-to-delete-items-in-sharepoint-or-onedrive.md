---
title: Não é possível eliminar itens no SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057756"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="6a0ec-102">Não é possível eliminar itens</span><span class="sxs-lookup"><span data-stu-id="6a0ec-102">Unable to delete items</span></span>

<span data-ttu-id="6a0ec-103">Problemas de eliminar itens?</span><span class="sxs-lookup"><span data-stu-id="6a0ec-103">Having issues deleting items?</span></span>

- <span data-ttu-id="6a0ec-104">Sempre certificar-se de que tem as [permissões adequadas](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) para eliminar o item ou ter uma tentativa de [administrador da colecção de site](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) a remover o item.</span><span class="sxs-lookup"><span data-stu-id="6a0ec-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="6a0ec-105">Certifique-se de que não existe uma definição de [política de retenção](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) no item.</span><span class="sxs-lookup"><span data-stu-id="6a0ec-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="6a0ec-106">Certifique-se de que o item não está [reservado](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para outro utilizador.</span><span class="sxs-lookup"><span data-stu-id="6a0ec-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="6a0ec-107">Por último, os administradores podem utilizar o [SharePoint padrões e práticas](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos que lhe permitem executar acções de gestão complexos tais como forçar a eliminação de itens de stubborn do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6a0ec-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="6a0ec-108">Remover ficheiro PNP</span><span class="sxs-lookup"><span data-stu-id="6a0ec-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="6a0ec-109">Remover pasta PNP</span><span class="sxs-lookup"><span data-stu-id="6a0ec-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="6a0ec-110">Remover Item da lista de PNP</span><span class="sxs-lookup"><span data-stu-id="6a0ec-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="6a0ec-111">Remover lista de PNP</span><span class="sxs-lookup"><span data-stu-id="6a0ec-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="6a0ec-112">Remover PNP campo (coluna)</span><span class="sxs-lookup"><span data-stu-id="6a0ec-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)