---
title: Incapaz de eliminar itens no SharePoint ou OneDrive
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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571282"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="853fa-102">Incapaz de apagar itens</span><span class="sxs-lookup"><span data-stu-id="853fa-102">Unable to delete items</span></span>

<span data-ttu-id="853fa-103">As políticas de retenção podem causar isso, você precisa de desativar ou excluir o respetivo porão que está a causar este problema.</span><span class="sxs-lookup"><span data-stu-id="853fa-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="853fa-104">Após a remoção de uma política de retenção ou de espera, pode demorar até 24 horas para que a alteração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="853fa-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="853fa-105">Certifique-se de que não existe uma definição de política de [retenção](https://docs.microsoft.com/office365/securitycompliance/retention-policies) no artigo.</span><span class="sxs-lookup"><span data-stu-id="853fa-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="853fa-106">O site pode ter excedido o limite de armazenamento, aumentado a quota do [site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) e apagado o item.</span><span class="sxs-lookup"><span data-stu-id="853fa-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="853fa-107">Certifique-se de que o artigo não é [verificado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) a outro utilizador.</span><span class="sxs-lookup"><span data-stu-id="853fa-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="853fa-108">Finalmente, os administradores podem usar [Padrões e Práticas SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos PowerShell que lhe permitem realizar ações de gestão complexas, tais como a eliminação de itens teimosos.</span><span class="sxs-lookup"><span data-stu-id="853fa-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="853fa-109">Remover ficheiro PNP</span><span class="sxs-lookup"><span data-stu-id="853fa-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="853fa-110">Remover pasta PNP</span><span class="sxs-lookup"><span data-stu-id="853fa-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="853fa-111">Remover o item da lista PNP</span><span class="sxs-lookup"><span data-stu-id="853fa-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="853fa-112">Remover a lista pnp</span><span class="sxs-lookup"><span data-stu-id="853fa-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="853fa-113">Remover o campo PNP (Coluna)</span><span class="sxs-lookup"><span data-stu-id="853fa-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)