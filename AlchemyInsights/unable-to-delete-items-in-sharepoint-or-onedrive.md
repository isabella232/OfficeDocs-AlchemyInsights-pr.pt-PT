---
title: Incapaz de excluir itens no SharePoint ou No OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049528"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="83854-102">Incapaz de excluir itens</span><span class="sxs-lookup"><span data-stu-id="83854-102">Unable to delete items</span></span>

<span data-ttu-id="83854-103">Tendo problemas para excluir itens do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="83854-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="83854-104">Certifique-se sempre de ter as [permissões apropriadas](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) para excluir o item ou ter uma tentativa de administrador de coleta do [site](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) remover o item.</span><span class="sxs-lookup"><span data-stu-id="83854-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="83854-105">Certifique-se de que não há uma configuração de política de [retenção](https://docs.microsoft.com/office365/securitycompliance/retention-policies) no item.</span><span class="sxs-lookup"><span data-stu-id="83854-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="83854-106">Certifique-se de que o item não seja [verificado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para outro usuário.</span><span class="sxs-lookup"><span data-stu-id="83854-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="83854-107">Finalmente, os administradores podem usar [padrões e práticas do SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos da PowerShell que permitem que você execute ações de gerenciamento complexas, como a exclusão de força de itens teimosos.</span><span class="sxs-lookup"><span data-stu-id="83854-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="83854-108">Remover arquivo PNP</span><span class="sxs-lookup"><span data-stu-id="83854-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="83854-109">Remover pasta PNP</span><span class="sxs-lookup"><span data-stu-id="83854-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="83854-110">Remover o item da lista PNP</span><span class="sxs-lookup"><span data-stu-id="83854-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="83854-111">Remover a lista pnp</span><span class="sxs-lookup"><span data-stu-id="83854-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="83854-112">Remover o campo pnp (coluna)</span><span class="sxs-lookup"><span data-stu-id="83854-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)