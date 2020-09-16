---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720693"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="394e5-102">Restringir o acesso no SharePoint ou no OneDrive</span><span class="sxs-lookup"><span data-stu-id="394e5-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="394e5-103">No SharePoint e no OneDrive, restringe o acesso a itens como ficheiros, pastas e listas, concedendo acesso apenas a grupos ou indivíduos a que pretende ter acesso.</span><span class="sxs-lookup"><span data-stu-id="394e5-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="394e5-104">Por padrão, as permissões no SharePoint são herdadas do alto da hierarquia.</span><span class="sxs-lookup"><span data-stu-id="394e5-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="394e5-105">Assim, um ficheiro herda as suas permissões da pasta, que herda as suas permissões da biblioteca, que herda as suas permissões do site.</span><span class="sxs-lookup"><span data-stu-id="394e5-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="394e5-106">Você pode compartilhar a um nível mais alto (como por exemplo, compartilhando um site inteiro) e, em seguida, quebrar a herança se você não quiser compartilhar todos os itens no site.</span><span class="sxs-lookup"><span data-stu-id="394e5-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="394e5-107">No entanto, não recomendamos isto porque torna a manutenção das permissões mais complexa e confusa no futuro.</span><span class="sxs-lookup"><span data-stu-id="394e5-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="394e5-108">Eis o que pode fazer em vez disso:</span><span class="sxs-lookup"><span data-stu-id="394e5-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="394e5-109">Se, por exemplo, quiser partilhar todo o conteúdo de uma pasta, exceto um ficheiro, mova esse ficheiro para um novo local que não seja partilhado.</span><span class="sxs-lookup"><span data-stu-id="394e5-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="394e5-110">Se tiver duas sub-dobras numa pasta e quiser partilhar uma sub-dobradura com os grupos A e B e permitir apenas o acesso do grupo A à segunda sub-dobra, partilhe a pasta dos pais com o grupo A e adicione o grupo B à primeira sub-dobra.</span><span class="sxs-lookup"><span data-stu-id="394e5-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="394e5-111">Pare de partilhar um ficheiro ou pasta </span><span class="sxs-lookup"><span data-stu-id="394e5-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

