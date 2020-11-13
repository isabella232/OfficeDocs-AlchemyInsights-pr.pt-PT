---
title: Não é possível eliminar itens no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019594"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="4ff3f-102">Incapaz de eliminar itens</span><span class="sxs-lookup"><span data-stu-id="4ff3f-102">Unable to delete items</span></span>

- <span data-ttu-id="4ff3f-103">As políticas de retenção podem causar isto, você precisa desativar ou excluir o respetivo hold que está causando este problema.</span><span class="sxs-lookup"><span data-stu-id="4ff3f-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="4ff3f-104">Depois de uma política de retenção ou detenção ser removida, pode levar até 24 horas para que a alteração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="4ff3f-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="4ff3f-105">Certifique-se de que não existe uma configuração da política de [retenção](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) no item.</span><span class="sxs-lookup"><span data-stu-id="4ff3f-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="4ff3f-106">O site pode ter excedido o limite de armazenamento, aumentar a quota do [site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) e apagar o item.</span><span class="sxs-lookup"><span data-stu-id="4ff3f-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="4ff3f-107">Certifique-se de que o artigo não é [verificado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) a outro utilizador.</span><span class="sxs-lookup"><span data-stu-id="4ff3f-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="4ff3f-108">Finalmente, os administradores podem usar [Padrões e Práticas sharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) que contém uma biblioteca de comandos PowerShell que lhe permitem executar ações de gestão complexas, tais como a eliminação de itens teimosos.</span><span class="sxs-lookup"><span data-stu-id="4ff3f-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="4ff3f-109">Remover Arquivo PNP</span><span class="sxs-lookup"><span data-stu-id="4ff3f-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="4ff3f-110">Remover pasta PNP</span><span class="sxs-lookup"><span data-stu-id="4ff3f-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="4ff3f-111">Remover item da lista PNP</span><span class="sxs-lookup"><span data-stu-id="4ff3f-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="4ff3f-112">Remover lista PNP</span><span class="sxs-lookup"><span data-stu-id="4ff3f-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="4ff3f-113">Remover campo PNP (Coluna)</span><span class="sxs-lookup"><span data-stu-id="4ff3f-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)