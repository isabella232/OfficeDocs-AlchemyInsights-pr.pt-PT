---
title: Restaurar uma pasta pública eliminada
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063718"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="5fcbd-102">Restaurar uma pasta pública eliminada</span><span class="sxs-lookup"><span data-stu-id="5fcbd-102">Restore a deleted public folder</span></span>

<span data-ttu-id="5fcbd-103">**Para restaurar os itens apagados de uma pasta pública:**</span><span class="sxs-lookup"><span data-stu-id="5fcbd-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="5fcbd-104">Ver [Não pode recuperar itens apagados de uma pasta pública não-mail no Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="5fcbd-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="5fcbd-105">**Para restaurar uma pasta pública eliminada (de qualquer tipo)**:</span><span class="sxs-lookup"><span data-stu-id="5fcbd-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="5fcbd-106">Utilize o seguinte comando EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="5fcbd-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="5fcbd-107">Sintaxe:</span><span class="sxs-lookup"><span data-stu-id="5fcbd-107">Syntax:</span></span>

    ><span data-ttu-id="5fcbd-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse [ ? {$_. Nome -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Path path where the folder will be restored></span><span class="sxs-lookup"><span data-stu-id="5fcbd-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="5fcbd-109">Exemplo: O seguinte comando restaurará a Subpasta1 e colocá-la-á em \Parent1:</span><span class="sxs-lookup"><span data-stu-id="5fcbd-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="5fcbd-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse [ ? {$_. Nome -eq "Subpasta1"}; Set-PublicFolder $pf.identity -Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="5fcbd-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="5fcbd-111">Consulte [restaurar uma pasta pública eliminada](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="5fcbd-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
