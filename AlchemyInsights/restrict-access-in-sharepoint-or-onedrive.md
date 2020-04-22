---
title: Restringir o acesso no SharePoint ou oneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715895"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a1a42-102">Restringir o acesso no SharePoint ou oneDrive</span><span class="sxs-lookup"><span data-stu-id="a1a42-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a1a42-103">No SharePoint e no OneDrive, restringe o acesso a itens como ficheiros, pastas e listas, concedendo acesso apenas a grupos ou indivíduos que deseja ter acesso.</span><span class="sxs-lookup"><span data-stu-id="a1a42-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="a1a42-104">Por padrão, as permissões no SharePoint são herdadas de um alto na hierarquia.</span><span class="sxs-lookup"><span data-stu-id="a1a42-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="a1a42-105">Assim, um ficheiro herda as suas permissões da pasta, que herda as suas permissões da biblioteca, que herda as suas permissões a partir do site.</span><span class="sxs-lookup"><span data-stu-id="a1a42-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="a1a42-106">Você pode compartilhar a um nível mais alto (como por exemplo, partilhando um site inteiro) e, em seguida, quebrar a herança se você não quiser compartilhar todos os itens no site.</span><span class="sxs-lookup"><span data-stu-id="a1a42-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="a1a42-107">No entanto, não recomendamos isto porque torna a manutenção das permissões mais complexas e confusas no futuro.</span><span class="sxs-lookup"><span data-stu-id="a1a42-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="a1a42-108">Eis o que podias fazer em vez disso:</span><span class="sxs-lookup"><span data-stu-id="a1a42-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="a1a42-109">Se, por exemplo, quiser partilhar todo o conteúdo de uma pasta, exceto um ficheiro, mude esse ficheiro para um novo local que não seja partilhado.</span><span class="sxs-lookup"><span data-stu-id="a1a42-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="a1a42-110">Se tiver duas subpastas numa pasta e pretender partilhar uma subpasta com os grupos A e B e permitir apenas o acesso do grupo A à segunda subpasta, partilhe a pasta-mãe com o grupo A e adicione o grupo B à primeira subpasta.</span><span class="sxs-lookup"><span data-stu-id="a1a42-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="a1a42-111">Pare de partilhar um ficheiro ou pasta</span><span class="sxs-lookup"><span data-stu-id="a1a42-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

