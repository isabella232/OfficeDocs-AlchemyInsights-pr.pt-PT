---
title: Eliminar permanentemente um site no SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955242"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="20639-102">Eliminar permanentemente um site no SharePoint</span><span class="sxs-lookup"><span data-stu-id="20639-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="20639-103">Para reutilizar um URL de um site eliminado (para recriar um site) ou para eliminar permanentemente um site porque o mesmo já não está a ser utilizado, pode utilizar a opção **Eliminar Permanentemente** a partir do Novo Centro de Administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="20639-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="20639-104">Aceda a [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) (Página de sites eliminados do novo centro de administração do SharePoint) e inicie sessão com uma conta que tenha permissões de administrador para a sua organização.</span><span class="sxs-lookup"><span data-stu-id="20639-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="20639-105">Na coluna da esquerda, selecione um site.</span><span class="sxs-lookup"><span data-stu-id="20639-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="20639-106">Clique em **Eliminar Permanentemente**.</span><span class="sxs-lookup"><span data-stu-id="20639-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="20639-107">**Nota**: os sites conectados em grupo não podem ser eliminados permanentemente do Novo Centro de Administração do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="20639-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="20639-108">Será necessário utilizar o [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="20639-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="20639-109">Para mais informações, consulte [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) (Eliminar permanentemente um site).</span><span class="sxs-lookup"><span data-stu-id="20639-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
